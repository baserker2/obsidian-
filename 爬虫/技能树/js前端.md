[JavaScript 语法 | 菜鸟教程 (runoob.com)](https://www.runoob.com/js/js-syntax.html)
前端技术汇总：
https://vue3js.cn/interview/vue/vue.html#%E4%BA%94%E3%80%81vue%E5%92%8Creact%E5%AF%B9%E6%AF%94

Vue，
webpack，
Jquery，
原始Ajax

js命令
onfetch是什么
[JavaScript 如何使用 Fetch API来获取数据|极客教程 (geek-docs.com)](https://geek-docs.com/javascript/javascript-tutorials/t_how-to-use-javascript-fetch-api-to-get-data.html)
$（）用法，jquery的元素查询器
[JS中$含义及用法 - JokerJason - 博客园 (cnblogs.com)](https://www.cnblogs.com/jokerjason/p/7404649.html)
js中object继承自prototype
[深入理解JavaScript——Object（对象） - 个人文章 - SegmentFault 思否](https://segmentfault.com/a/1190000042363833)
[JavaScript prototype（原型对象） | 菜鸟教程 (runoob.com)](https://www.runoob.com/js/js-object-prototype.html)
js中的作用域scopes
[JavaScript 作用域（Scope）详解 - 天份& - 博客园 (cnblogs.com)](https://www.cnblogs.com/forever-Ys/p/10091422.html)
js中的闭包：arguments 的主要用途是保存函数参数， 但这个对象还有一个名叫 callee 的属性，返回正被执行的 Function 对象，回调


自执行与webpack特征关系
[JS逆向实战19——通杀webpack逆向 - 始識 - 博客园 (cnblogs.com)](https://www.cnblogs.com/zichliang/p/17517073.html)
[Webpack 理解 Chunk - 掘金 (juejin.cn)](https://juejin.cn/post/6844903889393680392)
























定义var，let
JavaScript 对象是属性和方法的容器，就一嵌套json
创建对象的方法 methodName : function() { 代码 }
创建函数function myFunction(_var1_,_var2_)  {  代码_ }

JavaScript 函数可以通过一个表达式定义。
函数表达式可以存储在变量中：
var x = function (a, b) {return a * b};
var z = x(4, 3);
以上函数实际上是一个 **匿名函数** (函数没有名称)。
函数存储在变量中，不需要函数名称，通常通过变量名来调用。

## Function() 构造函数（类似java中抽象函数？）

var myFunction = new Function("a", "b", "return a * b");  
// Function("a", "b", "return a * b");  构造函数本体
var x = myFunction(4, 3);

自调用函数（**匿名自我调用的函数**）
函数无名且由（）包裹
(function () {  
    var x = "Hello!!";      // 我将调用自己  
})();

深入js语法
[深入理解JavaScript——Object（对象） - 个人文章 - SegmentFault 思否](https://segmentfault.com/a/1190000042363833)
数据结构
[数据结构与算法 | 菜鸟教程 (runoob.com)](https://www.runoob.com/data-structures/data-structures-tutorial.html)

[什么块级作用域，什么是函数作用域？它们有什么区别？ - 腾讯云开发者社区-腾讯云 (tencent.com)](https://cloud.tencent.com/developer/news/1065655)

立即执行函数
( function ( “ 参数 ” ) { " 函数方法 " ; } ) ( “ 给参数传的值 ” )
( function ( " 参数 " ) { “ 函数方法 ” ; } ( " 给参数传的值 " ) )
! function ( " 参数 " ) { " 函数方法 " ; } ( " 给参数传的值 " )　 
// ! 可以换作 void 或其他运算符（比如 +，-，= 等，都能起到立即执行的作用）

匿名函数
[【Web】从零开始的js逆向学习笔记(上)_webjs逆向学习-CSDN博客](https://blog.csdn.net/uuzeray/article/details/136118382)

