[SqLite]:[https://github.com/stephencelis/SQLite.swift]
[member_center]:[https://developer.apple.com/membercenter/index.action]

# Flourish 

This repository contains all fo the code to build Flourish, a secure mood journal
built in Swift for iOS devices. This souce code is meant to accompany the step-by-step
tutorial.   

## How to run Flourish in Xcode

Install SQLite:

1. Download or clone this repository to your computer 
2. Download or clone the [SQLite Project][SQLite] repository to your computer
3. Open the Flourish.xcworkspace file in the Flourish Repository using Xcode
3. In the SQLite][SQLite] documentation, find the Installation ection and follow the steps
to install SQLite into your Flourish xcode project 

To test out the iCloud saving function in Flourish, you must enable iCloud in your 
xcode project: 

1. Make sure you have a developer account tied to your Xcode project. Go to Xcode 
> Prefrences > Accounts and hit the plus (+) sign to add an Apple ID. 
2. In the Identity section of your App target’s General pane, make sure there is
a developer account selected in the "Team" dropdown menu. 
3. Visit the [Apple Developer Member Center][member_center] and click on Certificates,
Identifiers, and Profiles
4. On the next page, click Identifiers. 
5. Next, select AppIDs from the Identifiers menu and click the plus sign (+) to 
create a new AppID.
6. Under AppID suffix section, select Explicit App ID and enter a Bundle ID that matches 
the Bundle Identifier in the indentity tab in your Flourish.xcodeproj's Identity section. 
7. Under the App Services section, select the iCloud checkbox under the Enable Services menu.
This will bring up two radio buttons. Select "Include CloudKit support 
(requires Xcode 6)". 
8. Hit the Continue button to finish creating your AppID. 
9. Go to the Capablities section of your App Target's General pane and toggle on
the iCloud settings
![iCloud_Pane](https://developer.apple.com/library/ios/documentation/IDEs/Conceptual/AppDistributionGuide/Art/4_enableicloud_2x.png)
10. Under the iCloud dropdown menu in the Capabilities section, select the Key-value 
storage checkbox and the CloudKit checkbox in the services section. 
11. Right below the services section, select "Specify custom containers" in the 
containers section. You might have to hit the refresh button for Xcode to pull
your App ID from your developer account. 
12. If there are any errors, hit the "fix errors" button below the services and 
containers sections of the iCloud dropdown. 



