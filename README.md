# Proguard removes `Object#wait()`!

The following proguard settings removes `Object#wait()` because `<methods>` seems to
include all the inherited methods.

```
-assumenosideeffects class android.util.Log { <methods>; }
```

It sucks. Really.

