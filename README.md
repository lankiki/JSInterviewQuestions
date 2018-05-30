1.js 实现一个函数对javascript中json 对象进行克隆
var oldObject ="sdf";
   var newObject = JSON.parse(JSON.stringify(oldObject));
   console.log(newObject);
或者
    var a = 'dddd';
    function cp(a){return JSON.parse(JSON.stringify(a))}
    console.log(cp(a));
    
    
