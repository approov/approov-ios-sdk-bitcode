# Approov SDK
Bitcode enabled ApproovSDK binary release for iOS including podspec files.

Example Podfile:

```podfile
target 'YourTestApp' do
    use_frameworks!
    platform :ios
    pod 'approov-ios-sdk-bitcode', '3.0.0', :source => "https://github.com/approov/approov-ios-sdk-bitcode.git"
end
```

The native version of this library is located at https://github.com/approov/approov-ios-sdk

If you would like to add the Approov SDK as a binary dependency in your `swift package`, add this line to your `targets` section:

```swift
let releaseTAG = "3.0.0"
...
...
...
.binaryTarget(
            name: "Approov",
            url: "https://github.com/approov/approov-ios-sdk-bitcode/releases/download/" + releaseTAG + "/Approov.xcframework.zip",
            checksum : "ee9e432bca8060f109d00c04bbd28766dda6a38612d5056d737f54000e01f311"
        )


```
