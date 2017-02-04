Markdown 语法:

A First Level Header
====================
A Second Level Header
---------------------

Now is the time for all good men to come to
the aid of their country. This is just a
regular paragraph.

The quick brown fox jumped over the lazy
dog's back.
### Header 3

> This is a blockquote.
> 
> This is the second paragraph in the blockquote.
>
> ## This is an H2 in a blockquote
输出 HTML 为：

<h1>A First Level Header</h1>
<h2>A Second Level Header</h2>
<p>Now is the time for all good men to come to
the aid of their country. This is just a
regular paragraph.</p>
<p>The quick brown fox jumped over the lazy
dog's back.</p>
<h3>Header 3</h3>
<blockquote>
<p>This is a blockquote.</p>
<p>This is the second paragraph in the blockquote.</p>
<h2>This is an H2 in a blockquote</h2>
</blockquote>
修辞和强调

Markdown 使用星号和底线来标记需要强调的区段。

Markdown 语法:

Some of these words *are emphasized*.
Some of these words _are emphasized also_.
Use two asterisks for **strong emphasis**.
Or, if you prefer, __use two underscores instead__.
输出 HTML 为:

<p>Some of these words <em>are emphasized</em>.
Some of these words <em>are emphasized also</em>.</p>
<p>Use two asterisks for <strong>strong emphasis</strong>.
Or, if you prefer, <strong>use two underscores instead</strong>.</p>
列表

无序列表使用星号、加号和减号来做为列表的项目标记，这些符号是都可以使用的，使用星号：

* Candy.
* Gum.
* Booze.
加号：

+ Candy.
+ Gum.
+ Booze.
和减号

- Candy.
- Gum.
- Booze.
都会输出 HTML 为：

<ul>
<li>Candy.</li>
<li>Gum.</li>
<li>Booze.</li>
</ul>
有序的列表则是使用一般的数字接着一个英文句点作为项目标记：

1. Red
2. Green
3. Blue
输出 HTML 为：

<ol>
<li>Red</li>
<li>Green</li>
<li>Blue</li>
</ol>
如果你在项目之间插入空行，那项目的内容会用 <p> 包起来，你也可以在一个项目内放上多个段落，只要在它前面缩排 4 个空白或 1 个 tab 。

* A list item.
With multiple paragraphs.

* Another item in the list.
输出 HTML 为：

<ul>
<li><p>A list item.</p>
<p>With multiple paragraphs.</p></li>
<li><p>Another item in the list.</p></li>
</ul>
链接

Markdown 支援两种形式的链接语法： 行内 和 参考 两种形式，两种都是使用角括号来把文字转成连结。

行内形式是直接在后面用括号直接接上链接：

This is an [example link](http://example.com/).
输出 HTML 为：

<p>This is an <a href="http://example.com/">
example link</a>.</p>
你也可以选择性的加上 title 属性：

This is an [example link](http://example.com/ "With a Title").
输出 HTML 为：

<p>This is an <a href="http://example.com/" title="With a Title">
example link</a>.</p>
参考形式的链接让你可以为链接定一个名称，之后你可以在文件的其他地方定义该链接的内容：

I get 10 times more traffic from [Google][1] than from
[Yahoo][2] or [MSN][3].

[1]: http://google.com/ "Google"
[2]: http://search.yahoo.com/ "Yahoo Search"
[3]: http://search.msn.com/ "MSN Search"
输出 HTML 为：

<p>I get 10 times more traffic from <a href="http://google.com/"
title="Google">Google</a> than from <a href="http://search.yahoo.com/"
title="Yahoo Search">Yahoo</a> or <a href="http://search.msn.com/"
title="MSN Search">MSN</a>.</p>
title 属性是选择性的，链接名称可以用字母、数字和空格，但是不分大小写：

I start my morning with a cup of coffee and
[The New York Times][NY Times].

[ny times]: http://www.nytimes.com/
输出 HTML 为：

<p>I start my morning with a cup of coffee and
<a href="http://www.nytimes.com/">The New York Times</a>.</p>
图片

图片的语法和链接很像。

行内形式（title 是选择性的）：

![alt text](/path/to/img.jpg "Title")
参考形式：

![alt text][id]

[id]: /path/to/img.jpg "Title"
上面两种方法都会输出 HTML 为：

<img src="/path/to/img.jpg" alt="alt text" title="Title" />
代码

在一般的段落文字中，你可以使用反引号 ` 来标记代码区段，区段内的 &、< 和 > 都会被自动的转换成 HTML 实体，这项特性让你可以很容易的在代码区段内插入 HTML 码：

I strongly recommend against using any `<blink>` tags.

I wish SmartyPants used named entities like `&mdash;`
instead of decimal-encoded entites like `&#8212;`.
输出 HTML 为：

<p>I strongly recommend against using any
<code>&lt;blink&gt;</code> tags.</p>
<p>I wish SmartyPants used named entities like
<code>&amp;mdash;</code> instead of decimal-encoded
entites like <code>&amp;#8212;</code>.</p>
如果要建立一个已经格式化好的代码区块，只要每行都缩进 4 个空格或是一个 tab 就可以了，而 &、< 和 > 也一样会自动转成 HTML 实体。

Markdown 语法:

If you want your page to validate under XHTML 1.0 Strict,
you've got to put paragraph tags in your blockquotes:

<blockquote>
<p>For example.</p>
</blockquote>
输出 HTML 为：

<p>If you want your page to validate under XHTML 1.0 Strict,
you've got to put paragraph tags in your blockquotes:</p>
<pre><code>&lt;blockquote&gt;
&lt;p&gt;For example.&lt;/p&gt;
&lt;/blockquote&gt;
</code></pre>


蚂蚁和大象
====================

>蚂蚁和大象结婚不久，就闹起了矛盾。
>
>蚂蚁：每天一上床，你就只顾着自己呼呼大睡，也不抱抱我。
>
>大象：你还恶人先告状，每天我一上床就到处找你，你可倒好，无终无影，搞外遇去了吧。
>
>蚂蚁：当初见你身材高大，想你定是个有担当的人，不会让女人操劳，我才嫁给你。不想嫁给你之后，我还是一样的劳碌苦命。
>
>大象：当初我还看不上你啦，又黑又瘦。但我妈见你勤快，就劝我说‘黑点儿瘦点儿怕啥。结婚之后，给她吃好点，养白养胖不就行
>
>了’。不想你婚后这般吃法还是又黑又瘦。