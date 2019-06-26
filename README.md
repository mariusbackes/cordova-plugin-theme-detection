# Cordova plugin for theme detection

## Description

This plugin detects whether the dark mode is enabled on the device or not.

**Attention**: Dark mode was introduced in iOS 13, which is still in beta.
This plugin refers to the iOS 13 SDK and is at this point not for production use.

## Installation

Add the plugin with the following command:

`cordova plugin add cordova-plugin-theme-detection`

## Usage

```js
cordova.plugins.ThemeDetection.methodName(
  [parameter],
  function(success) {
    console.log(success);
  },
  function(error) {
    console.log(error);
  }
);
```

#### Ionic Native

A wrapper for Ionic Native will be available soon!

### Methods

#### isAvailable

`cordova.plugins.ThemeDetection.isAvailable()`

Checks whether the device is running on iOS 13 or newer and returns an object with a boolean value and a message.

#### isDarkModeEnabled

`cordova.plugins.ThemeDetection.isDarkModeEnabled()`

Checks whether the dark mode is enabled on device and returns an object with a boolean value and a message.

### Responses

**ThemeDetectionResponse**:

```js
ThemeDetectionResponse {
    value: boolean;
    message: string;
}
```

## Changelog

- 1.0.0: Initial version support for iOS.
