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
	
	
