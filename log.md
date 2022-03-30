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

There was so much to write down but now that it's done, I just need to make a function to randomly choose three and display them on the screen.  And then the hardest part will come, the CSS.

# Day 23 (2/24/2022)

## Personal Project

Created a shuffle function and random number generator function.

## Thoughts

Able to shuffle the "deck" and create a random number generator that uses a Set so the same card cannot be picked.  Need to create a function to set a state variable with the picked cards and then map them onto the screen.

# Day 24 (2/25/2022)

## Personal Project

Adjust card picking function and state variables for cleaner code.

## Thoughts

Able to select a three card spread and map them out onto the screen.  Need to find out how to do a card flip and adjust CSS afterwards.

# Day 25 (2/26/2022)

## Personal Project

Try to add flip card.

## Thoughts

Unable to add flip card as of yet.  Need to read more documentation.

# Day 26 (2/27/2022)

## Codewars

A day of Codewars in Python.  Challenge was to return a string of hours and minutes given an integer.

## Thoughts

Had some trouble for the logic on this one.  For some reason I though the modulo operator was the best way but realized that a combination of flooring a divided integer and the modulo operator was the way to go.

# Day 27 (2/28/2022)

## Personal Project

Worked on a personal project.

## Thoughts

Able to get a flip animation in React Native using Animated.  Followed a blog post about it.  Currently all the cards flip all at once but I think that's fine.  Need to display the card information from the state variable after some user interaction.

# Day 28 (3/1/2022)

## Personal Project

Worked on a personal project.

## Thoughts

Replaced the spread selection pressable from a text box to a "fanned deck" image.  Able to get images overlapped and able to keep functionality to set selected cards.

# Day 29 (3/2/2022)

## Personal Project

Worked on a personal project.

## Thoughts

Added a modal and basic CSS layout.  Need to add background and probably better buttons/pressables to open and close modal.  Also should add a start animation to whenever the user presses the initial pressable at the top to show that a new reading has occurred.

# Day 30 (3/3/2022)

## Skill Building

Worked on a database using Python and PostgreSQL

## Thoughts

Had to look back on previous notes and examples.  Should've done more practice with this earlier.

# Day 31 (3/4/2022)

## Skill Building

Worked on a the database from yesterday

## Thoughts

Added serializers, models, urls, and views to the database.  Used django rest framework as well.  Still a bit rusty with the process but the practice is making it so things are coming back.  Will add more tables and related files to this exercise incrementally.

# Day 32 (3/5/2022)

## Codewars

Worked on a Codewars problem today.

## Thoughts

The code challenge was to find the sum of each element to the power of an integer in an array, find the sum of the array, and then return the difference.  I wrote it the more JavaScript way where I made a loop to find the sum of each element to the power of the given integer and then found the sum of the array and then returned the difference.  The Python way is more succinct.

# Day 33 (3/6/2022)

## Codewars

Worked on a Codewars problem today.

## Thoughts

The code challenge was to find and return the sum of an integer depending on certain key values in Python dictionary.  I just put a conditional to filter the necessary additions and then returned the sum.  Still haven't gotten around to really digging into Python and still have the JavaScript way in my head.

# Day 34 (3/7/2022)

## Skillbuilding

Worked on a database using Python, Djanog, and PostgreSQL

## Thoughts

Remembering more and more from the GA lesson.  Adding to the relational database incrementally.  Next step is to add more models and serializers with urls and views accompanying it.  Possibly add user authentication later.

# Day 35 (3/8/2022)

## Skillbuilding

Worked on a database using Python, Djanog, and PostgreSQL

## Thoughts

Added more models, some with multiple foreign keys.  Had to rearrange the models since code still reads from top to bottom.  Added in necessary serializers, views, and url paths.  Next step is to add user authentication.

# Day 36 (3/9/2022)

## Codewars

Worked on a Codewars challenge.

## Thoughts

The challenge was to find the min and max values of a list in Python and return it in a list.  I remembered that Python as the min() and max() methods so returning those values was pretty simple.

# Day 37 (3/10/2022)

## SQL commands

Refresher for SQL commands

## Thoughts

Starting to remember the SQL commands and SQL specifics.

# Day 38 (3/11/2022)

## Shortlisted readiness test

Did a readiness test for a company that I applied to.  Was unsure about the specifics of the prompt.

## Thoughts

Didn't know exactly how they wanted the output to be.  The directions just stated a two dimensional array to output on a HTML page but it was on and IDE with no HTML page attached so I just wrote down code that takes the input and creates a two dimensional array.

# Day 39 (3/12/2022)

## SQL commands

Refresher for more SQL commands.  Used this website: https://sqlzoo.net/wiki/SELECT_from_WORLD_Tutorial

## Thoughts

More SQL command skill building.  Learned about ROUND, XOR and LENGTH operator and <> which is the equivalent of NOT EQUAL.

# Day 40 (3/13/2022)

## Codewars

Did a Codewars challenge today.  The challenge was to convert an integer into another integer with two decimal places.

## Thoughts

Not a particularly difficult one but one where I learned something about Python.  I can use :.2f for two decimal places when using an f string.

# Day 41 (3/14/2022)

## Codewars

Did a Codewars challenge today.  The challenge was to find the sum of the min value of each element in a two dimensional list.

## Thoughts

Still need to work on the Python way to solve these challenges in Python.  Pretty much did a JavaScript way of declaring an empty list, appending the minimum of each list element in the given list, and then returning the sum.

# Day 42 (3/15/2022)

## MongoDB

Revisiting MongoDB, Mongoose, and Express.

## Thoughts

Alot of reviewing for noSQL databases wit MongoDB.  Started an exercise using Mongoose and Express.  Will finish at a later time.

# Day 43 (3/16/2022)

## Codewars

Did a Codewars challenge today.  The challenge today was to return a copy of the list but with the min value removed.

## Thoughts

Learned something interesting about Python.  You can copy a list by using this syntax '[:]'.  Made a copy, took the min value out, and then returned the list copy.

# Day 44 (3/17/2022)

## MongoDB

Revisiting MongoDB, Mongoose, and Express.

## Thoughts

Almost finished with the MongoDB exercise.  Last thing to add is the endpoints.

# Day 45 (3/18/2022)

## MongoDB

Revisiting MongoDB, Mongoose, and Express.

## Thoughts

Finshed MongoDB exercise 1.  All routes work.

# Day 46 (3/19/2022)

## Codewars

Did a Codewars challenge today.  The challenge was to find the total count of drinks and return the count number of glasses of water and return it as a string.

## Thoughts

Did a standard declare/initialize of a variable.  Found all the numeric elements of the string and added them to the count variable.  And then returned it as a string to fulfill the prompt.  The Python version other people did is crazy.

# Day 47 (3/20/2022)

## Codewars

Did a Codewars challenge today.  The challenge was to find the sum of the ASCII value of two string inputs based on the elements' alphabetical place and return the greater variable.

## Thoughts

Did a standard declare/initialize of a variable, found the sum of the ASCII values of each string, and returned the greater value.  Did not remember to use Python's sum() function.

# Day 48 (3/21/2022)

## SQL

Did more SQL command review.

## Thoughts

Learned about using nested SELECT.

# Day 49 (3/22/2022)

## SQL and Codewars

Did more SQL command review and Codwars challenge.  The code challenge was to return the difference between the max and min values of a list in Python.

## Thoughts

Practiced more with nested SELECT and started learning about correlated subqueries.  The code challenge was simple but I could've done some code golf and had a one line return statement.  Will remember the if else return statement for later if possible.

# Day 50 (3/23/2022)

## Django, PostgreSQL database exercise 2

Started another exercise using django and postgresql.  Description is in the repository.

## Thoughts

Made initial commits and scaffolded out multiple files.  Will need to install more packages and add urls.py and serializers.py.

# Day 51 (3/24/2022)

## Django, PostgreSQL database exercise 2

Started another exercise using django and postgresql.  Description is in the repository.

## Thoughts

Created initial models, serializers, views, and urls.  Will finish making the rest of the required models, serializers, etc. at a later time.

# Day 52 (3/25/2022)

## Django, PostgreSQL database exercise 2

Psuedo finishes database exercise 2.  Added the rest of the models, serializers, views, and urls.

## Thoughts

Realized yesterday that I created the django app not where I wanted it to.  Moved around some files but now having a SECRET KEY bug.  Pretty sure the database works if it's able to run.  Will try and fix at a later time.  If I wanted to add to this, it would be authentication.

# Day 53 (3/26/2022)

## Codewars

Did a Codewars challenge today.  The prompt is the following:
Description:
You live in the city of Cartesia where all roads are laid out in a perfect grid. You arrived ten minutes too early to an appointment, so you decided to take the opportunity to go for a short walk. The city provides its citizens with a Walk Generating App on their phones -- everytime you press the button it sends you an array of one-letter strings representing directions to walk (eg. ['n', 's', 'w', 'e']). You always walk only a single block for each letter (direction) and you know it takes you one minute to traverse one city block, so create a function that will return true if the walk the app gives you will take you exactly ten minutes (you don't want to be early or late!) and will, of course, return you to your starting point. Return false otherwise.

## Thoughts

Did not realize there was a .count feature for Python lists.  Did a multi-conditional statement keeping track of 'n', 'e', 's', 'w'.  And will remember that you can do a boolean return statement using equality operators.

# Day 54 (3/27/2022)

## Codewars

Did a Codewars challenge today.  The challenge was to return a boolean to see if the function input is a square number.

## Thoughts

Was able to do a single line return statement and kind of looked Python-esque.  Did a ternary return statement, imported math to use the sqrt() function, and tested to see if the square root was an integer and not a float.

# Day 55 (3/28/2022)

## Basic Sorting Algorithms

Reviewed bubble and insertion sort.

## Thoughts

Was able to write a bubble sort algorithm after reviewing the notes from SEIR1115.  Insertion sort was different because I came accross the same / similar solution as I did in the course but it didn't work properly.  Had to look online for reference and came across a different solution.  Can be found here https://stackabuse.com/insertion-sort-in-javascript/ . Ultimately, need to go through the algorithm step by step for visualization purposes and to fully understand what the code was doing.

# Day 56 (3/29/2022)

## Divide and Conquer Sorting

Reviewed quick and merge sort.

## Thoughts

Had to go back through my previous solution which was aided by the solutions branch in the GA repository.  Had trouble creating the solution again and needed to break things down more mentally to understand why the code is written the way it is.  Will probably have to come back and review it again.

# Day 57 (3/30/2022)

## Distribution Sorting

Reviewed bucket sort.

## Thoughts

Had to do some review.  The logic for bucket sort seemed easier to grasp than the other sorting algorithms so far.  Had to copy and paste insertion sort because bucket sort uses it.