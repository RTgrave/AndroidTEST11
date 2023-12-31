# Integrating Mediated Networks

This README includes instructions for integrating MAX mediation network adapters in your UE4 app.

## Requirements

- CocoaPods
- Python 3.6+

## Instructions

1. [Create a Podfile](https://dash.applovin.com/documentation/mediation/ios/mediation-adapters) for the adapters you want to integrate. This file should be in the same directory as the `install_adapters.py` script.
2. Run `install_adapters.py` to download the adapters.
3. Copy the build rules generated by `install_adapters.py` into `AppLovinMAX.Build.cs`.
4. Follow the instructions for ["Preparing Mediated Networks"](https://dash.applovin.com/documentation/mediation/manual-integration-ios"). Add any necessary changes to `Info.plist` in `AppLovinMAX_UPL_IOS.xml`.
5. Download the third-party SDKs required by each installed adapter and create a corresponding `*.embeddedframework.zip` file in the directory `ThirdParty/IOS`.
6. Add iOS build rules for any third-party dependencies to `AppLovinMAX.Build.cs`.

