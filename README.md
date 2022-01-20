# Android
## important native code 

### Viewbinding 

This is to avoid findviewbyID. Viewbinding makes accessing view elements move easier and clearer. 

Add the code below to the module level build.gradle

```
  android {
    ...
    buildFeatures {
        viewBinding true
    }
  }
```

> HELP: [ViewBinding by Android](https://developer.android.com/topic/libraries/view-binding)

### Navigation Graph 
This is so you you get to use fragments instead of activities which are used for much more heavier work 
Navigation graphs also indicate how your app moves through the screens


### Navigate from Activity to Activity 
This code will prevent the backbutton pressed function to close the app
```
  Intent i = new Intent(getApplicationContext(), LoginActivity.class);
  startActivity(i);
  finish();
```
