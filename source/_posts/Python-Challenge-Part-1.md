title: Python Challenge(I)
date: 2015-01-18 11:27:25
tags: [Python]
---

[Python Challenge](http://www.pythonchallenge.com/)是一个解题游戏网站, 每解出一道题就会跳到下一题. 目前为止一共有33关. 虽说是Python Challenge, 其实用其他语言,比如Java, C++都是可以的.

[第一关](http://www.pythonchallenge.com/pc/def/0.html)
提示很明显了, 换一下URL地址. 把地址中的0换成 2^38.
``` Python
2 ** 38
```
得到第二关地址http://www.pythonchallenge.com/pc/def/274877906944.html

<br />
[第二关](http://www.pythonchallenge.com/pc/def/274877906944.html)
根据图片上的提示, 应该是要做一个映射. 再加上"think twice"这个提示, 应该可以猜出是平移映射两位. 这里用到string的translate来完成
``` Python
import string
intab = string.ascii_lowercase
outtab = string.ascii_lowercase[2 : ] + string.ascii_lowercase[0 : 2]
table = string.maketrans(intab, outtab)
"map".translate(table)
```
URL上的"map" translate后得到"ocr", 这就得到了第三关的地址 http://www.pythonchallenge.com/pc/def/ocr.html
这一关图片下面有一大段英文, translate后可以得到
> i hope you didnt translate it by hand. thats what computers are for. doing it in by hand is inefficient and that's why this text is so long. using string.maketrans() is recommended. now apply on the url.

<br />
[第三关](http://www.pythonchallenge.com/pc/def/ocr.html)
