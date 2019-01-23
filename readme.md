# To clean the build environment
# from project root folder

cd android
gradlew clean

# To bundle js file
# from project root folder

react-native bundle --platform android --dev false --entry-file index.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res

# To build release apk
# from project root folder

cd android
./gradlew assemblerelease

# install release apk to device
# goto android sdk platform-tools folder

CD Users\chong\AppData\Local\Android\Sdk\platform-tools
adb install D:\workspace\yana002\android\app\build\outputs\apk\release\app-release.apk