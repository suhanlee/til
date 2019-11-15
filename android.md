# Get APK Key hash
```
$ keytool -list -printcert -jarfile ./android/app/build/outputs/apk/release/app-release.apk | grep "SHA1: " | cut -d " " -f 3 | xxd -r -p | openssl base64
```
# Get key hash from key stores
```
$ keytool -exportcert -alias kyle -keystore ./android/app/ksytore/ReleaseKeyStore | openssl sha1 -binary | openssl base64
```
