### Instruction
```
$ yarn add react-native-maps 
```

#### (iOS) AppDelegate.m file
- If you use react-native-cofig and configuration setting is done, you can use it using ReactNativeConfig envFor function.
```
- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions
{
  NSString *gooleMapApiKey = [ReactNativeConfig envFor:@"GOOGLE_MAP_API_KEY"];
  
  [GMSServices provideAPIKey: gooleMapApiKey]; // add this line using the api key obtained from Google Console
```
