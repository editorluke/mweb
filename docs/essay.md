
###0602

* [x] constructor
    * 父类的构造函数
    
        ```
        function a(c){
            this.b = c;
            this.d =function(){
                alert(this.b);
            }
        }
        var obj  = new a('test');
        alert(obj.constructor);//function a(){}
        alert(a.prototype.constructor);//function a(){}
        
        obj是没有constructor 这个属性的，但是 obj.__proto__ = a.prototype;
        就从a.prototype中寻找，而 a.prototype.constructor 是就a。
        所以两者的结果是一一样的.
        
        ```
        
        





