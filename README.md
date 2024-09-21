# NoboButton
&nbsp;
Simple and fast way to create android button with icon, radius, background 

&nbsp;
### What is new? 
Please view the releases page for version change logs. [View Releases](https://github.com/alex31n/NoboButton/releases/)

&nbsp;
### Features!
- Drawable Resource - position, padding
- Font Awesome Icon - color, position, padding
- Radius, Background and Focus color
- Border - color and width
- Text - normal color, disable color,  size, style, AllCaps 

&nbsp;
### Screenshot
![Nobo Button Screenshot](https://raw.githubusercontent.com/alex31n/NoboButton/master/assets/button_screenshot.jpg)

&nbsp;
### Install

&nbsp;
Step 1. Add the JitPack repository to your build file  
Add it in your root build.gradle at the end of repositories:
```gradle
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        mavenCentral()
        maven { url 'https://jitpack.io' }
    }
}
```

Step 2. Add the dependency
```gradle
dependencies {
    implementation 'com.github.alex31n:NoboButton:2.0.7'
}
```

&nbsp;
### Use

&nbsp;
#### XML
Include namespace to the root View/Layout :
```
xmlns:app="http://schemas.android.com/apk/res-auto"
```
NoboButton with custom params
```
<com.ornach.nobobutton.NoboButton
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:padding="10dp"
    android:layout_marginBottom="20dp"
    app:nb_text="Buy Now"
    app:nb_borderColor="#FFFFFF"
    app:nb_borderWidth="2dp"
    app:nb_backgroundColor="#EF3D56"
    app:nb_focusColor="#B83CC3"
    app:nb_textColor="#FFF"
    app:nb_radius="5dp"
    app:nb_fontIcon="&#xf291;"/>
```

&nbsp;
#### JAVA
```
NoboButton button = new NoboButton(this);
button.setText("Submit");
button.setTextColor(Color.RED);
button.setAllCaps(true);
button.setFontIcon("\uf138");
button.setIconPosition(NoboButton.POSITION_LEFT);
button.setBackgroundColor(Color.WHITE);
button.setFocusColor(Color.GRAY);
button.setBorderColor(Color.RED);
button.setBorderWidth(2);
button.setRadius(10);
```

&nbsp;
#### Font Awesome Icon

Cheatsheet http://fontawesome.io/cheatsheet/

Note: before use **font awesome** please see their license http://fontawesome.io/license/

&nbsp;
#### Attributes
| Description (Data type) | XML Attribute | Java Attribute | 
|-------------------------------|-------------|-------------|
| Text (String) | app:text="Button Text" | setText("Submit") |
| Text color (color) |  app:textColor="#FFF" | setTextColor(Color.WHITE) |
| Text size (dimension) |  app:textSize="18sp" | setTextSize(18) |
| UPPER Text (boolean) |  app:textAllCaps="true" | setAllCaps(true) |
| Text Style (int); supported style: NORMAL, BOLD, ITALIC  |  app:textStyle="bold" | setTextStyle(NoboButton.TEXT_STYLE_BOLD) |
| border color (int) | app:borderColor="#FFF" | setBorderColor(Color.WHITE); |
| border width (dimension) | app:borderWidth="2dp" | setBorderWidth(2) |
| background color (int) | app:backgroundColor="#FF0000" | setBackgroundColor(Color.RED) |
| focus/pressed color (int) | app:focusColor="#FF4081" | setFocusColor(Color.GRAY) |
| radius of button (dimension) | app:radius="10dp" | setRadius(10) |
| disabled text color | app:disabledTextColor="#DDD" | setDisabledColor(Color.GRAY) |
| Awesome font unicode (String) | app:fontIcon="&#xf291;" | setFontIcon("\uf007"); |
| Icon drawable resource (int) | app:drawableResource="@drawable/ic_camera" | setDrawableResource(R.drawable.ic_camera) |
| Icon color (int) | app:iconColor="#FFF" | setIconColor(Color.WHITE) |
| Icon position (int); Supported position, LEFT, TOP, RIGHT, BOTTOM | app:iconPosition="left" | setIconPosition(NoboButton.POSITION_LEFT) |
| Space between icon & text (dimension) | app:iconPadding="10dp" | setIconPadding(10) |


&nbsp;
&nbsp;
## License
    Copyright 2017 Alex Beshine
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and limitations under the License.
    
