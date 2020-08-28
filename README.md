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
	4. CSS and Javascript will effect to page speed, so consider size of them and used percent. Should remove code note use in current page.

## Design System
	1. Do not use business to design db such as not use ID of employee to Primary key for employee table => employeeID can change (resign, moving) but reference of employee not change.
	2. System can be lock when log => should not allow this we can use event to publish event to other there process 
	3. Consider to use read and write database to avoid lock system when write and increate reading base on cache.

## Encrypt user data
	1. Problems  => how to emcrypt 

	
# Business question:
 1. Add limit business by on date, Please note that can run on holiday or not working date.
 2. Do not add host name into data to store. In feature we can change host or support mulitiple host.
 
# Maintaince: 
 1. Define task must do to system run such as system need holiday to work, we need update it manulay.
	Ex: we must extend verify PTO day if it at holidy or dateoff.
 2. Tracking all page of website, when deploy new website we know what page should redirect or not.

 
# Reactjs: 
	1. Destructure not destruct of object that ref by property, so change prop of that object not trigger re-render for children component.
	2. Change key of component, that force component will destroy and render new element, (Next user, this case we want re-render all children element with new props)

# PHP:
1. cannot call curl with https
      curl_setopt($ch,CURLOPT_SSL_VERIFYPEER, false);
