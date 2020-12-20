学习笔记




使用LL算法构建AST（抽象语法树）-语法分析
LL（left left）算法（从左到右扫描，从左到右规约）
LR算法

四则运算：
nuumber、oparate

语法定义：
<code>
&lt;expression&gt;::=
    &lt;additiveexpression&gt&lt;eof&gt;
&lt;additiveexpression&gt;::=
    &lt;multiplicaticeexpression&gt;
    &lt;additiveexpression&gt;&lt;+&gt;&lt;multiplicativeexpression&gt;
    &lt;additiveexpression&gt;&lt;-&gt;&lt;multiplicativeexpression&gt;
</code>