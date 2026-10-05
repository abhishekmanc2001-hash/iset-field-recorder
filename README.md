# iSET Field Recorder - APK build

## Easiest: build in the cloud (no Android Studio)
1. Create a free GitHub account and a new repository.
2. Upload ALL files of this folder (keep the .github folder).
3. Open the repo > Actions tab > "Build APK" > wait ~5 minutes.
4. Open the finished run > Artifacts > download iSET-Field-Recorder-APK.
5. Unzip, send app-debug.apk to the phone (WhatsApp/USB), tap to install
   (allow "install unknown apps").

## Or build locally (Node 20 + Android Studio)
npm install
npx cap add android
npx cap sync android
npx cap open android   -> Build > Build APK(s)

The app is bundled inside the APK, so it opens with no internet.
To change the app, edit www/index.html and rebuild.
