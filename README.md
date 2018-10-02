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

![Link](https://i.postimg.cc/0yRHfB8Y/link.png)

2. Add `libART.a` to **Link Binary With Libraries**

![](https://i.postimg.cc/v8KK1mkS/Screen_Shot_2018-10-02_at_12.17.27_AM.png)
![](https://i.postimg.cc/dtTxGYKQ/Screen_Shot_2018-10-02_at_12.18.11_AM.png)

