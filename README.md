# Indy.Framework

This repository contains a pre-built framework of the
[indy-sdk](https://github.com/hyperledger/indy-sdk). This has to be done as the
official build pipeline is broken, and this makes sure everyone can still access
the library for React Native or iOS development.

> This has only been tested for React Native and might not work the same as for
> a normal iOS mobile application.
> The framework is also not compatible with simulators. Please use a real device
> for development.

### Installation

This installation is not anything special next to moving the
`Indy.Framework` folder to a specific directory in your project.

```bash
git clone https://github.com/animo/Indy.Framework
cd Indy.Framework
mv Indy.Framework <PROJECT_DIRECTORY>/ios/Pods/Frameworks/
```

Additionally, you need to ensure the following:

- `ENABLE_BITCODE` is set to false
- `Indy.Framework` is added to the project as embedded content

You can set both in XCode.app by navigating to your project settings. `ENABLE_BITCODE` should be disabled by default.
Under the `General` tab in settings you can find `Frameworks, Libraries, and Embedded Content`. Click `+` to open the file selector and add `Indy.Framework` from your Pods.

NOTE: For these steps to work with a react native projects do _not_ follow the instructions in the [indy-sdk repo](https://github.com/hyperledger/indy-sdk) unless you know what you are doing or have some customised setup.
