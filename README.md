# Approov Bitcode SDK

> **IMPORTANT:** Bitcode is no longer supported by Approov from the SDK 3.2.0 and above.

Bitcode enabled Approov SDK binary release for iOS including podspec files.

Example Podfile:

```podfile
target 'YourTestApp' do
    use_frameworks!
    platform :ios
    pod 'approov-ios-sdk-bitcode', '3.1.0', :source => "https://github.com/approov/approov-ios-sdk-bitcode.git"
end
```

The native version of this library is located at https://github.com/approov/approov-ios-sdk

If you would like to add the Approov SDK as a binary dependency in your `swift package`, add this line to your `targets` section:

```swift
let releaseTAG = "3.1.0"
...
...
...
.binaryTarget(
            name: "Approov",
            url: "https://github.com/approov/approov-ios-sdk-bitcode/releases/download/" + releaseTAG + "/Approov.xcframework.zip",
            checksum : "b1c17d399cc6491ace55833b23378f740439c36bc90afeea3351a76d6839c94e"
        )


```
