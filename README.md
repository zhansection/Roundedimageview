# RoundedImageView




## Gradle

Add the following to your `build.gradle` to use:
```
repositories {
    maven { url 'https://jitpack.io' }
}

dependencies {
    implementation 'com.zhanke:roundedimageview:1.0.1'
}
```


## Usage

Define in xml:

```xml
<com.zhanke.roundedimageview.RoundedImageView
        xmlns:app="http://schemas.android.com/apk/res-auto"
        android:id="@+id/imageView1"
        android:src="@drawable/photo1"
        android:scaleType="fitCenter"
        app:riv_corner_radius="30dip"
        app:riv_border_width="2dip"
        app:riv_border_color="#333333"
        app:riv_mutate_background="true"
        app:riv_tile_mode="repeat"
        app:riv_oval="true" />
```

Or in code:

```java
RoundedImageView riv = new RoundedImageView(context);
riv.setScaleType(ScaleType.CENTER_CROP);
riv.setCornerRadius((float) 10);
riv.setBorderWidth((float) 2);
riv.setBorderColor(Color.DKGRAY);
riv.mutateBackground(true);
riv.setImageDrawable(drawable);
riv.setBackground(backgroundDrawable);
riv.setOval(true);
riv.setTileModeX(Shader.TileMode.REPEAT);
riv.setTileModeY(Shader.TileMode.REPEAT);
```



## Thanks

see [thanks](https://github.com/vinc3m1/RoundedImageView/releases)




## License

    Copyright 2019 Vincent Mi
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
       http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
