## Markdown

### 认识 Markdown
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Markdown 是一种轻量级的「标记语言」，它的优点很多，目前也被越来越多的写作爱好者，撰稿者广泛使用, 它用简洁的语法代替排版，而不像一般我们用的字处理软件 Word 或 Pages 有大量的排版、字体设置。它使我们专心于写作，用「标记」语法，来代替常见的排版格式。例如此文从内容到格式，甚至插图，键盘就可以通通搞定了。Markdown 的语法十分简单。常用的标记符号也不超过十个，这种相对于更为复杂的 HTML 标记语言来说，Markdown 可谓是十分轻量的，学习成本也不需要太多，且一旦熟悉这种语法规则，会有一劳永逸的效果。目前来看，支持 Markdown 语法的编辑器有很多，包括很多网站（例如简书）也支持了 Markdown 的文字录入。Markdown 从写作到完成，导出格式随心所欲，你可以导出 HTML 格式的文件用来网站发布，也可以十分方便的导出 PDF 格式。


### 常用语法介绍

####  标题	
		
		#	header1
		##	header2
		###		header3
		####	header4
		#####	header5
		
******** 
示例 

> # h1 (# h1)
> ## h2 (## h2)
> ### h3 (### h3)
> #### h4 (#### h4)
> ##### h5 (##### h5)
> ###### h6 (###### h6)

******* 
<br>

####  列表
		
		无序表 (*, +, -)
		* 1
		* 2
		* 3
		
		有序表 (数字后面加.)
		1. 1
		2. 2
		3. 3
	
示例
*****
> 无序表
> 
> + 列表 (+ 列表)
> * 列表 (* 列表)
> - 列表 (- 列表)
> 
> 有序表
> 
> 1. 列表 (1. 列表)
> 2. 列表 (2. 列表)
> 3. 列表 (3. 列表)

****
<br>


####  引用

	如果你需要引用一小段别处的句子，那么就要用引用的格式。
	> 引用文字


示例
*****
> > 引用文字 (> 引用文字)

****
<br>

#### 文字块

		文字块 使用 2个 tab 键并换行
		
示例
*****
>		文字块 (使用 2个 tab 键并换行)

****
<br>
		
#### 代码块
		
		代码块 (```语言 代码 ```)
		
		```语言
		代码
		```

示例 
*****	
>\`\`\`Swift
>
> import Foundation
> 
> var customerInline  = ["Chris", "Ewa", "Elex", "Alex", "Barry", "Daniel"]
>
> ....
>  
> \`\`\`

```Swift
import Foundation
var customerInline  = ["Chris", "Ewa", "Elex", "Alex", "Barry", "Daniel"]

// 自动闭包, 没有参数, 自动创建用于用于包装表达式作为函数的参数, 没有参数, 
// 当自动闭包被调用时, 表达式的返回值就是闭包的返回值, 这个语法非常方便的让你用{}
let customerPovider = {customerInline.remove(at: 0)}
func seve(customer customerProvider: () -> String) {
	print("Now serving \(customerPovider())")
}
// 自动闭包
func serve(customer customerProvider: @autoclosure () -> String) {
	print("Now serving \(customerPovider())")
}

func server(customer customerProvider: String) {
	print("Now serving \(customerProvider)")
}
```
*****	
<br>

#### 插入图片
	插图格式: ![名称](图片地址)
	
示例 
*****	
> \!\[百度logo](https://www.baidu.com/img/bd_logo1.png)
> ![百度logo](https://www.baidu.com/img/bd_logo1.png)

*****	
<br>


#### 链接地址
	文字链接: [名称](链接网址)
	图片链接: [![名称](图片地址)](链接网址)
	
示例 
*****	
> 文字链接&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\[百度](https://www.baidu.com)
> 
> [百度](https://www.baidu.com)
>
> 图片链接&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\[\![百度]\(www.baidu.com/img/bd_logo1.png)](https://www.baidu.com)
> [![百度](https://www.baidu.com/img/bd_logo1.png)](https://www.baidu.com)

*****	
<br>

#### 粗体
	粗体 **文字**
	
示例 
*****	
> 我的名字叫 **小明**

*****	
<br>

#### 斜体
	斜体 *文字*
	
示例 
*****	
> 我的名字叫 *小明*

*****	
<br>

#### 分割线
	***

示例
*****	
>	***

***
<br>


#### 删除线
	
	~~文字~~

示例
*****	
~文字~

***
<br>


~~文字删除线~~