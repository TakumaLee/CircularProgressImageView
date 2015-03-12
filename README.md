# CircularProgressImageView

## Sample

![Circular Progress ImageView](https://github.com/TakumaMochizuki/CircularProgressImageView/blob/master/raw/newsample.gif)

## How to use

### xml
```java
<com.takumalee.view.CircularProgressImageView
        android:id="@+id/cri"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:cpi_border_color="@android:color/holo_red_light"
        app:cpi_border_width="10dp"
        android:src="@mipmap/cat_takuma"/>
```

### java

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