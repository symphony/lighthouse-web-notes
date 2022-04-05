## Tips

### Variables
Storing your output strings as variables keeps them tidy and allows you to update them easily! This will also help keep your functions clean and easy to read.
```js
const lunchMsg = "This is my string to be printed!"
console.log(lunchMsg)
```

### Cascading If statements
The order that you check conditions matters. Try to think of which expressions trump others, and then check for them first.
```js
  if (!hungry) return notHungryMsg
  if (time < 20) return underTwentyMsg
  if (time <= 30) return underThirtyMsg
  return overThirtyMsg
  ```
  This way you don't have to repeat identical checks such as:
```js
if (time > 20 && time < 30)
else if (time < 20)
```

  If you are only looking for one If statement to be true, then you can test them one by one and break out of the search once you've found it. This helps you reduce messy nesting and keeps your code concise and readable.