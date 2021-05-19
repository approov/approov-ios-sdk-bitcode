# Approov SDK
Bitcode enabled ApproovSDK binary release for iOS including podspec files.

Example Podfile:

```podfile
target 'YourTestApp' do
    use_frameworks
    platform :ios
    pod 'approov-ios-sdk-bitcode', '2.7.0', :source => "https://github.com/approov/approov-ios-sdk-bitcode.git"
end
```

The native version of this library is located at https://github.com/approov/approov-ios-sdk

If you would like to add the Approov SDK as a binary dependency in your `swift package`, add this line to your `targets` section:

```swift
let releaseTAG = "2.7.0"
...
...
...
.binaryTarget(
            name: "Approov",
            url: "https://github.com/approov/approov-ios-sdk-bitcode/releases/download/" + releaseTAG + "/Approov.xcframework.zip",
            checksum : "c1d1e213711b050c82a39c4de6cc62ffe550d26dac95ee6f854a3a4b54b8b3f3"
        )


```