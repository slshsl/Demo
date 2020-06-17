[TCO]

# vs code 使用 Markdown 编写文档

## 使用 HTML 标签

直接使用 HTML 标签，可以设置文字居中，字体颜色等样色(HTML 语法)

```code
代码：
    <div align="center" style="color:red">VS Code 使用 Markdown 编写文档</div>
```
演示：
<div align="center" style="color:red">VS Code 使用 Markdown 编写文档</div>

## 标题写法

```code
代码：
    注：# 后面保持空格（和使用 h1/h2 标签功能类似）
    代码:      
    # 标题1
    ## 标题2
    ### 标题3
    #### 标题4
    ##### 标题5
    ###### 标题6
    标题一等价写法：在下面一行写三个等号（=），该文字自动格式化为标题1
    ===
    标题二等价写法：在下面一行写三个横线（-），该文字自动格式化为标题2
    ---
```

## 段落

这是段落
这是段落

## 引用

```code
代码1(单行式)：
    > hello world!
```
演示1：
> hello world!

```code
代码2(多行式)：
    > hello world!  
    > hello world!  
    > hello world!  
    > hello world!  
```
演示2：
> hello world!  
> hello world!  
> hello world! 

```code
代码3(多行嵌套)：
    > hello world!  
    >> hello world!  
    >>> hello world! 
```
演示3：
> hello world!
>> hello world!
>>> hello world!

## 强调（粗体、倾斜、删除）

*斜体*、_斜体_
**加粗** 、__加粗__
***加粗+斜体***、**_加粗+斜体_**
~~删除线~~
$\underline{下划线}$

## 标记 demo
==背景色== 

## 脚注
H~2~O
n^2^


## 语义标签

<i>斜体</i>
<b>加粗</b>
<em>强调</em>
<u>下划线</u>
<del>删除</del>
Z<sup>a</sup>
Z<sub>a</sub>
<kbd>Ctrl</kbd>

## 分隔符

三个或者更多星号、连接符(横线)、下划线
***
---
___

## 常用Font-Awesome

:notebook:

## 代码块

```code
  <div></div>
```

语法高亮

```javascript
  var num = 0;
  for (var i = 0; i < 5; i++) {
    num+=i;
  }
  console.log(num);
```
显示代码行数

```javascript{.line-numbers}
  var num = 0;
  for (var i = 0; i < 5; i++) {
    num+=i;
  }
  console.log(num);
```
高亮代码行数

```javascript{highlight=3}
  var num = 0;
  for (var i = 0; i < 5; i++) {
    num+=i;
  }
  console.log(num);
```
```javascript{highlight=1-2}
  var num = 0;
  for (var i = 0; i < 5; i++) {
    num+=i;
  }
  console.log(num);
```
```javascript{highlight=[1,3]}
  var num = 0;
  for (var i = 0; i < 5; i++) {
    num+=i;
  }
  console.log(num);
```

## 行内标记

你好`asdf`你好年后

## 链接
- 外部链接

  1. https://github.com

  2. [GitHub](https://github.com)

  3. [GitHub](https://github.com 'GitHub官网')

- 内部链接

  1. 链接仓库其他文件：[ReadMe](README.md)

  2. 链接本文档其他部分(空格用-代替)：[标记](markdown.md#标记-demo)

- 引用式链接

  1. [好看]

  2. 别名：[百度][baidu]

  3. 链接仓库其他文件：[ReadMe]

  4. 链接本文档其他部分：[标记]

## 图片链接

    ![alt](url text)
- 外部图片链接
  ![百度](https://dgss0.bdstatic.com/5bVWsj_p_tVS5dKfpU_Y_D3/res/r/image/2017-09-27/297f5edb1e984613083a2d3cc0c5bb36.png "百度网站")

- 内部图片链接
  ![百度1](https://github.com/slshsl/Demo/master/images/baidu.png "百度网站")

## 列表

  1. 有序列表
      1. 姓名
         1. 你好
         2. 你好
      2. 姓名
      3. 名称
  2. 无序列表(使用 *，+，- 表示无序列表)
      - 阿松大
      * 士大夫
        - 是否
        * 是否
      - 啊手动阀
      + asd

<!---下面是文档中引用的连接--->
[好看]:http://hao123.com
[baidu]:http://baidu.com
[ReadMe]:README.md
[标记]:markdown.md#标记-demo
