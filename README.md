# iOS-Style-Guide

#### MVVM (Model View ViewModel)

##### Model:

- Purely Entity
- No or very minimum logic
- Don't have any refernece of View
- Only ViewModel has access to it

##### View:

- Basically it's view controller
- It should have no business logic
- Must have ViewModel
- Doesn't pass it's reference to ViewModel
- Update UI according to output from ViewModel
- Navigation logic to different views.

##### ViewModel:

- It should be struct or class as per need. Maximize use of struct.
- It contains business logic. Like Network calls, Database operations, Helper functions.
- It's basic meaning should be it takes input and provides output.
- It should be easily testable.
- All functionalities here should be single purpose.
- Divide into extensions for different part like network, helper functions.

##

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
