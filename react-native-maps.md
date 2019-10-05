### Instruction
```
$ yarn add react-native-maps 
```
#### .env file
- Input key value on .env for putting key on build
```
GOOGLE_MAP_API_KEY=
```
#### (Android) AndroidManifest.xml
- Put meta tag inner application tags
```
<application>
  <!-- You will only need to add this meta-data tag, but make sure it's a child of application -->
      <meta-data
        android:name="com.google.android.geo.API_KEY"
        android:value="@string/GOOGLE_MAP_API_KEY"/>
</application>
```
#### (iOS) AppDelegate.m file
- If you use react-native-cofig and configuration setting is done, you can use it using ReactNativeConfig envFor function.
```
- (BOOL)application:(UIApplication *)application didFinishLaunchingWithOptions:(NSDictionary *)launchOptions
{
  NSString *gooleMapApiKey = [ReactNativeConfig envFor:@"GOOGLE_MAP_API_KEY"];
  
  [GMSServices provideAPIKey: gooleMapApiKey]; // add this line using the api key obtained from Google Console
```
