# SplashDemo

####An example of a splash screen with animations on Android

####带平移动画效果的Android Splash Demo
在界面上解决了两个问题

1.解决了白屏黑屏闪屏的问题
```
    <style name="SplashTheme" parent="Theme.AppCompat.NoActionBar">
        <item name="android:windowBackground">@drawable/cat</item>
        <item name="android:windowFullscreen">true</item>
        <item name="android:windowIsTranslucent">true</item>
```

2.解决了从全屏到非全屏模式下的ActionBar滑动问题
```
    // 防止从全屏到非全屏模式的ActionBar滑动
    SplashActivity.this.getWindow().setFlags(WindowManager.LayoutParams.FLAG_FORCE_NOT_FULLSCREEN,
        WindowManager.LayoutParams.FLAG_FORCE_NOT_FULLSCREEN);
```

####效果：
![](https://github.com/linpeiyou/SplashDemo/blob/master/app/src/main/res/drawable/Splash.gif)
