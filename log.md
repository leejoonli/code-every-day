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

# Day 11 (2/12/2022)

## Project 4 and Portfolio

Still haven't resolved bug unfortunately but added favicon to portfolio so a small win.  Lots of reading React Native documentation and testing.

## Thoughts

Still can't deploy to Heroku for whatever reason but I have a great team of instructors to rely on.  We'll get it eventually.  The favicon was really easy to put in thanks to https://convertio.co/ and some instruction from Tyler Conti.  Testing the React Native components is pretty cool and doing it with Typescript is interesting.  For now, Typescript is giving me bugs to fix, mainly because of type declarations but I'm fully team Typescript over regular JavaScript.

# Day 12 (2/13/2022)

## Project 4 and Portfolio

Still haven't resolved bug.  Tested more native core components in the meantime.

## Thoughts

Don't know how to fix the backend deployment bug.

# Day 13 (2/14/2022)

## Project 4

Resolved backend deployment bug.  Tested more native core components and added another api call.

## Thoughts

Turns out my backend local repository wasn't the latest version so when I tried to deploy to heroku it was using an outdated repo.

# Day 14 (2/15/2022)

## Project 4

Ran into a bug with the api call on expo.  Changed the textinput function and started working but now running into logout bug.

## Thoughts

There's alot of differences between React and React Native.  Very similar in terms of structure but the syntax for mobile development is different.  Interesting nonetheless.

# Day 15 (2/16/2022)

## Project 4

Completed MVP.  Achieved full CRUD functionality and added CSS.  Very minimal CSS but enough for this kind of application.  Used typings for almost everything, albeit some are considered bad habits.

## Thoughts

Very tired, writing this at 1am, need to sleep so I can deploy for tomorrow.  I keep forgetting to push this to GitHub so the map can be full of green.

# Day 16 (2/17/2022)

## Project 4 and Portfolio

Deployed project 4 to Expo and updated portfolio repository.

## Thoughts

Wanted to deploy to the App store but there's a developer account fee that you need to pay before distribution.  Ended up deploying to the Expo servers but any user needs the Expo Go app downloaded on their phone to view the application.  Also, updated portfolio to include project 4 and updated resume.

# Day 17 (2/18/2022)

## Codewars

Today is the end of GA SEIR1115.  Ended up doing a code challenge today on Codewars.

## Thoughts

Original solution passed the initial unit tests but the ATTEMPT unit tests came back failing.  My guess is that my solution took too long in terms of time complexity.  Refactored and passed.  Did it in Python and it was a bit weird to come back to it after only using it for backend stuff on my project.

# Day 18 (2/19/2022)

## Codewars

Today was a relaxing day of Codewars.  Had to find the min and max of a string of numbers and return back the min and max as a string.

## Thoughts

My solution was to split the string into an array of substrings, convert each substring in the list into an integer, find the min and max, convert the min and max into a string, and then return it.  Could probably refactor it to be better.  In fact the other solutions for this kata were very Python-esque answers.  I still have a lot to learn about Python.

# Day 19 (2/20/2022)

## Codewars

Another day of Codewars.  Today's challenge was to check if a given string is an isogram and return either true or false.  Done in Python.

## Thoughts

My solution was to first change the string into all lowercase with string.lower(), create an empty list to hold unique letters, then loop through the letters of the string, check to see if the letter is already in the list, and if it does exist return False, but if it finishes the loop return True.

# Day 20 (2/21/2022)

## Codewars

Another day of Codewars.  Today's challenge was to reverse words in a string while keeping double spaces and keeping the order of words the same.  Done in Python.

## Thoughts

During my google search, I came across an interesting Python-esque solution and it seemed to work.  I had to look up what .join in Python did and remember that you can essentially do a for loop inside of built-in functions and methods.

# Day 21 (2/22/2022)

## Codewars

Another day of Codewars.  Today's challenge was to get the ascii values of each letter in a string, join them together, find the sum of the joined values, create a new variable where any instance of 7 is replaced by 1, and return the absolute value of the original variable minus the new variable.

## Thoughts

This one was interesting and I did it in probably the worst way possible.  I created a list to store the split string letters, changed them to their ascii values, converted the elements back into a string to join them together, converted it back to an integer, and then found the sum of each individual element in the new integer.  And of course, I stored the new variable with the replaced values in a new variable and that was done while the original variable was still the string version of the joined elements.  And after finding the sum of each individual element for the new variable, I returned the absolute value of the original variable minus the new variable.  Looking at other people's solutions, it looks like I just did the long hand version of the order of operations which means my solution could've been refactored into a more sucinct Python-esque answer.

# Day 22 (2/23/2022)

## Personal Project

A full day of putting in seed data for a personal project intended as a gift for a friend.

## Thoughts

There was so much to write down but now that it's done, I just need to make a function to randomly choose three and display them on the screen.  And then the hardes part will come, the CSS.