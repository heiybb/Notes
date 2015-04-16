# Lingo教程

### 模板

```
模板1
sets:
person/cong,zhu,zhe/:old;
index/cong,zhe/:i;
endsets

data:
i=1,3;
old=2,3,4;
enddata

min=@sum{index{j}:old{i}};

模板2
sets:
yu/1..3/:y,x;
endsets

data:
y=2,?,4;
enddata

init:
x=1,,3;
endinit

min=@max(yu(i):x*y);

@for(yu(i):@bnd(1,x,3))

模板3
sets:
yu/Nov2012..Jan2013/:y;
cong/w,q/:i;
meng(yu,cong);
endsets

data:
y=1,2,3;
i=1,3;
enddata

min=@sum(zhu(l,j,k):y(i));


```
