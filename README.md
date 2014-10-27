ionic-typescript-definitions
============================

Typescript definitions for Ionic framework (http://ionicframework.com/)


ionic.d.ts is the main file with the main APIs of the Ionic framework defined.

cordova.d.ts is for who need to use the ionic keyboard plugin (https://github.com/driftyco/ionic-plugins-keyboard)


HOW TO USE:

The files declare a global objec 'ionic', so it is possible to call the global ionic APIs (http://ionicframework.com/docs/api/), like ionic.Platform, ionic.DomUtil or ionic.EventController.

There are also interfaces for all the delegates of the framework.

Example of using the ionic services and delegates inside a controller:

myNgModule.controller('TestCtrl', function ($scope, $ionicPopup: Ionic.IPopup, $ionicActionSheet: Ionic.IActionSheet) {
  $ionicPopup.alert(...);
  $ionicActionSheet.show(...);
}
