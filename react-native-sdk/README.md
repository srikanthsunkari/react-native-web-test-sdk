# react-native-sdk

## Getting started
1. Copy this library in your project root
2. Run the command `$ npm install ./react-native-sdk`
3. Run `react-native link react-native-sdk`

#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `react-native-sdk` and add `RNSDK.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libRNSDK.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Run your project (`Cmd+R`)<

#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.reactlibrary.RNSDKPackage;` to the imports at the top of the file
  - Add `new RNSDKPackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-sdk'
  	project(':react-native-sdk').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-sdk/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-sdk')
  	```

## Usage
```javascript

  