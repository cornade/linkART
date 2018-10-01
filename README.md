## How to link ART library to your react native project.

First of all, be sure your project was inited with `react-native init` command, because you'll need to handle staffs with source code with `XCode`.

### For Android Platform
Congradulations you guy, the ART library was linkd default in android platform, so you don not need doing anything.

### For iOS Platform

if you are using CocoaPod:

```bash
pod 'React', path: '../node_modules/react-native', subspecs: [
  'ART',
]
```

or you can handle this manually:


1. Drag  `ART.xcodeproj` (`working_directory/node_modules/react-native/Libraries/ART/ART.xcodeproj`) to the **Libraries** group in XCode.

2. Add `libART.a` to **Link Binary With Libraries**

