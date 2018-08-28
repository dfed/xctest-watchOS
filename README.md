# XCTest-watchOS

[![Carthage Compatibility](https://img.shields.io/badge/carthage-✓-e2c245.svg)](https://github.com/Carthage/Carthage/)
[![Version](https://img.shields.io/cocoapods/v/XCTest-watchOS.svg)](http://cocoadocs.org/docsets/XCTest-watchOS)
[![License](https://img.shields.io/cocoapods/l/XCTest-watchOS.svg)](http://cocoadocs.org/docsets/XCTest-watchOS)
[![Platform](https://img.shields.io/cocoapods/p/XCTest-watchOS.svg)](http://cocoadocs.org/docsets/XCTest-watchOS)

XCTest-watchOS provides an implementation of XCTest that can run on watchOS. XCTest-watchOS allows you to run your library’s existing `XCTest` suite on watchOS with minimal effort.

## Getting Started

1. Create a new watchOS app
1. Include your test files in your new watchOS app
1. Install XCTest-watchOS, and link the included XCTest framework from your new watchOS app
1. Call `XCTestCase.runAllTests()` from `applicationDidFinishLaunching` in your `WKExtensionDelegate` implementation in your new watchOS app
1. Run your new watchOS app, and see if your tests succeed

### CocoaPods

Install with [CocoaPods](http://cocoapods.org) by adding the following to your `Podfile`:

```
platform :watchos, '2.0'
use_frameworks!
pod 'XCTest-watchOS'
```

### Carthage

Install with [Carthage](https://github.com/Carthage/Carthage) by adding the following to your `Cartfile`:

```ogdl
github "dfed/XCTest-watchOS"
```

Run `carthage` to build the framework and drag the built `XCTest.framework` into your Xcode project.

### Swift Package Manager

Install with [Swift Package Manager](https://github.com/apple/swift-package-manager) by adding the following to your `Package.swift`:

```swift
dependencies: [
    .package(url: "https://github.com/dfed/XCTest-watchOS", from: "0.0.1"),
],
```

### Submodules

Or manually checkout the submodule with `git submodule add git@github.com:dfed/XCTest-watchOS.git`, drag XCTest.xcodeproj to your project, and add XCTest as a build dependency of your watch app.

## Requirements

* Xcode 9.0 or later.
* watchOS 2 or later.