# iOS-Style-Guide

#### **Configurations & Schemes**

- Development
- Staging
- Production

It can be have more then 3 configurations depending on the project requirements. Can have different naming conventions too.

##### Application name, bundle identifier, icons should be based on the configurations.
 
##

#### Launch View Controller

 - Purpose is to minimize the code inside Appdelegate.
 - When the app starts it's the first controller loaded after splash and Appdelegate.
 - It's clone of splash screen with the logic.
 - Initialize all shared instances here.
 - Can be easy later on to have a app splash animation.


##
