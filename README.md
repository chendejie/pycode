# python doc
## 编码
`# -*- coding: utf-8 -*-`
- 考虑兼容Emacs编辑器,使用上面写法, 不考虑兼容,使用下面写法
`# coding: utf-8`
- 其它自定义格式（不推荐），只要满足以下正则表达式即可
`# ^[ \t\f]*#.*?coding[:=][ \t]*([-_.a-zA-Z0-9]+)`
## 类型
### 数字
```

	+ - * / %
	/: 返回float类型
	//:真除,返回最大的整数结果int
	除了int,float,还有decimal.Decimal,fractions.Fraction,complex
```
### 字符串
```
	- 单行字符串: 
		单引号: '字符串'
		双引号: "字符串"
	- 字符串中都可以有转移字符
	- 如果想字符串中\x不被转移,可以在字符串引号前添加r如: r'c:\some\name'
	- 多行字符串:
		'''可以是多行字符串'''
		"""可以是多行字符串"""
	- 字符串重复: *
	- 字符串合并: +
	- 两个具体字符串相邻会自动合并
```
