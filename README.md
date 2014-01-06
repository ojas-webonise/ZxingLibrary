ZxingLibrary
============

Zxing barcode scanner library

##How to integreate

Add required permissions in manifest file

  <uses-permission android:name="android.permission.CAMERA"/>
  <uses-feature android:name="android.hardware.camera"/>

Add following activity declarations to manifest

  <activity 
    android:name="com.google.zxing.client.android.CaptureActivity" 
    android:configChanges="orientation|keyboardHidden" 
    android:screenOrientation="portrait" 
    android:theme="@android:style/Theme.NoTitleBar.Fullscreen"
    android:windowSoftInputMode="stateAlwaysHidden"/>
    
    <activity 
      android:name="com.google.zxing.client.android.encode.EncodeActivity">
      <intent-filter>
        <action android:name="com.google.zxing.client.android.ENCODE"/>
        <category android:name="android.intent.category.DEFAULT"/>
      </intent-filter>
    </activity>
