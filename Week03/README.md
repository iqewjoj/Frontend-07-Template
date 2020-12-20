学习笔记




使用LL算法构建AST（抽象语法树）-语法分析
LL（left left）算法（从左到右扫描，从左到右规约）
LR算法

四则运算：
nuumber、oparate

语法定义：
<code><expression>::=
    <additiveexpression><eof>
<additiveexpression>::=
    <multiplicaticeexpression>
    <additiveexpression><+><multiplicativeexpression>
    <additiveexpression><-><multiplicativeexpression>
</code>