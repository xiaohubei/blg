
#### 问：如果我想让属性abc是动态拼接的，怎么办？
````bash
obj['a' + 'bc'] = 123;
let propKey = 'foo';
let obj = {
  [propKey]: true,
  [`${propKey}` + 'abc']: 123,
  'first word': 'hello',
  ['h' + 'ello'] () {
    return 'hi';
  }
};
````
#### 问：可不可以这样定义一个对象
````bash
let obj = {
  'first word': 'hello'
};
````