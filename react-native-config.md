#### Install 
```
$ yarn add react-native-config
```

#### Linking
```
$ react-native link react-native-config
```
#### TroubleShooting

##### If ReactNativeConfig.h file not found
- You need to put search path, react-native-config header file directory
like `$(SRCROOT)/../node_modules/react-native-config/ios/ReactNativeConfig`
- Directory path maybe chagned. So I fork that library, you can use it
https://github.com/suhanlee/react-native-config on package.json 

```
    "react-native-config": "git+https://github.com/suhanlee/react-native-config.git",
```
