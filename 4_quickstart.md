---
layout: page
title: Quick Start
permalink: /quick-start
nav_order: 5
has_children: false
---

Quick Start
===========


(1) Start the backend
----------------
[Readme](https://github.com/opencircular/opencircular/blob/master/src/server/services/readme.md)
1. Open the `backend.code-workspace` or `cd src/server/services`
2. `npm i`
3. Read these instructions and install all the dependencies [Readme](https://github.com/opencircular/opencircular/blob/master/src/server/services/readme.md)
4. Open a new terminal tab and run dapr `npm run dapr`
5. Wait a few seconds then `npm run start`
6. Wait for the gateway to start. you should see this message 
```
🚀 Gateway ready at http://localhost:3999/graphql`.
```
  - *NOTE It takes about 10 seconds to load while it launches a few services on different ports and the gateway. It uses nodemon to monitor changes file changes. It uses Docker containers to run Dapr Microservices for pub/sub/stateful/redis/service invoke/gRPC
7. If you are debugging you can attach the vscode debugger 

```
debug tab in vsode > choose `Debug PlastiCoin (services)` > green play button
```
http://localhost:3999/graphql - This should boot the GraphQL explorer (gateway.ts) and you need a token to query the api see [GraphQL Explorer docs](#GraphQL-Explorer)

(2) Start the Blockchain
------------------
[Readme](https://github.com/opencircular/opencircular/blob/master/src/blockchain/hyperledger/readme.md)
1. Open the `blockchain.code-workspace`
2. Make sure you have Docker-desktop, Minifab and all the dependencies installed [instructions here](https://github.com/opencircular/opencircular/blob/master/src/blockchain/hyperledger/readme.md#1-prereq---install-minifabric)
3. Initialize and start the network in Docker [instructions here](https://github.com/opencircular/opencircular/blob/master/src/blockchain/hyperledger/readme.md#2-initialize-the-network-via-docker)
4. Start the gateway (debug/live reload) 
    - To start the application/backend/gateway.js you can simply goto debug in vscode and click `debug > "Docker Launch Debugging"`. 
5. Later on, if the images are still in docker you can start the network with the `npm run netup` and `npm run netdown` commands

(3) Start the Front End
------------------
[Readme](https://github.com/opencircular/opencircular/blob/master/src/client/react-native/readme.md)
#### Android

1. Open the `frontend.code-workspace` or `cd src/client/react-native`
2. `npm i`
3. Install the dependencies and copy the .env files as documented [here](https://github.com/opencircular/opencircular/blob/master/src/client/react-native/readme.md#install-frontend-dependencies)
3. make sure an emulator is running or preferably a device is plugged
4. If this is the first time running I recommend opening the android project in android studio 
to let gradle index and build automatically. Thereafter, you should be able to simply `npm run android` without android studio.
    - `src/client/react-native/android`
5. `npm run android` (make sure this runs jetifier, newer versions of react-native do!)
6. In a new tab watch for typescipt errors `npm run watch`


#### iOS

1. `cd src/client/react-native`
2. `npm i`
3. `cd ios && pod install && cd ..` 
4. Open the ios project with xcode
  - `open ./ios/plasticoin.xcworkspace`
5. make sure your mac has a developer certificate with an Apple developer account. Here is a good resource on how to do this: https://ionicframework.com/docs/appflow/package/credentials#ios-setup
6. Configure your apple developer cert. This is to ensure you have the provisioning profile that links your ios phone to your develoepr cert to the app ID com.dow.plasticoin. It should look similar to this:
![Image](./assets/images/ios-cert-config.png)
7. If you are using Azure AD (defualt config does not use this..so you can skip) you must fix an Auth package, as noted here: https://github.com/FormidableLabs/react-native-app-auth/issues/296#issuecomment-525400686
    - Make sure the pod files are installed for the package AppAuth `pod install`
    - Open this file `src/ios/Pods/AppAuth/Source/OIDAuthorizationService.m`
    - Comment out this block of code on line 124
    ```js
      // rejects URLs that don't match redirect (these may be completely unrelated to the authorization)
      // if (![self shouldHandleURL:URL]) {
      //  return NO;
      // }
    ```
7. Run the app on the simulator
    - you might need to clean the project `Product > clean build folder`