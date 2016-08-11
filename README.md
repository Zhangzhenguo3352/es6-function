```
//    function show(a){
//        return a;
//    }
    var show=a=>a
    alert(show(1))
```

```
//    function show(){
//        return 1;
//    }
    var show=()=>1
    alert(show())
```

```
//    function show(){
//        return alert(1)
//    }
    var show=()=>alert(1)
    console.log(show())
```

```
//    function show(){
//        alert(1)
//    }
    var show=()=>{ //带了 {} 里面是什么就是什么，不带 {} 就相当于添加了 return
        alert(1)
    }
    show()
```

```
    <script>
        window.onload=function(){
            var oDiv = document.querySelector('.div1');
            oDiv.onclick=()=>{ // function 的 () 就是 () 它后面就是“箭头函数 ”=>
                alert(1)
            }
        }
    </script>
```

```
是否支持anguments,
<script>
//    function show(){
//        alert(arguments.length)
//    }
    var show=()=>{
        alert('答案:  es6 不支持 arguments')
        //alert(arguments.length)
    }
    show(1,2,3)
</script>
```

```
构造函数,<br>和真正的 构造函数
<script>
//    function Person(name,age){//构造函数
//        this.name = name;
//        this.age = age;
//    }
//    Person.prototype.showName = function(){
//        return this.name;
//    };
//    var p1 = new Person('abc',12)
//    alert(p1.showName())

    //真正的构造函数
    'use strict';
    class Person{
        constructor(name,age){
            this.name = name;
            this.age = age;
        }
        showName(){
            return this.name
        }
    }
    var p1 = new Person('abc','456');
    alert(p1.showName())
</script>
```

