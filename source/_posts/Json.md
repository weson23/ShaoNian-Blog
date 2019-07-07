---
title: Json
date: 2019-04-09 22:50:16
tags:
---
# JSON:JavaScript Object Notation

### 什么是 JSON ？
* JSON 指的是 JavaScript 对象表示法（JavaScript Object Notation）
* JSON 是轻量级的文本数据交换格式
* JSON 是存储和交换文本信息的语法
* JSON 具有自我描述性，更易理解
### 优点（和XML对比）
1. 比XML 更小、更快，更易解析。

---
### JSON使用范围
*  用于编写基于JavaScript应用程序，包括浏览器扩展和网站。
*  JSON格式可以用于通过网络连接序列化和传输结构化数据。
*  主要用于在服务器和Web应用程序之间传输数据。
*  Web服务和API可以使用JSON格式提供公用数据。
*  还可以用于现代编程语言中。

### JSON语法
 JSON 语法是 JavaScript 语法的子集。
 
**一.语法结构**
1. 数据在“名称/值对”中
2. 数据由逗号分隔
3. 大括号 **"{}"** 保存对象
4. 中括号 **"[]"** 保存数组   

---
**二.JSON名称/值对**    
JSON 数据的书写格式是：名称/值对

值的组成:
1. 数字：（整数或浮点数）
2. 字符串：（在双引号中）
3. 逻辑值：（true 或 false）
4. 数组：（在中括号中（[]））
5. 对象：（在大括号（{}）中）
6. null

---
**三.JSON对象**  

实例：  
`{ "name":"runoob", "alexa":10000, "site":null }`  

JSON 对象使用在大括号({})中书写、对象可以包含多个 key/value（键/值）对。 

key 必须是字符串，value 可以是合法的 JSON 数据类型（字符串, 数字, 对象, 数组, 布尔值或 null）。

key 和 value 中使用冒号(:)分割、每个 key/value 对使用逗号(,)分割。

**访问对象值**  

实例：  
```
var myObj, x;
myObj = { "name":"runoob", "alexa":10000, "site":null };
```

1. 使用点号（.）来访问对象的值：    
实例：  
`x = myObj.name;`

2. 也可以使用中括号（[]）来访问对象的值：   
实例：  
`x = myObj["name"];`

**修改值**

1. 使用点号(.)来修改 JSON 对象的值：    
实例：  
`myObj.sites.site1 = "www.google.com";`

**删除对象属性**
1. 使用 delete关键字来删除JSON对象的属性:   
实例：  
`delete myObj.sites.site1;` 
2. 使用中括号([])来删除 JSON 对象的属性：   
实例：  
`delete myObj.sites["site1"]`

---
**四.JSON数组**   

实例    
`[ "Google", "Runoob", "Taobao" ]`

JSON数组在中括号中书写 

JSON 中数组值必须是合法的 JSON 数据类型（字符串, 数字, 对象, 数组, 布尔值或 null）  

实例：  
```
{
"name":"网站",
"num":3,
"sites":[ "Google", "Runoob", "Taobao" ]
}
```
1. 可以使用索引值来访问数组：   
`x = myObj.sites[0];`
2. 修改数组值   
`myObj.sites[1] = "Github";`
3. 删除数组元素     
`delete myObj.sites[1];`    
---     
**五.JSON.parse()** 