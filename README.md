# Tip
Note all tips

## Localizatin: What is problem with localization:
	1. Message (Error, info) from back end
	2. Update existing  meassage after released.
	3. Space: there some languae don't have space => all translate must put in 1 message. If we split it into multi message we will face with it.
	4. Format message (English: Left to right, Japan: Right to lef).
	5. Length of message will difference with each language => May be break UI
	6. There a some special word will not translate.
	7. Local with login, sigup page => we don't have user so we can't get setting of use. 
		7.1 Using different url for each locale, /en or /ja
		7.2 Not support localization default en
		7.3 Using default en for enter username after that swith to password screen and use setting of user inputed.

## Customize controll
	1. Must support a11y.

## Pagining
	1. How to know what item will be inclued in next page, may be item in before page will be included because there are some item add by user.
		=> we can use time post to sort
	2. Data is returned to fontend should able to view, because fontend can't effect by business such each add more filter.
	and there is bug infiniti scroll, in case check number case to display.

## SEO
	1. How to implement it with single page
	2. Robot.txt
	3. Sitemap.xml

## Design System
	1. Do not use business to design db such as not use ID of employee to Primary key for employee table => employeeID can change (resign, moving) but reference of employee not change.
	2. System can be lock when log => should not allow this we can use event to publish event to other there process 
	3. Consider to use read and write database to avoid lock system when write and increate reading base on cache.

## Encrypt user data
	1. Problems  => how to emcrypt 

	
# Business question:
 1.Add scheduler at day, Please note that can run on holiday or not working date.
 

