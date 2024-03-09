// 题目1
const a = 0;
const obj1 = {
  a: 1,
  func: function() {
    console.log(this.a)
  }
}
const obj2 = {
  a: 2,
  func: () => {
    console.log(this.a)
  }
}
const obj3 = {
  a: 3,
  func: function() {
    return () => {
      console.log(this.a)
    }
  }
}
const obj4 = {
  a: 4,
  func: function() {
    return function() {
      console.log(this.a)
    }
  }
}

obj1.func();
obj2.func();
(obj3.func())();
(obj3.func()).call(obj1);
(obj4.func())();
(obj4.func()).call(obj1);



// 题目2
const Pro = () => {
    this.x = '1';
    this.y = function () {};
}
var p = new Pro();
