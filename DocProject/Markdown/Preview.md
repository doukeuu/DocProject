#  Markdown 在Xcode中预览


1、在Finder中找到这个project，右键点击项目的.xcodeproj，选择显示包内容；

2、用TextEdit新建一个空白rtf文件，修改后缀名为.txt，打开并删除其中内容；

3、上述txt文件修改文件名，前面加英文句号（.），然后用.xcodesamplecode.plist替换整个文件名，此时文件变为隐藏属性，可通过Shift + Command + 。快捷键显示出来；

4、用TextEdit打开文件，将以下文件内容拷贝到文件中并保存：

```XML
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
<plist version="1.0">
<array />
</plist>
```

5、重新打开markdown文件，既见预览效果，但此时不能再修改，如果需改动，需将该.xcodesamplecode.plist文件移出.xcodeproj文件，需预览时再移入。

