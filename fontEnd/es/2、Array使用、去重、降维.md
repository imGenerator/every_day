# 一、数组常规用法，增删查改迭代、元素是否存在
添加元素
```add Element
push
unshift()
slice()
splice()
concat()
```
删除元素
```delete Element
pop() // 末尾delete
shift() // 首位delete
splice(0,key) //指定键值delete，从第几位del
```
查询元素
```search Element
find()
findIndex()
keys()

```
修改元素
```fix Element
通过slice()
通过索引，直接赋值的方式
```
数组的迭代
```iterator item
some()
every()
filter()
map()
forEach()
reduce()
for...in
for...of...
for 
```
确认元素是否存在集合内
```
includes()
findIndex()
```
# 二、降维
就是将多维数据结构转化一维的数据结构
1.判断集合元素是否为数组类型
2.使用递归
```
const dimensionalityReduction = (item) =>{
  let newArray = [];
  return function(){
    if(Array.isArray(item)){
      return dimensionalityReduction(item);
    }else{
      newArray.push(item);
    }
    return newArray;
  }
}
```
# 三、去除重复
```
```