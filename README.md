SwipeBack [![Build Status](https://travis-ci.org/liuguangqiang/SwipeBack.png?branch=master)](https://travis-ci.org/liuguangqiang/SwipeBack)
===========

## Origin [SwipeBack](https://github.com/liuguangqiang/SwipeBack)

SwipeBack is a android library that can finish a activity by using gesture.

Added DragDirectMode. You can set DragDirectMode to change the swipe direction.
```
public enum DragDirectMode {
   EDGE,
   VERTICAL,
   HORIZONTAL
}
```
##Usage

###Gradle
```
allprojects {
	repositories {
		maven { url 'https://jitpack.io' }
	}
}
```
```
dependencies {
   	compile 'com.github.pavel163:SwipeBack:1.0.0'
}
```

###SwipeBackActivity
SwipeBackActivity is a base activity for using this library more easier.This Activity will help us to show a shadow.

```
public class CommonActivity extends SwipeBackActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_common);
        setDragDirectMode(SwipeBackLayout.DragDirectMode.VERTICAL);
    }

}
```


