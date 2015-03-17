# CircularProgressImageView

## Sample

![Circular Progress ImageView](https://github.com/TakumaMochizuki/CircularProgressImageView/blob/master/raw/newsample.gif)

## How to use

### 1. Dependencies
```gradle
	compile 'com.github.takumalee:CircularProgressImageView:1.0'
```

### 2. xml
```java
<com.takumalee.view.CircularProgressImageView
        android:id="@+id/cri"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:cpi_border_color="@android:color/holo_red_light"
        app:cpi_border_width="10dp"
        android:src="@mipmap/cat_takuma"/>
```

### 3. java

```java
CircularProgressImageView  cri = (CircularProgressImageView) findViewById(R.id.cri);

/**
* progress arrange need between 1 and 100
*/
cri.setProgress(progress);

```

### extend ImageView

Because base on ImageView, so you can use every ImageView method to set attributes.

e.g.

```java
imageView.setImageBitmap(bitmap);
imageView.setScaleType(ScaleType.CROP);
...

```

License
-------

    Copyright 2014 Henning Dodenhof
    Copyright 2015 TakumaLee

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.