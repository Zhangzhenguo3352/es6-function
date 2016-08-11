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
    var show=()=>{ //���� {} ������ʲô����ʲô������ {} ���൱������� return
        alert(1)
    }
    show()
```

```
    <script>
        window.onload=function(){
            var oDiv = document.querySelector('.div1');
            oDiv.onclick=()=>{ // function �� () ���� () ��������ǡ���ͷ���� ��=>
                alert(1)
            }
        }
    </script>
```

```
�Ƿ�֧��anguments,
<script>
//    function show(){
//        alert(arguments.length)
//    }
    var show=()=>{
        alert('��:  es6 ��֧�� arguments')
        //alert(arguments.length)
    }
    show(1,2,3)
</script>
```

```
���캯��,<br>�������� ���캯��
<script>
//    function Person(name,age){//���캯��
//        this.name = name;
//        this.age = age;
//    }
//    Person.prototype.showName = function(){
//        return this.name;
//    };
//    var p1 = new Person('abc',12)
//    alert(p1.showName())

    //�����Ĺ��캯��
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

