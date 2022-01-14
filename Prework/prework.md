
# iOS Pre-work: Tip Calculator App

This pre-work incorporates the following required steps and 2 optional steps:

1. [Setup Xcode](#heading-1-setup-xcode)
1. [Familiarize yourself with Swift](#heading-2-familiarize-yourself-with-swift)
1. [Build the initial Tip Calculator](#heading-3-build-the-initial-tip-calculator)
1. [Submit your app for review](#heading-4-submit-on-the-application-dashboard)
1. [Common Errors](#heading-common-errors)
1. [Bonuses](#heading-bonuses)


## 1. Setup Xcode

<a href="https://itunes.apple.com/us/app/xcode/id497799835?mt=12#" target=blank> Download Xcode from the Mac App Store. </a>

**NOTE:* Membership in the iOS Developer Program is **not** required. This program costs $99 a year and is only required if you want to distribute your apps in the App Store and have access to beta iOS releases.

## 2. Familiarize yourself with Swift

There are a bunch of resources out there to learn Swift. We recommend taking a look at the following options:


* Apple's <a href="https://docs.swift.org/swift-book/GuidedTour/GuidedTour.html" target=blank> **Official Swift Guide** </a>.
<a href="" target=blank> </a>
* Download the <a href="https://docs.swift.org/swift-book/GuidedTour/GuidedTour.playground.zip" target=blank> **Swift 5 Playground** </a> to experiment with the Swift 5 syntax.
* You can also find more resources <a href="https://developer.apple.com/swift/resources/" target=blank> **here** </a>.


## 3. Build the initial Tip Calculator


### Let's begin developing! 

:::info
Expand the triangles below to collapse the tabs.
:::
 

<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 0: Setting up the Project 🏗 </summary>

* Make sure you have the latest version of Xcode installed.
*  Open Xcode and click "Create a new Xcode project".
*  Under the **"iOS"** Tab, click on **"App"**, then click "Next".
*  Set the Interface to "Storyboard"
*  Make sure you set up your project as shown in the gif below.
*  Choose a location to save the project. *We recommend saving the project on your Desktop*.

<img src='https://i.imgur.com/S3xoM2r.gif' title='Xcode Setup' alt='Xcode Setup' />

</details>

<br>

<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 1: Storyboard Layout 📱 </summary>

Drag 5 labels, 1 text field, and a segmented control bar from the Objects Libary. Drag them onto your View Controller in `Main.Storyboard`. See the gif below.

<img src='https://imgur.com/Yzmmb3E.gif' title='Objects Library' alt='Objects Library' />

Afterwards, check to see that your Tip Calculator storyboard elements looks like the image below.

<img src='https://imgur.com/idVTdtw.png' title='ViewController Layout' alt='ViewController Layout' height=500 />

We'll need to name and format the items on our Storyboard. This can be done in the  "Attributes Inspector" section, on the righthand side.

<img src='https://imgur.com/995vtYd.gif' title='Naming objects' alt='Naming objects' />

</details>

<br>


<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 2: Connecting Storyboard Elements to ViewController 🚠</summary>

To connect the objects to our code, you'll need to open the Assistant Editor.
*Note: There are a few ways to open it.*

**1. Press and hold the `alt/option` button on your keyboard and click the file you want to open in the Assitant Editor.**

**2. Click the "Add Editor" button on the right button, click the top folder icon and click the `ViewController.swift` file, as shown below.**

<img src='https://imgur.com/j7t7AHt.gif' title='Assistant Editor Add Editor' alt='Assistant Editor Add Editor' />

**3. Click on the "Adjust Editor" options button and click "Assistant".**

<img src='https://imgur.com/MBNonBD.gif' title='Assistant Editor Adjust Editor' alt='Assistant Editor Adjust Editor' />

We need to connect our items to our code in the `ViewController.swift` file. To connect the UI elements to your ViewController, press and hold the <kbd> control </kbd> key (also called control-dragging) from the item in the Storyboard and move the mourse cursor to the swift file under the `viewDidLoad()` function. See the gif below on control-dragging.

<img src='https://i.imgur.com/3m3AIE2.gif' title='Xcode Control Drag' alt='Xcode Control Drag' />

Do this for the following objects:

* Text Field (name it `billAmountTextField`)
* Label, next to the 'Tip Percentage' label (name it `tipAmountLabel`)
* Segmented Control (name it `tipControl`)
* Label, next to the 'Total' label (name it `totalLabel`)
* Action from segment control, under the `override func viewDidLoad()` function (name it `calculateTip`). Like this:
	<img src='https://i.imgur.com/xrY8tnq.gif' title='Xcode Layout' alt='Xcode Layout' />

#### Checking Your Outlets

Make sure that your outlets are connected to your view controller by making sure they look like this:

<img src='https://imgur.com/YNbfpr2.png' title='Xcode Layout' alt='Xcode Layout' />

Another way to check is through the Document Outline. 

Check to make sure each item is connected by right-clicking the 'Tip Calculator' view controller in the `Main.storyboard` file, as shown below.

<img src='https://imgur.com/cpdKVbS.png' title='Verifying Item Connections' alt='Verifying Item Connections' />


:::warning
**NOTE:** If you see any outlets with a warning (⚠️) sign next to it, **remove it and reconnect them correctly!**
:::

</details>

<br>

<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 3: Adding Logic to the App 🧠 </summary>

Now that everything is connected, we can begin coding.
In the `calculateTip` function, we need to do three things:

1. Get the initial bill amount and calculate the tips.
1. Calculate the total cost.
1. Update the tip and total labels.

Add the logic code to the function we created inside of the `caculateTip()`function:

<img src='https://imgur.com/KhtfW91.png' title='Calculate Tip' alt='Calculate Tip' />

You may notice that the tip and total don't display properly. To fix this, change the width of the tip percentage label and the total label.

After all this, go ahead and run your project and test it out on your desired iPhone simulator shown below:

<img src='https://imgur.com/1DD3mOj.png' title='Calculate Tip' alt='Calculate Tip' />


### ⚠️ Next Step: [Submit your Tip Calculator](#heading-4-submit-on-the-application-dashboard)

If your app works, push it to GitHub and record a gif of your working app. If you want to go above and beyond, try improving the UI and adding features. See below for some optional user stories.

###### Some ideas to improve the app are:

    - Create a tip slider that adjusts the tip percentage.
    - Make a tip splitting feature
    - A settings page to change the currency (based on global location) or the default tip


</details>

<br>



## 4. Submit on the application dashboard

<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 1: Create a GitHub Repository 📕 </summary>

1. <a href="https://courses.codepath.org/snippets/ios_university/github_desktop#1-heading-github-desktop" target=blank> <b> Create Repository, Commit, and Push using GitHub Desktop </b> </a>
	- ⚠️ <b> NOTE: </b> If you prefer using terminal, feel free to check out our guide on using <a href="https://guides.codepath.com/ios/Using-Git-with-Terminal" target=blank> <b> Git + Terminal </b> </a>
1. **Save and update** this <a href="https://courses.codepath.org/snippets/ios_university/readme_templates/prework_readme.md?raw=true" target=blank><b> Tip Calculator - README Template </b></a> in your project repository as a `README.md` file and push it to GitHub 
	<img src='https://i.imgur.com/2MEcW8P.gif' title='saving readme file' width='' alt='saving readme file' />
1. After making your first commit/push, double check that your repository is `public`
	- Go to your github.com dashboard, click on your prework project, select the settings tab and scroll all the way down
	- It should look something like this
		- <img src='https://i.imgur.com/LdJ4P5t.png' title='Public Repo' width='' alt='Public Repo' />
1. Create GIF of your project and add it to your `README.md`
	- <a href="https://hackmd.io/@codepath-tfs/record-gifs-quicktime" target=blank> Creating a Gif (using QuickTime) </a> – **Does NOT** require downloading tools
	- <a href="https://www.youtube.com/watch?v=8ELbIR67-cQ&list=PLrT2tZ9JRrf6oUda8qqSMwrJWn-SM-BQT&index=4" target=blank>Creating a Gif (using Recordit)</a> *2:15* – **Requires** downloading tool

:::warning

**GIF Recording Tools**

- <a href="http://recordit.co/" target=blank> Recordit </a>
- <a href="https://getkap.co/" target=blank> Kap </a>

:::


</details>

<br>


<details>
<summary style="font-size:1.25em; font-weight: 600"> Step 2: Submit through the application portal 🙌 </summary>

1. Head to the <a href="https://apply.codepath.org/dashboard" target=blank> application dashboard </a> and click the **SUBMIT** button in the *Pre-work Status* section. 
<img src="https://i.imgur.com/WzXvbgU.png" height=400 /><br>  

**NOTE:** If you can't find this section, try to log out of your GitHub, refresh the page, and then log back in.

1. Complete the submission form

- **Field 1:** Enter your Tip Calculator GitHub repo URL
- **Field 2:** Enter the URL of your App walkthrough gif
  - Example: `https://i.imgur.com/my_walkthrough.gif`
  	^ Make sure your GIF link ends with `.gif`, otherwise it won't work!
		^ You can test it in an *incognito/private mode* in your browser as well
- **Field 3:** Enter about how many hours you spent on the pre-work. (There is no right or wrong answer here)
- **Field 4:** Enter any additional info (optional).

1. Click the **Submit** button to submit your pre-work 👍

Congratulations on completing the required portion of the pre-work! The remaining steps are optional, but **completing them will significantly improve your chances of being accepted** into the class.

:::success
**🎉 Congratulations, you finished the tip calculator! 🎉**
:::


### Excellent Past Submissions 💯

Here are some examples of excellent past submissions. It only takes a couple hours to implement the basic version, but you should spend more time exploring the iOS framework.

- Examples with Animations

<img src='https://github.com/naeims/tipcalculator/raw/master/anim_tip_calculator.gif' title='img' width='200' alt='img' /> <img src='http://i.imgur.com/8Ra8d4j.gif' title='img' width='200' alt='img' /> <img src='https://github.com/peterbai/ios-tip-calculator/raw/master/gif/gif-currency-01.gif' title='img' width='200' alt='img' />

- Examples with Dark Mode Enabled

<img src='https://github.com/membriux/CodePath-iOS/raw/main/TipCalculator/walkthrough.gif' title='dark mode' width='200' alt='img'/>
<img src='https://i.imgur.com/vDUlI9p.gif' width='200' title='dark mode'/>

</details>

<br>

## Common Errors

<details>
<summary style="font-size:1.25em; font-weight: 600"> Error 1: GIF Not Showing 🙀</summary>

For the GIF to show, make sure that your link has the file extension at the end (.gif)

Here is an example URL of how it should look:
<a href="https://i.imgur.com/JL1snRo.gif" target=blank> https://i.imgur.com/JL1snRo.gif </a>

^^ *Notice* the ***.gif*** extension at the end

On your readme md file, the markdown should look like this:
`![](https://i.imgur.com/JL1snRo.gif)`

We recommend using these tools to help you record GIFs on your computer:

:::warning

**GIF Recording Tools**

- <a href="http://recordit.co/" target=blank> Recordit </a>
- <a href="https://getkap.co/" target=blank> Kap </a>

:::

</details>

<br>


<details>
<summary style="font-size:1.25em; font-weight: 600"> Error 2: GitHub Reference Error 🐙 </summary>

**ERROR: GitHub reference 'refs/heads/master' not found (-9)**

This problem has many solutions to it. Here a few links to help you fix it:

SOLUTIONS 

1. https://stackoverflow.com/questions/30809205/couldnt-set-refs-heads-master-when-commit
2. https://stackoverflow.com/questions/33262304/cannot-resolve-git-xcode-7-repository-issue-commit-fails-error-building-trees
3. https://github.com/desktop/desktop/issues/3838#issuecomment-359297523

If those solutions don't work, you can create another GitHub repo and simply copy/paste your project in that repo folder.

</details>

<br>



<details>
<summary style="font-size:1.25em; font-weight: 600"> Error 3: Any issue with Outlets 🔌</summary>

This is most likely an issue with your outlets. Go to the outlets menu on the storyboard and verify that your outlets are connected correctly.

This can be caused when you create and delete a current outlet and create a new one. 

The image below shows how an outlet is made correctly:

![](https://raw.githubusercontent.com/jonkykong/SideMenu/master/etc/Screenshot3.png)

The second image shows an outlet that was broken (the broken outlet is the one with a warning sign <img alt="warning" title="warning" src="/images/emoji/unicode/26a0.png"}" style="vertical-align:middle" width="20" height="20" /> next to it):

![](https://i.imgur.com/CjpWKIm.png)

</details>

<br>


## Bonuses!


<details>
<summary style="font-size:1.25em; font-weight: 600"> 1. Add a Settings Screen to the Tip Calculator ⚙️</summary>

Example Apps with settings screen: 

<img src='https://media.giphy.com/media/l580imUdTxyeKq8OaB/giphy.gif' width='200' title='img'/>
<img src='https://i.imgur.com/b51YqaJ.mp4' width='200' title'img'/>

### Enable Navigation between Screens

Now that we are adding a second screen to our app, we'll want to enable navigation from our first screen. We'll be using <a href="http://guides.codepath.org/ios/Using-Navigation-Controllers" target=blank> "push" navigation </a> to allow the user to go from the main tip screen to the settings screen.

The first step in enabling push navigation is to embed our tip ViewController inside of a UINavigationController. After opening `Main.storyboard` and selecting the `ViewController`, select `Editor => Embed In => Navigation Controller` from the Xcode menu. The steps are also shown in the following gif:

![](https://i.imgur.com/8w0jLlX.gif)

Next, we'll move on to creating the settings screen.

### Create a Settings View Controller

Every screen in your application is implemented by a view controller. A view controller has two parts: the designed part that's in the Storyboard and an Swift class that contains the code for that screen.

If a screen in the application doesn't require any code, then it can use the default UIViewController. However, as soon as you need to handle events like a user tapping on the screen, then you need to create a custom view controller for that screen.

1. For our settings screen, we need a custom view controller (`SettingsViewController`):

- Create the class (File -> New -> File -> Cocoa Touch Class) with the following options:

  <img src='https://i.imgur.com/ZRAM1Bk.png' title='SettingsVC' width='' alt='SettingsVC' />

- Then, use the "Object Library" to add a View Controller to the `Main.storyboard` and associate it with the `SettingsViewController` class:

    <img src='https://i.imgur.com/Vght24Z.gif' title='storyboard_settings_vc' width='' alt='storyboard_settings_vc' />


1. Now we need a button for the user to tap to open the settings screen:
  
- We'll do this by adding a button to the navigation bar:

	<img src='https://i.imgur.com/0gJ9OvP.gif' title='bar button settings' width='' alt='bar button settings' />

- Note: If you don't see the text "Tip Calculator" in your navigation bar, you can configure this in the `viewDidLoad` method of your Tip ViewController:

    ```swift
    override func viewDidLoad() {
        super.viewDidLoad()

        // Sets the title in the Navigation Bar
        self.title = "Tip Calculator"

        // ...
     }
       ```

- Let's go back to the `Main.storyboard` and check out our`BarButtonItem` called 'Settings'. Lets make this button take "segue" us to the `SettingsViewController` when we tap on it:

	<img src='https://i.imgur.com/dMpcSYt.gif' title='Segue to Settings' width='' alt='Segue to Settings' />


- **Note:** You'll need to ctrl-drag from the `BarButtonItem` to the `SettingsViewController` to create the show segue.

**Additional info:** In iOS, navigation stacks are one of the most common navigation mechanisms. You've seen it in many apps when you tap a button a new view slides in from the right. When you tap the back button, the previous view slides in from the left. A UINavigationController maintains the stack of view controllers and you can push new view controllers onto the stack. The back button is automatically added and tapping on the back button will pop the most recent view controller.

### Designing the Settings Screen

The purpose of the settings screen is to configure the default tip percentage. In the `SettingsViewController` we added to the Main Storyboard, design what you think the SettingsViewController should look like.

### Loading and Saving

There are several different ways to save data in iOS. The simplest to use is called <a href="http://guides.codepath.org/ios/UserDefaults" target=blank> UserDefaults </a>. UserDefaults allows you to save arbitrary keys and values and then retrieve these later from anywhere in your app.

Note the `synchronize` call. NSUserDefaults automatically and periodically synchronizes, but to manually flush the keys and values to disk, call [synchronize](https://developer.apple.com/library/ios/documentation/Cocoa/Reference/Foundation/Classes/NSUserDefaults_Class/#//apple_ref/occ/instm/NSUserDefaults/synchronize) to guarantee that your updates are saved.

For the Tip Calculator, you can save the new default tip percentage each time the user changes it on the settings screen.

### View Controller Lifecycle

When returning to the main `TipViewController` from the settings screen, it would be good to have the tip percentage reflect the new default value. One way to do that is load the tip percentage from UserDefaults whenever the view appears.

A view controller has a series of "lifecycle" methods that are called at various stages. When the view controller is initially set up, `viewDidLoad` is called. As it is shown `viewWillAppear` and `viewDidAppear` are called. As it is hidden `viewWillDisappear` and `viewDidDisappear` are called. The lifecycle methods are split into two methods (i.e. `viewWillAppear` and `viewDidAppear`) because sometimes you want some behavior to happen before the transition animation starts or after the transition animation ends.

In `TipViewController.swift`, try adding the following methods and watch the console output as you navigate into the settings view and back. Note the comment in `viewWillAppear` about retrieving the default tip percentage.

```swift
override func viewWillAppear(_ animated: Bool) {
    super.viewWillAppear(animated)
    print("view will appear")
    // This is a good place to retrieve the default tip percentage from UserDefaults
    // and use it to update the tip amount
}

override func viewDidAppear(_ animated: Bool) {
    super.viewDidAppear(animated)
    print("view did appear")
}

override func viewWillDisappear(_ animated: Bool) {
    super.viewWillDisappear(animated)
    print("view will disappear")
}

override func viewDidDisappear(_ animated: Bool) {
    super.viewDidAppear(animated)
    print("view did disappear")
}
```

### Animating View Properties (Optional)

<a href="http://guides.codepath.org/ios/Animating-View-Properties" target=blank> Animating view properties </a> is a great way to improve your UI. Many UIView properties can be animated, including frame, center, backgroundColor, alpha, transform, etc.

Be sure to include in the README an updated GIF walkthrough.

</details>

<br>

<details>
<summary style="font-size:1.25em; font-weight: 600"> 2. Extend your app, improve UI, add features 🎨 </summary>

Try your hand at implementing the following user stories and any other extensions of your own choosing:

- Remember the bill amount across app restarts. After an extended period of time, clear the state. This is a UI trick that Apple uses with the Spotlight app. If you return there a minute later, it will show your most recent search. if you return 10 minutes later, it defaults to blank. To implement this, plug into the application lifecycle and track time using NSDate.
- Use locale specific currency and currency thousands separator.
- Add a light/dark color theme to the settings view. In viewWillAppear, update views with the correct theme colors.
- Make sure the keyboard is always visible and the bill amount is always the first responder. This way the user doesn't have to tap anywhere to use this app. Just launch the app and start typing.
- Add animations to your UI
- The Tip calculator has a very primitive UI. Feel free to play with colors, layout, or even modify the UI to improve it.


</details>

<br>

# Still have questions about pre-work?

* If you encounter technical difficulties while submitting your work, please join our Pre-work Support Workspace **[here](https://go.codepath.org/preworkslack)**. 
  - This [workspace](https://go.codepath.org/preworkslack) is intended to support applicants with pre-work completion difficulties. 
  - Make sure to join and [create an account](https://go.codepath.org/preworkslack) with us to get assistance from our awesome team of tech experts and other students who may have encountered the same technical issues as yours!
