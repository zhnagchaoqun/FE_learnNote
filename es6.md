## **let const**
   - 块级作用域
      (```)
        var a = [];
        for (var i = 0; i < 10; i++) {
          a[i] = function () {
            console.log(i);
          };
        }
        a[6](); // 10
      (```)
   - 不存在变量提升
   - 暂时性死区
   - 不允许重复声明

