# iOS-Style-Guide

#### MVVM (Model View ViewModel)

##### Model:

- Purely Entity
- No or very minimum logic
- Don't have any reference of View
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
- Don't know anything about view.

##

#### **Configurations & Schemes**

- Development
- QA
- Staging
- Production

It can have more then 3 configurations depending on the project requirements. Can have different naming conventions too.

##### Note: Application name, bundle identifier, icons should be based on the configurations. Make it shared with other users.

##

#### GitIgnore

```
## Build generated
build/
DerivedData/

## Various settings
*.pbxuser
!default.pbxuser
*.mode1v3
!default.mode1v3
*.mode2v3
!default.mode2v3
*.perspectivev3
!default.perspectivev3
xcuserdata/

## Other
*.moved-aside
*.xccheckout
*.xcscmblueprint

## Obj-C/Swift specific
*.hmap
*.ipa
*.dSYM.zip
*.dSYM

## Playgrounds
timeline.xctimeline
playground.xcworkspace

# Swift Package Manager
#
# Add this line if you want to avoid checking in source code from Swift Package Manager dependencies.
# Packages/
# Package.pins
# Package.resolved
.build/

# CocoaPods
# Pods should be added to repo to make easy for multiple developers.
# Pods/

# Carthage

Carthage/Build

# fastlane

fastlane/report.xml
fastlane/Preview.html
fastlane/screenshots/**/*.png
fastlane/test_output

````
 
##

#### Launch View Controller

 - Purpose is to minimize the code inside Appdelegate.
 - When the app starts it's the first controller loaded after splash and Appdelegate.
 - It's clone of splash screen with the logic.
 - Initialize all shared instances here.
 - Can be easy later on to have a app splash animation.


##

#### Project Folder Structure

##

#### Naming Conventions
