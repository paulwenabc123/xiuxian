修仙傳 Android 專案
====================
遊戲本體：app/src/main/assets/index.html
App 名稱：app/src/main/res/values/strings.xml
App 圖示：app/src/main/res/mipmap-*/ic_launcher.png
版本號：app/build.gradle.kts 裡的 versionCode / versionName

方法一：Android Studio → File > Open 選這個資料夾 → 等同步完成 →
        Build > Build App Bundle(s) / APK(s) > Build APK(s)
        APK 位置：app/build/outputs/apk/debug/app-debug.apk

方法二：上傳到 GitHub，Actions 會自動產生 APK（見 .github/workflows/build-apk.yml）

更新遊戲：用新的 index.html 取代 app/src/main/assets/index.html，
         並把 versionCode 加 1，再重新 Build。
