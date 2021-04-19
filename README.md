# tsa-tanium-config
Environment configuration and customization for Tanium platform infrastructure.

## Console Favicons
Customized console favicons to differentiate between Tanium environments.
### Configure
Tanium Server on Windows only:
* Copy the icon to *$env:PROGRAMFILES\Tanium\Tanium Server\http\tux-console\assets\images\favicon.ico*.
* The change can take a few minutes to apply and requires a browser cache reload.
### Files
* Development: console\favicons\favicon-dev.ico
* Production EMEA: console\favicons\favicon-prod-emea.ico
* Production US (Tanium default): console\favicons\favicon.ico
## Console Logos
Customized console logos to differentiate between Tanium environments.
### How to configure
* Log into the Tanium Console, access Administration > Miscellaneous > Console Configurations and upload a new file under Console Logo.
* The change can take a few minutes to apply and requires a browser cache reload.
### Files
* Development: console\logos\Alt_Logo-dev.png
* Production EMEA: console\logos\Alt_Logo-prod-emea.png
* Production US (Tanium default) console\logos\Alt_Logo.svg
## Console Header Text
Customized header text to differentiate between Tanium environments.
### How to configure
Do one of the following:
* Log into the Tanium Console, access Administration > Miscellaneous > Console Configurations and enter a new value for Console Header Text.
* Log into the Tanium Console, access Administration > Global Settings and enter a new Text value with Server type with the name *console_headerText*.
### Values
* Development
* Production EMEA (Works Council)
* Production US
## Console Color
Customized console color to differentiate between Tanium environments.
### How to configure
Do one of the following:
* Log into the Tanium Console, access Administration > Miscellaneous > Console Configurations and choose a new color under Console Color.
* Log into the Tanium Console, access Administration > Global Settings and create/edit the setting named *console_consoleColor* with Value Type *Text*, Type *Server*, and the value as a hex color starting with #.
### Values
* Development: #31F341
* Production EMEA: #FFFF33
* Production US (Tanium default): #EB3330