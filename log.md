# Day 1 (2/2/2022)

## Code Challenge

Welcome. In this kata, you are asked to square every digit of a number and concatenate them.

For example, if we run 9119 through the function, 811181 will come out, because 92 is 81 and 12 is 1.

Note: The function accepts an integer and returns an integer

## Code Challenge Solution

```js
function squareDigits(num){
  const str = num.toString();
  let newNum = '';
  for(let i = 0; i < str.length; i++) {
    newNum += (parseInt(str[i]) ** 2);
  }
  return parseInt(newNum);
}
```

## Thoughts

Originally, I converted num to a string and then used .split('') but it returned an object and not an array.  When researching why, I learned that the output of String.prototype.split is an Array and that is an Object.

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split#Summary

So I just used a for loop, stored it in a new variable, and then converted it to a number.

# Day 2 (2/3/2022)

## Portfolio

Pushed initial commit and scaffolded out components for my portfolio.  Created a react app with typescript.

## Thoughts

Didn't put alot of actual code down since I was reading on typings-for-css-modules-loader.

# Day 3 (2/4/2022)

## Portfolio

Filled all components previously scaffolded out.  Added necessary information and other placeholder text.

## Thoughts

Filling out content is time consuming.  The hour went by so fast.

# Day 4 (2/5/2022)

## Portfolio

Added CSS to multiple components and added a placeholder div element for home page image.

## Thoughts

CSS is so time consuming but necessary.

# Day 5 (2/6/2022)

## Portfolio

Added CSS to multiple components and import images.

## Thoughts

Need to rename image files for img src paths.

# Day 6 (2/7/2022)

## Portfolio

Added CSS to technologies components and display images.

## Thoughts

Had to import each image because it was giving an img src path error.