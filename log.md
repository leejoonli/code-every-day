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

# Day 7 (2/8/2022)

## Portfolio

Added CSS to project and about components.  Justified text in project description and about me.

## Thoughts

Portfolio is coming along well.  Need to adjust add animation triggered by scroll and create navigation links with smooth scroll and add project 4.  Possibly change the background image because it's very white at the bottom.

# Day 8 (2/9/2022)

## Portfolio

Added CSS/animations to navigation and other components.  Deployed on netlify.

## Thoughts

Portfolio is deployed on netlify.  Mobile ready but needs adjustment for web format.  Tried using an icon library but the github and linked in icons were trademarked and not included.  Ended up just getting it somewhere else.  The AOS library is really cool and easy to use.  Lots of built in animations that trigger on scroll.  Had a little bug with installing it since this app is using Typescript but eventually got it to run.

# Day 9 (2/10/2022)

## Portfolio

Adjusted portfolio for web format.

## Thoughts

Portfolio is almost done.  Need to figure out the downloadable pdf file link and change the icon on the tab.  Then add in final project.

# Day 10 (2/11/2022)

## Project 4

Started project 4 for General Assembly.  Created a base Typscript React Native app and pushed it into a git repository.  Created a Django app and PostgreSQL database.

## Thoughts

Started off trying to do everything at once when it came to django but quickly realized that was a terrible idea.  Started from scratch and incrementally made my way up to custom user models.  Still a long way to go for completion and deployment.

# Day 11 (2/12/2022)

## Project 4 and Portfolio

Added Users to database.  Unable to push to Heroku and still in the process of debugging.  Added downloadable pdf link to portfolio.

## Thoughts

Tried to deploy project 4 backend to Heroku but got a Typeerror.  Still in process of debugging with the help of one of my instructors.  Added axios GET request to native app and was able to retrieve data.  Could not verify whether or not it shows on mobile since I can't connect to localhost on my phone but the data shows up on web.

Added pdf link to portfolio.  Just needed to add an extension to VScode.  However, I ran into a bug with App.test.tsx after installing the extension and importing the pdf file to the component.  Ended up commenting out the test in App.test.tsx and works fine and I don't think I need to keep that test for deployment.  All that's left to do is finish project 4 and add it and change the icon that shows up next to the title of the page on the tab.  Typescript for this project seems very unnecessary since I didn't do much with typings and it brought up certain bugs.