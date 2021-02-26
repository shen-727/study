# MARKDOWN 语法(简略版)

## 标题

使用 `#`及`##……`来表示标题，例如：  

```markdown
### 标题测试
```

或单行 `=`或 `-` 来表示

```markdown
标题测试1
========
标题测试2
--------
```

## 段落换行

段落换行使用两个以上空格加回车

或直接空行进行换行

## 字体类型

```markdown
*斜体文本*  
_斜体文本_  
**粗体文本**  
__粗体文本__  
***粗斜体文本***  
___粗斜体文本___ 
```

*斜体文本*  
_斜体文本_  
**粗体文本**  
__粗体文本__  
***粗斜体文本***  
___粗斜体文本___  

## 分隔线

你可以在一行中用三个以上的星号、减号、底线来建立一个分隔线，行内不能有其他东西。你也可以在星号或是减号中间插入空格。下面每种写法都可以建立分隔线

```markdown
---
***
___
```

---
***
___

## 删除线

如果段落上的文字要添加删除线，只需要在文字的两端加上两个波浪线 `~~` 即可

```markdown
~~删除线~~
```

~~删除线~~

## 下划线

下划线可以通过 HTML 的 `<u>` 标签来实现：

```markdown
<u>下划线</u>
```

<u>下划线</u>

## 脚注

```markdown
脚注[jiaozhu]

[jiaozhu]:脚注是对文本的补充说明。
```

脚注[jiaozhu]

[jiaozhu]: markdown

## 列表

无序列表使用星号`(*)`、加号`(+)`或是减号`(-)`作为列表标记，这些标记后面要添加一个空格，然后再填写内容：

```markdown
* 列表
+ 列表
- 列表
```

* 列表
* 列表
* 列表

有序列表使用数字并加上` . `号来表示，如：

```markdown
1. 列表
2. 列表
3. 列表
```

1. 列表
2. 列表
3. 列表

列表嵌套只需在子列表中的选项前面添加四个空格即可：

```markdown
1. 列表
   - 嵌套
```

1. 列表
   * 嵌套
  
## 区块

Markdown 区块引用是在段落开头使用` > `符号 ，然后后面紧跟一个空格符号，区块是可以嵌套的：
```markdown
> 1
>> 2
>>> 3
```
> 1
>> 2
>>> 3  

在区块中使用列表
```markdown
>* 1
>+ 2
>- 3
```
>* 1
>+ 2
>- 3

在列表中使用区块
```markdown
* 1
   > a
   > b
* 2
   > c
   > d
```
* 1
   > a  
   > b
* 2
   > c  
   > d

## 代码
如果是段落上的一个函数或片段的代码可以用反引号把它包起来（``` ` ```）
``` ` printf() ` ```
` printf() `  
你也可以用` ``` `包裹一段代码，并指定一种语言（也可以不指定）：
```markdown
    ```c
    #include <stdio.h>
    int main()
    {
      printf("hellow world!");
      return 0;
    }
    ```
```
```c
#include <stdio.h>
int main()
{
   printf("hellow world!");
   return 0;
}
```
## 链接
```markdown
[链接名称](链接地址)

或者

<链接地址>
```

[百度](https://baidu.com)  
<https://www.baidu.com>

高级链接
```markdown
这个链接用 1 作为网址变量 [Google][1]
这个链接用 runoob 作为网址变量 [Runoob][runoob]
然后在文档的结尾为变量赋值（网址）

  [1]: http://www.google.com/
  [runoob]: http://www.runoob.com/
```
这个链接用 1 作为网址变量 [Google][1]  
这个链接用 runoob 作为网址变量 [Runoob][runoob]  
然后在文档的结尾为变量赋值（网址）

[1]: http://www.google.com/
[runoob]: http://www.runoob.com/

## 图片

开头一个感叹号 !  
接着一个方括号，里面放上图片的替代文字  
接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上选择性的 'title' 属性的文字。

```markdown
![picture]![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")
```
![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")  
<img src="http://static.runoob.com/images/runoob-logo.png" width="70%">

## 表格
Markdown 制作表格使用` | `来分隔不同的单元格，使用` - `来分隔表头和其他行。
```markdown
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |
```
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |

我们可以设置表格的对齐方式：

`-:` 设置内容和标题栏居右对齐。  
`:-` 设置内容和标题栏居左对齐。  
`:-: `设置内容和标题栏居中对齐。

## 高级技巧
支持HTML元素，如  
使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑
