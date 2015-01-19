title: Python Challenge(I)
date: 2015-01-18 11:27:25
tags: [Python]
---

[Python Challenge](http://www.pythonchallenge.com/)是一个解题游戏网站, 每解出一道题就会跳到下一题. 目前为止一共有33关. 虽说是Python Challenge, 其实用其他语言,比如Java, C++都是可以的.

[第0关](http://www.pythonchallenge.com/pc/def/0.html)
提示很明显了, 换一下URL地址. 把地址中的0换成 2^38.
``` Python
2 ** 38
```
得到第二关地址http://www.pythonchallenge.com/pc/def/274877906944.html

<br />
[第1关](http://www.pythonchallenge.com/pc/def/274877906944.html)
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
[第2关](http://www.pythonchallenge.com/pc/def/ocr.html)
根据提示, 在网页源码里找到一大段字符串。里面写着“find rare characters in the mess bellow”, 所以要我们统计字符的个数, 找出出现次数少的字符。字符串太长, 就不贴上来了, 假定字符串存在msg里
``` Python
for c in set(msg):
    print c, msg.count(c)
# 得到
'''
1219
! 6079
# 6115
% 6104
$ 6046
& 6043
) 6186
( 6154
+ 6066
* 6034
@ 6157
[ 6108
] 6152
_ 6112
^ 6030
a 1
e 1
i 1
l 1
q 1
u 1
t 1
y 1
{ 6046
} 6105
'''
```
把只出现一次的那几个字母组合一下, 得到"equality", 替换URL里的"ocr"得到 http://www.pythonchallenge.com/pc/def/equality.html

<br />
[第3关](http://www.pythonchallenge.com/pc/def/equality.html)
