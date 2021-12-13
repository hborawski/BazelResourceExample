# BazelResourceExample

This repository is a small example that illustrates a problem bundling resources into an iOS application with `ios_application` rule from https://github.com/bazel-ios/rules_ios



## Running

### Xcode

Open the `BazelResourceExample.xcodeproj` in Xcode, and run the app. This will open the application to the `Main.storyboard` which has a Label and an Image. The image is loaded from `Assets.xcassets`, and should show the Bazel logo.

### Bazel

From the command line, run `./bazelisk run //:BazelResourceExample --apple_platform_type=ios`

The application will launch, and only the UILabel will be visible, along with a console message:

```sh
BazelResourceExample[52984:2749012] Could not load the "bazel" image referenced from a nib in the bundle with identifier "com.example.BazelResourceExample"
```

