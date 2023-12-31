[TOC]

# 介绍

常量和变量听名字就知道是什么意思了吧，常量声明后不被修改而变量可以。这两个东西有什么用呢？我觉得不用去介绍，在看完本篇文章后你应该就会有个大概的印象了。

# 声明

**常量和变量在使用之前必须声明！**你只要知道有这个规则就行了，想必不需要用教小朋友的方法来给你举一个生动形象的例子了吧？

```swift
let a = 1 // 声明常量
var b = 2 // 声明变量
```

如上述代码所示**`let`用来声明常量**、**`var`用来声明变量**（`// 文字`这样的格式表示注释，你可以在`//`后面写任何内容而不影响代码本身）。不出意外这两个单词只要输入在你的编辑器中就会立马变色。

学会怎么声明之后然后尝试输入以下代码：

```swift
a = 3
b = 4
c = 5
```

不出意外的话就要出意外了，你的编辑器会在`a = 3`和`c = 5`这两行报错。应该都很好理解的吧：

1. a 是用`let`声明的常量，不可以修改，遂报错。
2. b 是用`var`声明的变量，可以修改，故正常。
3. c 根本就没有声明，更别提修改了，当然报错了。

## 单行声明

```swift
let a = 1, b = 2, c = 3, d = 4 // 声明多个常量
var e = 5, f = 6, g = 7, h = 8 // 声明多个变量
```

声明是学会了，但是当我们需要大量的常量或变量的时候一个一个的声明就太繁琐了，按照上述代码直接在一行去写就行了，每个常量/变量之间用`,`（**英文逗号**）分隔开。

> 切记写代码的时候除了注释不要用任何中文符号！！！真用了细心看看报错提示也应该能找出来，用个好分辨中英文符号的字体写多了一眼就应该可以分辨出来（编辑器默认的应该就还不错）。后面我就不再强调了，真的太多初学者经常犯这样的错误了。
