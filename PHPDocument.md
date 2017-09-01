# PHP Document

### 注意，所有内联（inline）模式中再次内联的，内部只能使用内联形式

* `@abstract` 指定为抽象类（已经弃用）
* `@access` 访问权限，如public、private、protected等等
* `@author` 作者信息
  * `@author authorName <example@domain.com>`
* `copyright` 版权信息
* `@category` 指定package的分组
* `@deprecated` 在未来的版本中将要被删除的元素，后面可以留空，也可以接版本号或具体描述
* `@example` 高亮的示例代码，有几种形式，其中的文件路径必须是fopen支持的路径：
  * `@example /path/to/example.php description`
  * `@example url://path/to/example.php description`
  * `@example relativepath/to/example.php description`
  * `<code>换行，包括验证php标签</code>`（内联）
  * `{@example /path/to/example.php startline number of lines }`
  * `{@example url://path/to/example.php startline number of lines }`
  * `{@example relative/path/to/example.php startline number of lines }`
* `@final` 指定为final（已经弃用）
* `@filesource` 指定直接将此元素解析为代码高亮
* `@global` 全局变量，有以下两种格式
  * `@global datatype $globalvariablename`
  * `@global datatype description`
* `@ignore` 忽略产生这个元素的phpdoc，比如用if分别执行的define，可以除去第一个define其余全部忽略
* `@internal` 开发人员内部phpdoc（在用户phpdoc中不可见）
  * `{@internal include other inline tags}}`
* `@license` 指定许可URL和名称
  * `@license URL name of license`
* `@link` URL链接，有如下几种形式：
  * `@link URL link text`
  * `@link URL ,URL, URL ,...`
  * `{@link URL description }`
  * `{@link element description }`
* `@method` 类外描述__call支持的函数
  * `@method function declaration description`
* `@name` PHP行为，将$GLOBAL['x']转换为$var
* `@package` 用于PHPDocument组织页面或类
  * `page-level package (defines, functions, includes/requires)`
  * `class-level package (class, all its variables and methods)`
* `@param` 函数参数，有两种形式（无限个数参数用`$paramname,...`表示）：
  * `@param datatype $paramname description`
  * `@param datatype1|datatype2 $paramname description`
* `@property` 类外描述__get和__set支持的属性，有几种形式：
  * `@property datatype $variablename description`
  * `@property-read datatype $variablename description`
  * `@property-write datatype $variablename description`
* `@return` 返回值说明
  * `@return datatype description`
  * `@return datatype1|datatype2 description`
* `@see` 元素链接
  * 支持如下（多个函数名由逗号分隔）：
    * `file.ext`
    * `elementname`
    * `class::methodname()`
    * `class::$variablename`
    * `functionname()`
  * `@see file.ext|elementname|class::methodname()|class::$variablename|functionname()|function functionname unlimited number of values separated by commas`
  * 未完待续，有需要补充的注意事项
* `@since` 第一次出现的版本信息，如@since Version 2.1
  * `@since version/info string`
* `@static` 静态函数或变量
* `@staticvar` 描述function/method使用到的静态变量
  * `@staticvar datatype description`
* `@subpackage` 配合`@package`组织包，指示子包
* `@todo` 将来要实现的功能
* `@tutorial` 教程的链接
  * `@tutorial package/ subpackage/ tutorialname.ext #section.subsection description`或`{@tutorial package/ subpackage/ tutorialname.ext #section.subsection description }
    * `package/` -- Preface to specify a tutorial in a specific package
    * `subpackage/` -- Preface to specify a tutorial in a specific package/subpackage
    * `#section` -- Link to a specific section of the documentation package/subpackage/tutorial.ext#section
    * `.subsection` -- Link to a specific sub-section of the documentation package/subpackage/tutorial.ext#section.subsection
* `@uses` 与`@see`相似，但是`@uses`在目标位置创建反向链接指向当前位置
  * `@uses file.ext|elementname|class::methodname()|class::$variablename|functionname()|function functionname description of how the element is used`
* `@var` 类属性的变量类型
 * `@var datatype description`
* `@version` 指定版本信息
* `{@inheritdoc}` 指定子类关于父类的信息
* 未完待续
