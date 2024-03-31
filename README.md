# swift-mdk
libmdk swift binding

## Swift Package
<del>Must download [sdk](https://sourceforge.net/projects/mdk-sdk/files/nightly/mdk-sdk-apple.tar.xz/download) and extract to package dir</del>

## CocoaPods
Add
```ruby
pod 'swift-mdk'
```
in Podfile. Add

```swift
import swift_mdk
```
in your code

Projects created by XCode 15+ may failed with sandbox rsync error
```
Sandbox: rsync.samba(78689) deny(1) file-read-data /Users/wangbin/Library/Developer/Xcode/DerivedData/....

```

 then set change `ENABLE_USER_SCRIPT_SANDBOXING = YES` to `ENABLE_USER_SCRIPT_SANDBOXING = NO` in project.pbxproj, or set `User Script Sandboxing` to `NO` in xcode project `Build Settings`