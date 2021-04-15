## **let const**
   - 块级作用域
      ```
        var a = [];
        for (var i = 0; i < 10; i++) {
          a[i] = function () {
            console.log(i);
          };
        }
        a[6](); // 10
        var a = [];
        for (let i = 0; i < 10; i++) {
          a[i] = function () {
            console.log(i);
          };
        }
        a[6](); // 6
      ```
      var声明 => 全局只有一个变量i => 每次循环都会改变i => 所有数组a的成员里面的i，指向的都是同一个i
      let声明 => 当前的i只在本轮循环有效 => 每一次循环的i其实都是一个新的变量，每一轮循环的变量i都是重新声明的（JavaScript 引擎内部会记住上一轮循环的值）
   - 不存在变量提升
   - 暂时性死区
   - 不允许重复声明

