VATCH - Android app + home-screen widget

BUILD THE APK WITHOUT ANDROID STUDIO
1. Create a free account at github.com and make a new repository.
2. Upload everything from this folder (including the hidden .github folder).
3. Open the Actions tab and run "Build Vatch APK".
4. After about 5 minutes, open the finished run and download "Vatch-apk".
5. Unzip it and copy app-debug.apk to your phone. Allow "install unknown apps", then open it.

ADD THE WIDGET
Long-press the home screen > Widgets > Vatch. Drag it onto the home screen.
The widget shows hour and minute hands and updates every minute.
(Android does not allow a moving second hand in widgets.)
On Android 12+, if the widget is a minute or two late, allow
Settings > Apps > Vatch > Alarms & reminders.

FULL-SCREEN APP
The status and navigation bars are hidden and the screen stays on.
Tap the watch to hide or show the controls. Swipe from the screen edge to see the system bars.

WITH ANDROID STUDIO
npm install
npx cap sync android
npx cap open android
Build > Build APK(s)

FILES
www/index.html                                   the watch (edit, then run: npx cap sync android)
android/app/src/main/java/com/vatch/app/         MainActivity.java (full screen), VatchWidget.java (widget)
