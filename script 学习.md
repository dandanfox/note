# script 学习

Array

### create a Array



```
  var fruits=["Apple","Banana"];

  console.log(fruits.length)

  fruits.forEach(function(item,index){
    console.log(item,index);
  });

  fruits.push('Oranges');   //append to array

  fruits.pop();             //remove last element

  fruits.shift();           //remove firest elemnt from Array

  fruits.unshift('first element');        //add element to index 0

  var pos = fruits.indexOf("Apple");

  var removedItem = fruits.splice(pos,1); //splice(start,deleteCount,[add elements])

  var shallowCopy = fruits.slice();//copy a Array
```
