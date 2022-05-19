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
