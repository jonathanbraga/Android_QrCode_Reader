## Settings

* NuGet Packages
  - Xamarin.GooglePlayServices.Vision
  - Xamarin.Android.Support.V4.AppCompat
  - Xamarin.Android.Support.V7.AppCompat

* AndroidManifest

```
  <uses-permission android:name="android.permission.CAMERA"/>
  <uses-permission android:name="android.permission.VIBRATE"/>
  
  <uses-sdk android:minSdkVersion="16" />
  <application android:allowBackup="true" android:label="@string/app_name">

    <meta-data android:name="com.google.android.gms.vision.DEPENDENCIES"
               android:value="barcode"/>
    
  </application>
```

* AssemblyInfo

```
[assembly: UsesPermission(Android.Manifest.Permission.Camera)]
```
