[文档详见原项目](https://github.com/hinesboy/mavonEditor#readme)

# 说明
这个包修复了mavonEditor@2.9.0存在的xss问题.
虽然官方打了补丁,但是仍然需要自行配置xss规则,且对预览模式不生效.查看了源码之后,
发现mavonEditor是基于markdown-it开发的,其本身具有xss方面配置项.现在修改配置
后打包供自己现有项目使用.

现在在文本中输入HTML标签会被过滤,如果有展示HTML标签的需要,请使用markdown语法中
的代码块包裹,即可正常显示.