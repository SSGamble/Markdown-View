## MarkedView Example

[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-MarkedView-green.svg?style=true)](https://android-arsenal.com/details/1/3801)
[![License](https://img.shields.io/badge/license-MIT-green.svg)]()
[![Platform](https://img.shields.io/badge/platform-Android-green.svg) ]()
[![Download](https://api.bintray.com/packages/mittsuu/maven/markedview/images/download.svg) ](https://bintray.com/mittsuu/maven/markedview/_latestVersion)


![sample_sc](https://github.com/mittsuu/MarkedView-for-Android/blob/master/sample-sc.gif)


## Introduction


The MarkedView is the markdown text viewer.


## Usage


It is a simple module, which enable you to convert any files into initialized view.


```xml
// xml
<com.mittsu.markedview.MarkedView
    android:id="@+id/md_view"
    android:layout_width="match_parent"
    android:layout_height="match_parent"/>

```


```java
// Java code

import com.mittsu.markedview.MarkedView;

・・・

// call from xml
MarkedView mdView = (MarkedView)findViewById(R.id.md_view);
// call from code
// MarkedView mdView = new MarkedView(this);

// set markdown text pattern. ('contents' object is markdown text)
mdView.setMDText(contents);

// load Markdown file pattern.
// mdView.loadFile(filePath)

```

```java
/* option */

// code block in scrolling be deactivated.
mdView.setCodeScrollDisable();

```

## Demo

* Load file

Read markdown file from asset folder.

* Live rendering

Preview display on the right side of the input field.

![sample_lr](https://github.com/mittsuu/MarkedView-for-Android/blob/master/sample-lr.png)


## Installation


Add the dependency

```gradle
dependencies {
    compile 'com.mittsu:markedview:1.0.5@aar'
}
```

## See Also

* MarkedView-for-iOS  
https://github.com/mittsuu/MarkedView-for-iOS


## Credits

This used the following open source components.

[Marked](https://github.com/chjj/marked) : Markdown parser written in JavaScript

[highlight.js](https://highlightjs.org/) : Syntax highlighting for the Web


## License


MarkedView is available under the MIT license. See the [LICENSE](https://github.com/mittsuu/MarkedView-for-Android/blob/master/LICENSE) file for more info.
