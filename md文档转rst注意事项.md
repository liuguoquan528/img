# 关于文档名称

文档中请勿写文档名称，文档名称在conf.py中定义

# 关于标题

标题里不要包含编号，编译为pdf或html后会自动添加编号

# 关于标题层级
markdown标题语法当前层级下跨标题级别，如：H1,H3时，转rst时会出错（标题级别不一致或直接无法识别该标题）。

# 关于标点符号
markdown文档编辑时英文双引号“”不成对，标点符号全角半角问题出错也会导致文档内容超出pdf A4纸不换行。

# 关于编写文档注意事项
文档编写时注意标题的英文大小写问题，正文断句，有逗号没句号应避免。

# 代码块

请使用围栏代码块的形式，将代码用 ``` 包围，可标注代码种类，也可以不标注。

效果如下：

``` shell
#For Ubuntu
# apt install dkms -y
# update-pciids
#For CentOS
# yum install dkms -y
# update-pciids
```

# 表格示例

- 请务必设置表名，设置方法：在markdown的原表格上面加入": [表名]"并加一空行
- 各列宽目前仅支持等分，如果表格列数多文字长，建议不要采用表格而是采用其他形式展现（例如列表等）
- 如果表格中包含图片，且图片较大的情况，请不要采用表格形式展现，因为pdf文档宽度有限。建议：表格中仅备注 见下方图“图片名称”，然后将图片放在表格下方

```
: 表格名称

| 时间      | 版本 | 作者 |
| --------- | ---- | ---- |
| 2022.2.25 | 2.0  | 张三 |
```

效果如下：

: 表格名称

| 时间      | 版本 | 作者 |
| --------- | ---- | ---- |
| 2022.2.25 | 2.0  | 张三 |

# 图片示例

- 正文中的图片请务必设置图片名称，如下，“安装语言”即为图片名称
- 图片路径中请全部使用"/"，例如将"image\"请全部改为"image/"

示例如下：

```
![安装语言](image/windows_install_language.png)
```

效果如下：

![安装语言](image/windows_install_language.png)

# 脚注

请参考如下示例：

```
Here's a simple footnote,[^1] and here's a longer one.[^2]
 
 
[^1]: This is the first footnote.
 
[^2]: Here's one with multiple paragraphs and code.
Here's one with multiple paragraphs and code.
Here's one with multiple paragraphs and code.
```

# 文档内部链接

```
[代码块](#代码块)
```

请注意不要添加标题编号！#号是必须的（且#好的层级不能乱）！否则最后生成的pdf将不能跳转

# 注意事项

**Note：** md没有特定语法表示

