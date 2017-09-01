[ref1]: https://manual.phpdoc.org/HTMLSmartyConverter/PHP/phpDocumentor/tutorial_tags.pkg.html "phpDocumentor tags"

# 写在前面

### 以前学Java的时候我是知道有Java Document的，可以用工具从源码的“``/**@xxx*/``”注释里提取并组织成API文档。
### 但是后来并没有对Java产生多大的兴趣（Android除外），最近有去学习PHP高级的用法，看了Smarty的源码，发现了一个有意思的东西。
### 我用的IDE是JetBrains的PhpStorm，我自己写的工厂类，用传递的$string产生目标类实例对象，但是IDE不能智能提示了，这就很烦呀，但是为什么Smarty就可以呢？明明Smarty还用了魔术方法，却还有详细的智能提示？

## 那今天我们的猪脚就上桌了：<b>PHP Document</b>

参考（Reference）：
+ [phpDocumentor] [ref1]
