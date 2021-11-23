### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  let res;
  if (hungry === false) {
    res = 'Go back to work';
  } else {
    if (availableTime < 20 && availableTime > 0) {
      res = 'Maybe a banaana for lunch.';
    } else if (availableTime >= 20 && availableTime <= 30) {
      res = 'Maybe a Bigmac.Yum!';
    } else if (availableTime > 30) {
      res = 'Why not have a Steak?';
    }
  }
  return res;
};
```