# Approov SDK
Bitcode enabled ApproovSDK binary release for iOS including podspec files.

Example Podfile:

```podfile
target 'YourTestApp' do
    use_frameworks!
    platform :ios
    pod 'approov-ios-sdk-bitcode', '2.9.0', :source => "https://github.com/approov/approov-ios-sdk-bitcode.git"
end
```

The native version of this library is located at https://github.com/approov/approov-ios-sdk

If you would like to add the Approov SDK as a binary dependency in your `swift package`, add this line to your `targets` section:

```swift
let releaseTAG = "2.9.0"
...
...
...
.binaryTarget(
            name: "Approov",
            url: "https://github.com/approov/approov-ios-sdk-bitcode/releases/download/" + releaseTAG + "/Approov.xcframework.zip",
            checksum : "535cb7b12aa878d6abca175010adaa36a1acb3eebfb5d096a03b2630404f7569"
        )


```
