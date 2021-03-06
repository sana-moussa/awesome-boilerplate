# awesome boilerplate - WIKI -

## Internal
This is a private wiki used as a reference for developers.
<!--Here you can write all specific commands and notes that you need to share with all committers of this project-->

### Links
* Staging system
* Live system

### Credentials
<!--access credentials-->
* For  test users/ each existing Role

### Notes
<!--internal notes to developers-->

### Important Commands to run
<!--Important Commands to run with a short description of the context-->
ther very important one is :
```bash
npm install
```
### Contacts
<!--How to contact the responsible person for this project -->

## Translations
<!--Where are the translation documents and how to generate translation files-->
### links
### commands

## Mobile Env Setup
<!--All about mobile env: certificates, SDK, special config...-->

## Mobile Build
<!--Notes on how to build the app -->
## Running on iOS Simulator

_Note_: You must be on a Mac for this.

- Be sure your Meteor app is running: In the ```MeteorApp``` directory, type ```meteor```

You've got a few ways you can run the app for iOS:

- From the `MobileApp` directory run `react-native run-ios`

## Running on iOS Device

_Note_: You must be on a Mac for this.

- Be sure your Meteor app is running: In the ```MeteorApp``` directory, type ```meteor```
- Get the IP address of your machine (you can run `ipconfig getifaddr en1` to do so)
- In `MobileApp/app/config/settings.js` change `localhost` to your machine's IP address
- Plug your device into your computer (make sure it's on the same network)
- Open the project in Xcode
- Select your device in Xcode and press "Build and run"

For further information please reference the [official docs](https://facebook.github.io/react-native/docs/running-on-device-ios.html#content).

## Running on Android Simulator

- Be sure your Meteor app is running: In the ```MeteorApp``` directory, type ```meteor```
- Get the IP address of your machine
- In `MobileApp/app/config/settings.js` change `localhost` to your machine's IP address
- Make sure you have an emulator configured and running.
- From the `MobileApp` directory run `react-native run-android`

On OSX you can get your IP address by running `ipconfig getifaddr en1` in a terminal window.

On linux running `ifconfig` will get you a list of your network interfaces along with their IP addresses. For the stock Google simulator you will want to use the IP of your active network connection (probably `eth0` or `wlan0`). If you are using the Genymotion simulator, it runs in a Virtual Box VM with a Host-only network interface. You will want to use the IP address of this network which may look like vboxnet0 under ifconfig.

## Running on Android Device

- Be sure your Meteor app is running: In the ```MeteorApp``` directory, type ```meteor```
- Make sure [USB Debugging is enabled](https://facebook.github.io/react-native/docs/running-on-device-android.html#prerequisite-usb-debugging)
- Plug your device into your computer
- Run `adb devices` to make sure your device shows up
- Run `adb reverse tcp:8081 tcp:8081`
- In `MobileApp/app/config/settings.js` change `localhost` in `METEOR_URL` to your computer's IP address (see note in "Running on Android" section on how to get your IP Address)
- Run `react-native run-android`

