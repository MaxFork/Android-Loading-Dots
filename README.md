# Android-Loading-Dots

A library which allows you to have some beautiful loading with dots, 
for both Java and Kotlin in XML, 
If you need **Jetpack Compose** version of this library then click [here](https://github.com/razaghimahdi/Compose-Loading-Dots)

## Developed by Mahdi Razzaghi Ghaleh

[![](https://jitpack.io/v/razaghimahdi/Android-Loading-Dots.svg)](https://jitpack.io/#razaghimahdi/Android-Loading-Dots)

## Step 1. Add it in your root build.gradle at the end of repositories:

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}

## Step 2. Add the dependency

	dependencies {
	        implementation 'com.github.razaghimahdi:Android-Loading-Dots:1.3.0'
	}

## Step 3. How to use

XML:

```xml
            <com.razzaghimahdi78.dotsloading.linear.LoadingWavy
            android:id="@+id/loadingWavy"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            app:dots_color="@color/colorPrimaryDark"
            app:dots_count="3"
            app:dots_duration="500"
            app:dots_size="medium" />
            
            <com.razzaghimahdi78.dotsloading.linear.LoadingFady
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            app:dots_color="@color/colorPrimaryDark"
            app:dots_count="3"
            app:dots_duration="500"
            app:dots_size="medium" />
            
            <com.razzaghimahdi78.dotsloading.linear.LoadingBiggy
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            app:dots_color="@color/colorPrimaryDark"
            app:dots_count="3"
            app:dots_duration="500"
            app:dots_size="medium" />
            
            
            <com.razzaghimahdi78.dotsloading.linear.LoadingScaly
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            app:dots_color="@color/colorPrimaryDark"
            app:dots_count="5"
            app:dots_duration="400"
            app:dots_size="medium" />
            
            <com.razzaghimahdi78.dotsloading.linear.LoadingDancing
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            app:dots_color="@color/colorPrimaryDark"
            app:dots_count="3"
            app:dots_duration="800"
            app:dots_size="medium" />
            
            
            <com.razzaghimahdi78.dotsloading.circle.LoadingCircleFady
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            app:dots_color="@color/colorPrimaryDark"
            app:dots_duration="800"
            app:dots_size="medium" />
            
            <com.razzaghimahdi78.dotsloading.circle.LoadingCircleRotation
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            app:dots_color="@color/colorPrimaryDark"
            app:dots_duration="800"
            app:dots_size="medium" />
```

## Step 4. How to initial

```Java
        LoadingWavy LoadingWavy=findViewById(R.id.loadingWavy);
        LoadingWavy.setSize(DotSize.MEDIUM);
        LoadingWavy.setDotsCount(3);
        LoadingWavy.setDuration(400);
        LoadingWavy.setColor(Color.parseColor("#FF3700B3"));

```

```Kotlin
        val LoadingWavy: LoadingWavy = findViewById(R.id.loadingWavy)
        LoadingWavy.setSize(DotSize.MEDIUM)
        LoadingWavy.setDotsCount(3)
        LoadingWavy.setDuration(400)
        LoadingWavy.setColor(Color.parseColor("#FF3700B3"))
```

Done !!!

### **Note**

There are 5 type of sizes:

```Java
public enum DotSize {
    TINY,
    SMALL,
    MEDIUM,
    BIG,
    HUGE
}
```


https://user-images.githubusercontent.com/61207818/214298326-3f5d8aa2-38c5-4dab-ab5f-695639f5ff0f.mp4



