# DOM 是什么？有什么用？

> 这里说的`DOM`是泛指文档对象模型整个技术栈（`不是指DOM节点`）；

## DOM是什么？

`DOM` （`Documnet Object Model`）中文名是：文档对象模型。  

## DOM有什么用？ 

> 文档对象模型的作用：
> 文档对象模型提供了一套方法来`增删改查` `DOM节点` 。（提供了document对象）

- 可用这样理解：网页中显示的内容都是由`DOM节点`构成的，网页中显示的内容改变了，本质就是修改了某些`DOM节点`。
- 那么`React.js框架`写出来的网页，在使用的过程中，状态改变了，会导致页面渲染更新。其实就是`React操作了DOM节点`来更新页面的。

# DOM节点是什么？有什么用？

## DOM节点是什么？

整个文档（网页中显示的内容）就是由`许多的DOM节点`组成的，`DOM节点`是文档的`一个颗粒`，`html中的每个标签`都有一个`元素节点`与之对应；html标签中的`每一对属性`也都有一个`属性节点`与之对应；html中的`每段文本`也都有一个`文本节点`与之对应。

## DOM节点有什么用？

让我们可以`使用JavaScript`通过`增删改查DOM节点` 来修改页面展示的内容。

## DOM节点的特性：

所有节点`本质都是一个JavaScript对象`，既然是对象就有属性。所有的节点都包含如下属性：`nodeType` `nodeName` `nodeValue`

```js
const textElement = document.createElement('div')
console.log(textElement)           // <div></div>
console.log(typeof textElement)    // 'object'
console.log(textElement.nodeType)  // 1
console.log(textElement.nodeName)  // 'DIV'
console.log(textElement.nodeValue) //  null
```



# DOM范畴里的 document对象提供的3个获取 文档中节点的方法。

要弄清楚：我们在html里说的是元素 ；和DOM里还有JavaScript里说的是节点；dom中的文档可用理解为页面中显示的内容。

###### 1.getElementById

###### 2.getElementsByTagName

###### 3.getElemnetByClassName

# 文档中元素提供的获取本身属性，和设置本身属性的2个方法

1.getAttribute

2.setAttribute



createElement

createTextNode

appendChild

insertBefore

 

> 

# DOM树是什么？



DOM节点分为三类： 1.元素节点 2.属性节点 3.文本节点