1.js 实现一个函数对javascript中json 对象进行克隆
var oldObject ="sdf";
   var newObject = JSON.parse(JSON.stringify(oldObject));
   console.log(newObject);
或者
    var a = 'dddd';
    function cp(a){return JSON.parse(JSON.stringify(a))}
    console.log(cp(a));
2.js 实现 ajax 请求或者submit请求时 锁屏功能以及开锁功能（请求时界面Loading以及元素不能点击，请求完成即消除Loading）
function(url, fn) {
     var obj = new XMLHttpRequest(); // XMLHttpRequest对象用于在后台与服务器交换数据
     obj.open('GET', url, true);
     obj.onreadystatechange = function() {
            if(obj.readyState == 4 && obj.status == 200||obj.status == 304) {

                   loading.style.display = "none"

                } else {

                   alert("不能点击,哈哈哈!");

                }

       };
obj.send(null);
}
