# 学习笔记

## 使用LL算法构建AST（抽象语法树）

语法分析：
+ LL（left left）算法（从左到右扫描，从左到右规约）

+ LR（left right）算法

## 四则运算：
### 词法定义：
+ TokenNumber：1 2 3 4 5 6 7 8 9 0的组合
+ Oparate：+ - * /
+ Whitespace：<SP>
+ LineTerminator：<LF><CR>

### 语法定义：
<pre>
<code>
&lt;Expression&gt;::=<br/>
    &lt;AdditiveExpression&gt&lt;EOF&gt;<br/>

&lt;AdditiveExpression&gt;::=<br/>
    &lt;MultiplicaticeExpression&gt;<br/>
    &lt;AdditiveExpression&gt;&lt;+&gt;&lt;MultiplicativeExpression&gt;<br/>
    &lt;AdditiveExpression&gt;&lt;-&gt;&lt;MultiplicativeExpression&gt;<br/>

&lt;MultiplicativeExpression&gt;::=<br/>
&lt;Number&gt;<br/>
&lt;MultiplicativeExpression&gt;&lt;*&gt;&lt;Number&gt;<br/>
&lt;MultiplicativeExpression&gt;&lt;/&gt;&lt;Number&gt;<br/>
</code>
</pre>