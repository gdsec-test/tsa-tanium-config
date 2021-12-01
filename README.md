# tsa-tanium-config
Environment configuration and customizations for the Tanium platform. Excludes custom content.

# Tanium Architecture
## Production US
Tanium Console: https://tanium.int.gdcorp.tools (VPN required)
![GoDaddy Tanium Architecture (Production US)](/docs/diagrams/res/tanium-architecture-prod-us.png)

## Production EMEA (Works Council)
Tanium Console: https://wc-tanium.int.gdcorp.tools (VPN required)
![GoDaddy Tanium Architecture (Production EMEA WC)](/docs/diagrams/res/tanium-architecture-prod-emea.png)

## Development
Tanium Console: https://tanium-dev.int.gdcorp.tools (VPN required)
![GoDaddy Tanium Architecture (Development)](/docs/diagrams/res/tanium-architecture-dev.png)

# Tanium Console
The configurations described below are (or should be) live in their respective Tanium environments.

See: [Tanium Console User Guide: Customizing the Tanium Console and Interact](https://docs.tanium.com/platform_user/platform_user/console_customizations.html) for up-to-date instructions.
## Console Favicons
Customized console favicons to differentiate between Tanium environments.
### Configure
Tanium Server on Windows only:
* Copy the icon to *$env:PROGRAMFILES\Tanium\Tanium Server\http\tux-console\assets\images\favicon.ico*.
* The change can take a few minutes to apply and requires a browser cache reload.
### Files
* Development: [favicon-dev.ico](https://github.com/gdcorp-infosec/tsa-tanium-config/blob/579fbdf82c4ef32050656969c67397e25642d933/console/favicons/favicon-dev.ico)
* Production EMEA: [favicon-prod-emea.ico](https://github.com/gdcorp-infosec/tsa-tanium-config/blob/579fbdf82c4ef32050656969c67397e25642d933/console/favicons/favicon-prod-emea.ico)
* Production US (Tanium default): [favicon.ico](https://github.com/gdcorp-infosec/tsa-tanium-config/blob/579fbdf82c4ef32050656969c67397e25642d933/console/favicons/favicon.ico)
## Console Logos
Customized console logos to differentiate between Tanium environments.
### How to configure
* Follow the configuration steps in [Tanium Console user guide: Customize the console logo](https://docs.tanium.com/platform_user/platform_user/console_customizations.html#Customize_the_console_logo).
### Files
* Development: [Alt_Logo-dev.png](https://github.com/gdcorp-infosec/tsa-tanium-config/blob/579fbdf82c4ef32050656969c67397e25642d933/console/logos/Alt_Logo-dev.png)
* Production EMEA: [Alt_Logo-prod-emea.png](https://github.com/gdcorp-infosec/tsa-tanium-config/blob/579fbdf82c4ef32050656969c67397e25642d933/console/logos/Alt_Logo-prod-emea.png)
* Production US (Tanium default): [Alt_Logo.svg](https://github.com/gdcorp-infosec/tsa-tanium-config/blob/579fbdf82c4ef32050656969c67397e25642d933/console/logos/Alt_Logo.svg)
## Console Header Text
Customized header text to differentiate between Tanium environments.
### How to configure
Do one of the following:
* Follow the configuration steps in [Tanium Console user guide: Select the Tanium Console header text](https://docs.tanium.com/platform_user/platform_user/console_customizations.html#header_text).
* Alternatively, access Administration > Global Settings and create/edit the setting named `console_headerText` as follows:
  * Value Type: `Text`
  * Type: `Server`
  * Value: `Production US` - Enter the desired header text value.
### Values
* Development: `Development`
* Production EMEA: `Production EMEA (Works Council)`
* Production US: `Production US`
## Console Color
Customized console color to differentiate between Tanium environments.
### How to configure
Do one of the following:
* Follow the configuration steps in [Tanium Console User Guide: Customize the console color](https://docs.tanium.com/platform_user/platform_user/console_customizations.html#Customize_the_console_color).
* To apply a specific color value, access *Administration > Global Settings* and create/edit the setting named `console_consoleColor` as follows:
  * Value Type: `Text`
  * Type: `Server`
  * Value: `#000000` - Enter the hex value for the desired color.
### Values
* Development: `#31F341`
* Production EMEA: `#FFFF33`
* Production US (Tanium default): `#EB3330`
