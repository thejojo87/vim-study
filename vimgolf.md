[TOC]
# vimgolf
 
 18291 active golfers, 179992 entries, 347 challenges 

# 安装

## 1. 先安装gem
http://rubyinstaller.org/downloads/

## 2. windows powershell里

gem install vimgolf

## 3. 设置vimgolfkey

在网站登陆后，获取key，然后vimgolf setup

## 4. 安装gvim

ftp://ftp.vim.org/pub/vim/pc/gvim80-069.exe

# 开始

## 1. Simple, Practical, and Common - 11133 entries 

### 代码

vimgolf put 55b18bbea9c2c30d04000001

### 问题

Start file

*temp var1 0
*temp var2 "hi"
*temp var3 -1
*temp var4 42
*temp var5 "asdf"
*temp var6 0

Simple things we do all the time should be able to be done with very few keystrokes, but sometimes I find something I need to do makes me go, "There MUST be a better way."

This challenge is just a simple movement and entering text at a certain place.



End file

*temp var1 0
*temp var2 "hi"
*temp var3 -1
*temp var4 42
*temp var5 "asdf"
*temp var6 0
*temp var7 11

Simple things we do all the time should be able to be done with very few keystrokes, but sometimes I find something I need to do makes me go, "There MUST be a better way."

New text.

This challenge is just a simple movement and entering text at a certain place.


### 答案：22步

Here are your keystrokes:
#Yp<C-A>w11.GONew t<C-N><C-N>.<CR><Esc>ZZ

我能做到的最多就是26步

Here are your keystrokes:
5jyyp<C-A>w11.3joNew text.<CR><Esc>ZZ

第一步-光标移动到 第一段的最后一行。

因为这一行也是*temp开头的。
所以利用这一点，直接#从后面搜索出来了。

yy 直接用Y省了一次，不过yy更快我觉得。

下一步就是直接G，进入最后一行，然后O，上一行新建一个。

快速搜索 	
* 在文件中向前搜索当前光标所在的单词
# 在文件中向后搜索当前光标所在的单词 


退出 	ZQ 无条件退出
:q! 无条件退出
ZZ 存盘并退出
:wq 存盘并退出 