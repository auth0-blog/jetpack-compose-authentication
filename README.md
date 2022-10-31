# jetpack-compose-authentication
Completed project for the “Get Started with Jetpack Compose Authentication” article


## Project Description

This repository contains the completed version of the project featured in the Auth0 Developer Blog article _Get Started with Jetpack Compose Authentication_. The article walks the reader through the process of building a simple app using Jetpack Compose and adding Auth0 authentication to it.

The resulting app is simple, with two screens. The first is the “Logged out” screen, which appears when the app is launched:

![The app’s “Welcome” screen.](https://images.ctfassets.net/23aumh6u8s0i/79V4LEtvxB3v6SmVpFTJiv/6b3e9a97e35320bb7b23921786b624c5/welcome_screen.png)

Pressing the _Log in_ button starts the login process, which is handled by Auth0. The app delegates login to Auth0, which opens its web-based [Universal Login](https://auth0.com/docs/authenticate/login/auth0-universal-login) page, shown below:

![The default Auth0 Universal Login web page.](https://images.ctfassets.net/23aumh6u8s0i/1wO8fe8gEACROirEUKh0r9/6fea0a9aca8635b929abc273b26b2574/universal_login_-_emulator.png)

If the user provides valid login credentials, they are taken to the app’s “Logged in” screen:

![The app in its “logged in” state, with a title that reads “You’re logged in!”.](https://images.ctfassets.net/23aumh6u8s0i/5gNAhdJeDuRARnH8wTIVc5/aceaf6a3b65365ee9957d1cc47b5ac84/logged_in_screen.png)

This screen displays the following information gathered from the user’s profile:

* The user’s photo
The user’s name
* The user’s email address
* Tapping the _Log Out_ button logs the user out and returns them to the initial “Logged out” screen.


## Getting Started

### Prerequisities

You’ll need the following to build the app:

### 1. An Auth0 account

The app uses Auth0 to authenticate users, meaning you need an Auth0 account. You can <a href="https://auth0.com/signup" data-amp-replace="CLIENT_ID" data-amp-addparams="anonId=CLIENT_ID(cid-scope-cookie-fallback-name)">sign up for a free account</a>, which lets you add login/logout to 10 applications, with support for 7,000 users and unlimited logins — plenty for your prototyping, development, and testing needs.

### 2. An Android development setup

To develop applications for Android, make sure you have the following, in the order given below:

* Any computer running Linux, macOS, or Windows from 2013 or later with at least 8 GB RAM. When it comes to RAM, more is generally better.
* [**Java SE Developer Kit (JDK), version 11 or later.**](https://www.oracle.com/java/technologies/javase-jdk16-downloads.html) You can find out which version is on your computer by opening a command-line interface and entering `java --version`.
* [**Android Studio,**](https://developer.android.com/studio) version 2021.2.1 Patch 2 (also known as “Chipmunk”) or later. Jetpack Compose is a recent development, so you should use the most recent stable version of Android Studio.
* **At least one Android SDK (Software Development Kit) platform.** You can confirm that you have one (and install one if you don’t) in Android Studio. Open _Tools_ → _SDK Manager_. You’ll see a list of Android SDK platforms. Select the current SDK (**Android 12.0 (S)** at the time of writing), click the _Apply_ button, and click the _OK_ button in the confirmation dialog that appears. Wait for the SDK platform to install and click the _Finish_ button when installation is complete.
* **An Android device, real or virtual:**
	* **Using a real device:** Connect the device to your computer with a USB cable. Make sure that your device has Developer Options and USB debugging enabled.
	* **Using a virtual device:** Using Android Studio, you can build a virtual device (emulator) that runs on your computer. Here’s my recipe for a virtual device that simulates a current-model inexpensive Android phone:
		1. Open _Tools_ → _AVD Manager_ (AVD is short for “Android Virtual Device”). The _Your Virtual Devices_ window will appear. Click the _Create Virtual Device..._ button.
		2. The _Select Hardware_ window will appear. In the _Phone_ category, select _Pixel 3a_ and click the _Next_ button.
		3. The _System Image_ window will appear, and you’ll see a list of Android versions. Select _S_ (API 31, also known as Android 12.0). If you see a _Download_ link beside R, click it, wait for the OS to download, then click the _Finish_ button. Then click the _Next_ button.
		4. The _Android Virtual Device (AVD)_ window will appear. The _AVD Name_ field should contain _Pixel 3a API 31_, the two rows below it should have the titles _Pixel 3a_ (a reasonable “representative” phone, released three years ago at the time of writing) and _S_, and in the _Startup orientation_ section, _Portrait_ should be selected. Click the _Finish_ button.
		5. You will be back at the _Your Virtual Devices_ window. The list will now contain _Pixel 3a API 31_, and that device will be available to you when you run the app.


## Additional Reading

		
## License

The code in this repository is licensed under the Apache 2.0 License.