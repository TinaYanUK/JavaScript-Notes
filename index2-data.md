
### Data
.unshift() 加数组最前面
.push() 加数组最后面

.shift() 减数组最前面一个
.pop() 减数组最后面一个

.splice(index, numbers of elements)
返回被切掉的数组
```markdown
let array = ['I', 'am', 'feeling', 'really', 'happy'];
let newArray = array.splice(3, 2);
// newArray equals ['really', 'happy']
```
.splice(index, numbers of elements, elements added to the same index)
```markdown
const numbers = [10, 11, 12, 12, 15];
const startIndex = 3;
const amountToDelete = 1;

numbers.splice(startIndex, amountToDelete, 13, 14);
// the second entry of 12 is removed, and we add 13 and 14 at the same index
console.log(numbers);
// returns [ 10, 11, 12, 13, 14, 15 ]
```
