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

# Day 58 (3/31/2022)

## Distribution Sorting

Learned about Radix sort.

## Thoughts

Had to do research about radix sort.  Learned that it implements count sort.  Understand how it works but still need to work on implementation and how it's written in code.

# Day 59 (4/1/2022)

## Codewars

Did a codewars challenge today.  The challenge was to find the max of the difference between two max length elements in two arrays.

## Thoughts

Did a very repetative solution.  Very JavaScript-esque but wanted some time to relax so I did some spaghetti code.  Got the solution to work.  Some of the other answers were very Python looking.  Still need alot of practice with Python and what it can do.

# Day 60 (4/2/2022)

## Codewars

Did a codewars challenge today.  The challenge was to swap cases of a string

## Thoughts

Did a for loop to iterate over the sting and then a conditional to check what case the letter is and then swap change it and add it to an empty string.  Then return the new string.  Did not know there was a swapcase() in Python.  Seems very convenient.

# Day 61 (4/3/2022)

## Codewars

Did a codewars challenge today.  The challenge was to round a number to the nearest 10th.

## Thoughts

Created a temp variable to divide the input integer by 10.  Then returned round(temp) * 10.  Saw another solution with round() and you can write it like round(i, -1) and it'll round to the nearest tenth.  Need to remember you can use negative numbers in these kinds of functions.

# Day 62 (4/4/2022)

## Binary Search

Reviewed binary search algorithm.

## Thoughts

Able to do the brute force solution of binary search.  Had an unnecessary nested loop while previous solution did not.  Had to reference previous solution for recursion.  Need to remember the default value to arguments in a function.

# Day 63 (4/5/2022)

## Personal Project

Finally continued the personal project.

## Thoughts

Imported most of the card images.  Not all because they are not labeled and I don't know which is which.

# Day 64 (4/6/2022)

## Personal Project

Continued the personal project.

## Thoughts

Removed flip animation and bad card packing image.  Realized I can't continue until all images are imported.

# Day 65 (4/7/2022)

## Codewars

Did a codewars challenge today.  The challenge was to iterate starting from the rightmost on an integer.  Had to convert to string and then back to int.

## Thoughts

Still doing Python challenges in a JavaScript way.  Don't understand one of the other solutions.

# Day 66 (4/8/2022)

## Codewars

Did a codewars challenge today.  The challenge was to find if the substring is included at the end of a given string.

## Thoughts

Able to do the code golf one line solution in Python.

# Day 67 (4/10/2022)

## Codewars

Did a codewars challenge today.  The challenge was to find if if the 2nd input is greater than the average of an array of numbers.

## Thoughts

Did a boolean comparison return statement.

# Day 68 (4/11/2022)

## Linked list review

Reviewed the GA lesson on linked lists.

## Thoughts

Need to review more.

# Day 69 (4/12/2022)

## Linked list review

Reviewed code from linked list assignment.

## Thoughts

Went over the node class, linked list class, append node, prepend node, pop, remove from front.

# Day 70 (4/13/2022)

## Linked list review

Reviewed code from linked list assignment.

## Thoughts

Went over the insert at, remove at, search, and sort.

# Day 71 (4/14/2022)

## Hash table review

Reviewed hash table GA lecture.

## Thoughts

Need to start coding hash table logic again.

# Day 72 (4/15/2022)

## Codewars

Did a codewars challenge today.  The challenge was to find the longest length string in a list and return the length.

## Thoughts

Was able to do a Python one line return statement.  Learned that you can use key=len in the max() function to get the longest length of a list of strings.

# Day 73 (4/16/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return a list of indexes of a string if the index is a vowel.

## Thoughts

Was able to do a Python one line return statement.  Had some trouble because the find index methods in Python don't return the current index of iteration.

# Day 74 (4/17/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return a sorted list if the input is truthy.

## Thoughts

Tried to do a one line return statement but syntax was off.  Was on the right track but didn't quite get it.

# Day 75 (4/18/2022)

## Personal project

Worked on a personal project.  Finalized background images and removed flip animation.

## Thoughts

Adding an image background is a bit annoying since there's no background image CSS property in React Native.

# Day 76 (4/19/2022)

## Personal project

Worked on a personal project.  Finalized application and deployed to Expo servers.

## Thoughts

Adding fonts in React Native is really a process I don't want to go through and the fonts available to Andriod is absolutely minimal.

# Day 77 (4/20/2022)

## Personal project

Reworked on a personal project.

## Thoughts

Mobile app development is now confirmed in my eyes to not be what I want to do.  I cannot deploy a version that others can use without paying for a development account.

# Day 78 (4/21/2022)

## Personal project

Reworked on a personal project.

## Thoughts

Redid the application is React and deployed on Netlify.

# Day 79 (4/23/2022)

## Codewars

Worked on a codewars challenge today.  The challenge was to return a boolean if the input is a narcissistic number (sum of the each character in the integer to the power of the length of the integer)

## Thoughts

Find it difficult to be Python esque with more complex algorithms.

# Day 80 (4/24/2022)

## Codewars

Worked on a codewars challenge today.  The challenge was to return a list of some strings depending on a conditional.

## Thoughts

Tried to do a Python answer but wasn't sure how with a ternary return statement.

# Day 81 (4/25/2022)

## Hash Table

Reviewed the hash table lesson and did a couple methods for the code.

## Thoughts

Mentally I have an idea on how it should work using walker but hard to put things into code with these complex data structures.

# Day 82 (4/26/2022)

## Hash Table

Reviewed the rest of the hash table lesson.

## Thoughts

Need to remember that these data structures can have other data structures and you can access methods in those classes.

# Day 83 (4/27/2022)

## C#

Started an introduction to C#.

## Thoughts

Mostly went over concepts used in C# and .NET.  Went over classes, namespaces (group of related classes), assemblies (group of related namespaces), CLR (common language runtime), IL (intermediate language).  C# is a programming language while .NET is a framework for building applications on Windows.

# Day 84 (4/28/2022)

## C#

Continued learning about C#.

## Thoughts

Went over more basics of C#.  How to declare variables and initialize them, naming conventions, overflow, scope, and went over a basic console application.

# Day 85 (4/29/2022)

## C#

Continued learning about C#.

## Thoughts

Went over more basics of C#.  Type conversion (implicit: byte->int depending on the value of byte it will add zeros to compensate for the lack of memory, explicit: int->byte will likely cause memory leak, and non-compatible types: str->int will need either Convert class in the System namespace or a parsing function which is included but I forgot the syntax) and operators.  The operators look exactly like other programming languages.  Mentioned bitwise operators but did not go in depth.

# Day 86 (4/30/2022)

## Codewars

Did a codewars challenge today.  The challenge was to validate if a given string input is an IP address.  Leading zeros are considered false.

## Thoughts

Did not know how to do this the Python way.  Did a loop and conditionals to check for edge cases.  Some of the other answers seem intense.

# Day 87 (5/1/2022)

## Codewars

Did a codewars challenge today.  The challenge was to mask a string input with hashes except the last 4 characters.

## Thoughts

Did a basic variable and loop to iterate through and had conditionals for whether or not to use a hash or the character in the string.

# Day 88 (5/2/2022)

## C#

Continued learning about C#.

## Thoughts

Practiced loops, conditionals, variable data types and operators.

# Day 89 (5/3/2022)

## C#

Continued learning about C#.

## Thoughts

Practiced lists (arrays) and looping through the array.

# Day 90 (5/4/2022)

## C#

Continued learning about C#.

## Thoughts

Practiced classes, objects, and methods.

# Day 91 (5/5/2022)

## Codewars

Did a codewars challenge today.  The challenge was to Jaden case a string (capitalize every word in a sentence).

## Thoughts

Did a basic variable declaration and used split method and join method to create the new capitalized words.  Looking at the other solutions, it could've been combined into a single line return statement.

# Day 92 (5/6/2022)

## Codewars

Did a codewars challenge today.  The challenge was to find the number of numbers in a range that don't contain the number 5.

## Thoughts

Used a list and appended numbers based on a conditional that didn't include 5.  Had to convert each iteration to a string and see if the string 5 was in the current iteration.  Then returned the length of the list.  Looking at the other solutions, it was essentially the same thing but condensed into a single line return statement.

# Day 93 (5/7/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return an array (list) of numbers that correspond with whether or not an index of a letter in a string matches its alphabetical position.

## Thoughts

Created a list to store the numbers, looped through the list, initialized a count variable, iterated through each string, compared whether the current letter's index matches its alphabetical counterpart, and if it did increased the count variable, then appended the count variable to the list and returned the list.  Had to break this problem down more than I originally thought.

# Day 94 (5/8/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return the nth root of a number.

## Thoughts

Turns out there's a mathematical operation that you can write in code that isn't a predetermined function in Python.  x**(1/n) to get the nth root of x.

# Day 95 (5/9/2022)

## C#

Reviewed what I learned earlier about C#.  Started to learn about LINQ.

## Thoughts

Very similar to SQL commands and JS array iterator methods.  There's something about enumerable and enumerator which I don't fully understand but will look into later.

# Day 96 (5/10/2022)

## C#

Continued learning about C#.  Learning more about LINQ and async / await.

## Thoughts

Understand that LINQ is used to query data from a database in C# but don't fully understand why you should use the queries.  Async and await seem similar to what I saw in JS but the keywords are attached to the function names.  Need to read more.

# Day 97 (5/11/2022)

## C#

Continued learning about C#.  Learning more about async / await.

## Thoughts

Learning more about the concept of async / await, when to use it, some nuances about Task and awaiting return value.  Following a C# video tutorial series CSharpFritz.

# Day 98 (5/12/2022)

## C#

Continued learning about C#.  Learning more about async / await.

## Thoughts

Continued following a C# video tutorial series CSharpFritz about async / await.  Still have a long way to go.

# Day 99 (5/14/2022)

## Codewars

Did a codewars challenge today.  The challenge was to find the minimum number of laps given two integer inputs two people have to do before they meet each other again.

## Thoughts

Looked like a case of finding the lowest common multiple of each integer input.  math.lcm didn't seem to work, probably because of version number based off of stack overflow answers, so created another function to return lcm, then returned two integers based off the input and the lcm.

# Day 100 (5/15/2022)

## Codewars

Did a codewars challenge today.  The challenge was to convert the sum of two integers into binary.

## Thoughts

Looked online and found bin() is a built in Python method.  It prefixes with 0b so used .replace() to get rid of the prefix.

# Day 101 (5/16/2022)

## Codewars

Did a codewars challenge today.  The challenge was to find if an array had a subset array inside it.

## Thoughts

Used a rather long conditional statement to return the correct value.  Saw a {}.issubset(set(array)) solution and thought it was really intersting.

# Day 102 (5/17/2022)

## C#

Continued learning about C#.  Finished video lesson on async / await.  Read documentation on creating an API with ASP.NET Core.

## Thoughts

I think I have a basic understanding of what the documentation example is trying to explain and of C# as a programming language.  Need to start coding.

# Day 103 (5/18/2022)

## C#, Portfolio, Django Database

Worked on API with C# and .NET Core, updated Python PostgreSQL database 1 and portfolio.

## Thoughts

Deployed database to heroku and updated portfolio to match.  Running into an error with the API exercise.  Will look into tomorrow.

# Day 104 (5/19/2022)

## C#, Django Database Documentation

Worked on API with C# and .NET Core, updated Python PostgreSQL database 1 README.md.

## Thoughts

Able to solve the API error.  Continued with the walkthrough in the Microsoft documentation.  Not complete yet.

# Day 105 (5/20/2022)

## C#

Finsihed todo API with C# and .NET Core.

## Thoughts

Finished the walkthrough.  Not going to deploy to Azure because it's a subscription.

# Day 106 (5/23/2022)

## Stacks and Queues

Reviewed the lesson on stacks and queues.

## Thoughts

Finished an array based stack and queue.  Will need to read up on extra material for this topic later on.

# Day 107 (5/24/2022)

## Stacks

Did some independent learning about stacks.

## Thoughts

The use of stacks is more common than I realized and can be given in many coding interviews.  Need to brush up more on stacks and queues.

# Day 108 (5/25/2022)

## Stacks

Did some independent learning about stacks.

## Thoughts

The implementation of stacks for certain problems is more complicated than I though.  Looked over infix to postfix operands.  Didn't quite understand how to read postfix at the start but after a question on geek for geeks I have a better understanding.

# Day 109 (5/26/2022)

## Queues

Did some independent learning about queues.

## Thoughts

Read up about priority queues and how they could be implemented.  Instead of just the base value, you could use something like an object which also holds a property of the priority.  Then you would have to order the queue based on priority.  There are different organizations of queues, ASC or DESC, which affects the heap inside memory.

# Day 110 (5/27/2022)

## Sets

Did some review on the sets lecture.  Did the classic two sum problem.

## Thoughts

Redid the JS sets implementation from the GA lecture/homework.  Able to get through it, the last method confused me since the test was coming out failed.  Had to do with the order of the set returned.  Wrote a better two sum solution using a set.  Don't know why I was trying to create a nested for loop and use a set at the same time the first time around.

# Day 111 (5/30/2022)

## Hash Tables

Did some review on hash table lecture again.

## Thoughts

Looked over the code for recreating a hash table and was reminded of an array method I forgot about (Array.fill()).  Used linked lists inside an array.  OOP is pretty much the cornerstone in data structures in general.  I think time complexity is (O(n + 1) so it rounds to O(n) since we only care about the general complexity and not the specifics?).

# Day 112 (5/31/2022)

## Graphs

Did some review on GA graphs lecture.

## Thoughts

Refreshed on breadth first search (one side, recursion, like a finding the exit to a maze) and depth first search (one level at a time), adjacency list (object with array properties) and adjacency matrix (2d array of ones and zeros), direct (one node to the other, one direction) and undirect (relation from both nodes to each other).

# Day 113 (6/1/2022)

## Binary Trees

Did some review on GA binary tree lecture.

## Thoughts

Refreshed on the properties of a tree (root, leaf nodes, edges, key, siblings, parent, child, subtree, height), reviewed types of binary trees (full, degenerate, balanced, perfect, complete), reviewed traversing a binary tree with loops and recursion.  Need to finish out code review.

# Day 114 (6/2/2022)

## AVL Trees

Did some review on GA AVL tree lecture.

## Thoughts

Still don't fully understand how self balancing trees work.  Need to to more work and learning.

# Day 115 (6/3/2022)

## DevOps Pipeline, Codewars

Did some reading on DevOps Pipeline and a codewars challenge.  The challenge was to return the sum of the smallest two integers in a list in Python.

## Thoughts

There's a handy list.sort() method but when I was trying to use it, it was giving me a type error.  So I used sorted() and added the first two indices and returned the value and it seemed to work.  DevOps is getting more interesting as I read into it.  Read about CI/CD and how DevOps is the proprietor of that ideal.  The idea of creating an environment that has little downtime and is continuously monitored and tested is fascinating.  Need to do more reading and practice creating a pipeline.  Will follow the tutorial here https://www.atlassian.com/devops/continuous-delivery-tutorials/jira-jfrog-pipelines.

# Day 116 (6/6/2022)

## DevOps Pipeline

Did some more reading on DevOps.

## Thoughts

Read about DevOps toolchain and test automation.  There are multiple tools each having its own purpose whether it be planning, building, or monitoring the deployed application.  And it requires that all teams work together and test incrementally and often so that the deployed version is good to go and to also fix any issues rapidly.  Read about infrastructure as code.  Don't completely understand and will need to read into it further along with product manager examples and automated testing tools.

# Day 117 (6/7/2022)

## DevOps Pipeline

Did some more reading on DevOps.

## Thoughts

Read about YAML.  Yet Another Markup Language is interesting to learn about.  The codeifying of test automation is cool but I don't know how it works under the hood.  The YAML pipeline has the stage -> job -> script/task.  Stage ex: Build, Deployment, Monitoring. Job: Things to do/test. Script/task: how to do/test.  The cool thing about YAML pipeline is that you can edit the file directly using a text editor rather than using a specified tool to edit the file.  You can get it from the repository and make changes and commit those changes and the YAML file will be edited and executable afterwards.

# Day 118 (6/8/2022)

## DevOps Pipeline

Did some more reading on DevOps.

## Thoughts

Learned about a very basic multistage YAML pipeline.  Each stage will be dependent on the previous artifact being successfully built.  The last stage will stage the pipeline and then move it to production.  Each stage will execute commands and built artifacts to be used on the next stage.  This is getting more and more complicated but interesting.

# Day 119 (6/9/2022)

## Docker

Did some more reading on Docker.

## Thoughts

Docker is a platform as a service that packages software in "containers" which can be accessed and run on site and in public or private cloud.  The parts of a docker is: the Docker daemon, which manages the container and handles container objects, the objects which are images (a read only template used to build containers/used to store and ship applications), container (an encapsulated environment that runs applications), and service (allows containers to be scaled across multiple daemons/a set of cooperating daemons are called a swarm and it communicates through the Docker API), and registries which is a repository of all the Docker images.

# Day 120 (6/10/2022)

## Codewars

Did a codewars challenge today.  The challenge was to create a new property with a string value on every element in a dict in Python using already existing dict properties.

## Thoughts

Did a very simple for loop and added a new property on each dict in the list.  Tried doing a single line return statement but was not successful.  The single line return statement has a **dev which I'm not exactly sure what it does.  It looks like it allows you to pass multiple arguments to a function directly noted by this stack overflow answer: https://stackoverflow.com/questions/36901/what-does-double-star-asterisk-and-star-asterisk-do-for-parameters.

# Day 121 (6/13/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return a list with n elements that are even, negative included.

## Thoughts

Couldn't think of a way to do a one line return statement.  Did a loop and a conditional after n elements were appended in the list.  The other solutions are very elegant.  Was wondering if I could use a negative iteration and it turns out it's possible with [-n:] and a loop inside the return list.

# Day 122 (6/14/2022)

## Docker

Played around with Docker.

## Thoughts

Read more into Docker and created a beginner container following the tutorial.  Will continue with finishing tutorial at a later time.

# Day 123 (6/15/2022)

## Docker and Codewars

Read Docker documentation and did a codewars challenge today.  The challenge was to prefix the string elements in a list with numbers.

## Thoughts

Did a basic for loop and added to the beginning of the string.  Need to keep trying the one line return statements.

# Day 124 (6/16/2022)

## Codewars

Did a codewars challenge today.  The challenge was to add n elements and alternate what gets appended.

## Thoughts

Did a basic for loop and added a conditional based off the index.  One Python-esque solution is very interesting (return [[first_value, second_value][i % 2] for i in range(n)]).  There was another one that I did understand and now I remember that you can use a ternary loop in the returned list.

# Day 125 (6/17/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return the middle index of a string, if the string had an even length, return the two middle indices.

## Thoughts

Didn't realize when you divide a len() in Python, it returns as a decimal.  Need to learn more about the [:] Python syntax.

# Day 126 (6/20/2022)

## Codewars

Did a codewars challenge today.  The challenge was to remove elements from one list based off the elements in another list.

## Thoughts

Did a for loop with a filter and .__ne__ which was cool but the other solutions were so much simpler and more in line with Python coding.  A single line return with a loop in the brackets.

# Day 127 (6/21/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return a modified string input with no vowels.

## Thoughts

Did a basic loop with a conditional and a list of all the vowels needed to be searched for.  Could've just created a string instead of a list inside the conditional.

# Day 128 (6/22/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return the next perfect square.

## Thoughts

Did some basic algebra to find if the input is a perfect square, then add 1 to the perfect square, and then square it and return the value.  Forgot that there's a Python method called .is_integer() to find if the input was a perfect square.

# Day 129 (6/23/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return a list of a string input split by two chars.  If the length is odd add a '_'.

## Thoughts

Initialized an empty list.  Did a loop and appended each two chars into the list.  Then returned the list.

# Day 130 (6/24/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return the number of 1s in a binary string conversion of an integer input.

## Thoughts

Had difficulty understanding what the prompt was asking me to do.  Originally, I thought the prompt was asking to return the length of the bit conversion but it was asking to return the count of 1s in the bit conversion.  Found the bin() method which converts an integer into the binary string.  Looped over the string and counted the number of 1s and return it.  Could've used the .count() method.  return bin(n).count('1');

# Day 131 (6/27/2022)

## Codewars and Docker

Learned more about Docker today and did a codewars challenge today.  The challenge was to return a camelCase version of a string.

## Thoughts

Learned about very basic docker commands, the vital difference between images and containers (containers are more the environment and images are the things inside the environment to run the program).  Couldn't figure out how to do a one line return statement for the code challenge.  Did some basic methods to get the string how I wanted and returned it.

# Day 132 (6/28/2022)

## Codewars and Docker

Learned more about Docker today and did a codewars challenge today.  The challenge was to return a pig latin version of a string input.

## Thoughts

Learned more docker commands, how to run multiple services, and how to build a docker image.  Going to need to do actual practice to solidify knowledge from video tutorial.  If you change the custom docker image, you need to build it again (stop container, delete container, delete image, rebuild).  The code challenge was easier than I thought but still can't do it in a single line return statement.  Need to remember that I can use the return value of methods more than I think.

# Day 133 (6/29/2022)

## Codewars and Docker

Learned more about Docker today and did a codewars challenge today.  The challenge was to return sorted string based off a number in the string.

## Thoughts

Learned about building your own docker image using a Dockerfile, pushing to a private repository, deploying through docker, and persisting data through docker volume.  I need to review what I watched today but next step is to practice.  The challenge wasn't too difficult and was able to have a single line return statement.  Saw a solution using key=lambda and need to dig more into that.

# Day 134 (6/30/2022)

## Docker

Practiced Docker commands.

## Thoughts

Got pretty sidetracked but ran some basic docker commands.  Couldn't get the local host working since I don't have GitLab or a template to practice using mongo and mongo express containers.  Learned about windows powershell commands.

# Day 135 (7/1/2022)

## Codewars

The challenge was to return a boolean if three integers make up a triangle.  Tried another challenge before which I had a solution but time complexity failed the solution.

## Thoughts

Had to look up the mathematics for determining if three sides make up a triangle.  Pretty simple.  The other challenge I didn't know how to fix the time complexity issue.

# Day 136 (7/4/2022)

## Codewars

The challenge was to return number of '.' equal to the lengths of each string.

## Thoughts

Did not know how to do this in a one line return statement.  Did the brute force method.  Split the string, find the lengths of each string with '.', used the string version of the math operator and then returned a string created by a for loop using the length gotten from the algebra.  Looking at the other solutions, there an eval() method that parses the expression passed and runs python code.  Cool built in method I didn't know about.

# Day 137 (7/5/2022)

## Docker

Practiced Docker.

## Thoughts

Having a tough time learning Docker.  Tried to follow a written tutorial on the Docker docs but local host wouldn't load.  Need to debug and practice more.

# Day 138 (7/6/2022)

## Docker and Codewars

Tried practicing docker.  Did a codewars challenge.  The challenge was to return the value of a string based off the values the instructions give you.

## Thoughts

Figured out the error is CORS related and not sure how to proceed.  The code challenge was pretty easy.  Could've done a loop and conditionals but decided to create a class and in the class it has a function that returns the value of the string just to practice OOP.

# Day 139 (7/7/2022)

## Docker and Codewars

Tried practicing docker.  Followed another docker guide from the docs.  The codewars challenge was to return the index of the middle number in the list.

## Thoughts

Moved on to another docker docs guide since I can't figure out the CORS issue.  Figured out an authentication issue that I was having because of a single letter misspelling.  Able to create a container and access local host and pushed to remote repository.  Did a way overcomplicated OOP way of solving the problem.  Forgot that there's a sorted() method which sorts the array so you can sort it, and then return the middle index.

# Day 140 (7/8/2022)

## Codewars

Did a code challenge today.  Given a list of list of integers return the difference.

## Thoughts

Could've done a simple one line return statement of summing the difference of a loop that uses the lists in the list but decided to create a class that returns the number of the initial passengers and the leaving passengers in the bus prompt.  Then in the function, returned the difference.

# Day 141 (7/11/2022)

## Docker

Practiced Docker.

## Thoughts

Practiced using a docker volume / database and bind mounts.  Refreshed information on types of volumes.

# Day 142 (7/12/2022)

## Docker

Practiced Docker.

## Thoughts

Practiced with multi container apps and using docker compose.  Get the general idea on how to use it but don't know where to start when containerizing previous projects.

# Day 143 (7/13/2022)

## Docker

Practiced Docker.

## Thoughts

Practiced docker scan, and multi image layering, image caching, .dockerignore.  Read about multi stage builds (Maven/Tomcat, React).  Tried containerizing GA project 1 but not working.

# Day 144 (7/14/2022)

## Docker and Codewars

Practiced Docker.  Did a codewars challenge.  The challenge was to find the largest consecutive 5 digit number in a given number.

## Thoughts

Tried to containerize project 1 but still not working.  Not sure how to proceed so I did a codewars challenge instead.  Did some more OOP practice even though the challenge could be done in a single line.  The single line return statement looked more complicated than I thought but I'm satisfied with my answer since it gave me more OOP practice.

# Day 145 (7/15/2022)

## Docker and Codewars

Practiced Docker.  Did a codewars challenge.  The challenge was to find how many times a number can be divisible by another number.

## Thoughts

Able to containerize project 1.  Changed the dockerfile to something else I found and it worked.  Also, added a docker-compose.yml file so it's now able to be used with docker-compose.  The challenge was very easy.  Did a basic while loop and had a variable to keep track of how many times the number was divided.  One of the solutions has a log() method from the math library. Don't remember too much math so I didn't know that was a solution you could do.  Probably need to do some more challenging challenges.

# Day 146 (7/18/2022)

## Docker

Practiced Docker.

## Thoughts

Able to containerize project 2.  Working on containerizing project 3.

# Day 147 (7/19/2022)

## Docker and Dropbox Assessment test

Practiced Docker and took an assessment test.

## Thoughts

Able to run a container for project 3 but can't seem to get docker-compose to work.  Turns the daemon black and unable to be used.  Can't find anything online about it.  Bombed the assessment test because I'm inexperienced.  Was able to give an answer for 3/4 questions but the rotating and flipping diagonally of a numerical matrix I did not understand.  And even some of the answers I did give weren't good either.  One didn't meet the time complexity test and the other had bugs and didn't finish all the tests.

# Day 148 (7/20/2022)

## Docker

Practiced Docker.

## Thoughts

Tried to create a Dockerfile for Django project.  Could not get it to work.

# Day 149 (7/21/2022)

## Dropbox Assessment

Did an assessment test.

## Thoughts

Good practice but I need to get more.  Barely finished the 1st segment.  Used OOP and created classes with methods to finish segment 1.  Also realized I need to think more about how the code works when I write it.  Wish I had more time and I think if I did I would finisht the assessment but alas it was timed.

# Day 150 (7/22/2022)

## Codewars

Did a codewars challenge.  The challenge was to find the minimum perimeter given an area of a rectangle.

## Thoughts

Ok OOP practice but my solution seemed like it didn't meet the execution time limit.  Not sure the exact reason and not sure how to refactor it.

# Day 151 (7/25/2022)

## Docker

Practiced Docker.

## Thoughts

Able to get a basic Django docker container running.  Have a general idea of what the Dockerfile and docker-compose.yml files are saying/doing but still don't understand when some of the syntax/lines are necessary.  Also, still don't know how to containerize project 3 backend.

# Day 152 (7/26/2022)

## Docker

Practiced Docker.

## Thoughts

Very slow process on how to use docker with Django and PostgreSQL.  Image can build but container can't run.  Still don't know exactly what lines of code is necessary for container to run.

# Day 153 (7/27/2022)

## C#

Practiced C#.

## Thoughts

Docker wasn't going well so I swapped to writing a console app in C#.  Going back to the battleship one from one of the GA assignments.  Forgot how to write code in C# and had to look things up.  Wondering if I should also learn C/C++.

# Day 154 (7/28/2022)

## C#

Practiced C#.

## Thoughts

Finished the GA battleship assignment in C#.  There's a bug that each stat on the alien ship is set to a single random number/double instead of different ones for every alien ship.  Not sure why it's happening or how to fix it.

# Day 155 (7/29/2022)

## Codewars

Did a codewars challenge today.  One was to debug a sum of numbers in an int and the other was to find the minimum number of moves in tower of hanoi depending on the number of disks.

## Thoughts

Redid the bugged solution and was able to get a one line return statement.  Also did a one line return statement for the tower of hanoi as well.  Since I built tower of hanoi I had prior knowledge that there's a mathematical solution to finding the minimum number of moves and was able to do another one line return statement.  Also been practicing in typeracer to get faster but need practice typing code.

# Day 156 (8/1/2022)

## C#

Practiced C#.

## Thoughts

Converted some sorting algorithm code into C#.  There's no spread operator so had to find a workaround.  Didn't test it either so I'm not sure if it works or not and I don't know how to run C# code in the terminal like with node.

# Day 157 (8/2/2022)

## C# and Codewars

Practiced C# and did a codewars challenge.  The challenge was to return the sum of the ascii values for every letter in a string.

## Thoughts

Redid some of the sorting algorithm code to match C#.  Fixed a bug with the space battle c# code.  Turns out that Random is an object and when you create it, it has a lifecycle that is greater than the runtime of the code so it was giving the same value.  Just had to create it once and then pass the object to each method.  The code challenge was very easy once you understood the prompt, it had no directions, just an example, and I was able to get a one line return statement.

# Day 158 (8/3/2022)

## C#

Practiced C#.

## Thoughts

Created a calculator console app following the microsoft docs.  Made an initial commit to create a web app using C#.  It's going to be a web version of the calculator console app.

# Day 159 (8/4/2022)

## C#

Practiced C#.

## Thoughts

Very slow day.  Read that C# is generally not used for front end development but it can do some server side calculations just not sure how to implement that.  Read some basic starter stuff for .NET.  So just translated some data structure stuff into C#.

# Day 160 (8/5/2022)

## Random things

Read a little about .NET, did a codewars challenge, watched some stuff about recursion.

## Thoughts

Need to focus harder.  Did two codewars challenges but only finished one.  The first one was easy, just returning the min value or the index of min value based off an indicator input.  Able to get a one line return statement.  The other challenge was to return a string of numbers depending on if the string has duplicate letters.  For some reason, I cannot think of a solution right now.  It feels like my brain isn't working for some reason.

# Day 161 (8/8/2022)

## Assessment test, Codewars, C#

Did an assessment test for US Senate and a codewars challenge.  The challenge was to return the last element in a list.  Did some C# coding practice.

## Thoughts

The assessment test prompts weren't that difficult.  It was assertions in Python, an API call/tests, and Django/Python serializers and views.  The API call prompt might have been bugged because my new Error() was being read as null instead of the message I put in.  The codewars challenge was actually easy but I still have to look up how to do Python syntax.  Finished writing linked list methods in C#.  Couldn't get the sort method to work but all the other methods do.  It's pretty cool writing code in C#.

# Day 162 (8/9/2022)

## C#

Did random reading and initial commit for restarting calculator app.

## Thoughts

This will not be a web application but rather a form application using Visual Studio's window form app template.  Will need to fiddle around with how things will interact with each other and to see if it can be deployed but one step at a time.

# Day 163 (8/10/2022)

## C#

Added stuff to calculator app.

## Thoughts

Having trouble with the logic.  Added the base amount of buttons for numbers and operations.

# Day 164 (8/11/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return a string based off of the array of chars in the input array.

## Thoughts

Don't know why I had trouble with this.  Tried to do two for loops but my mind had trouble thinking of something.  Ended up doing a while loop and a for loop.  Had an array of strings that I joined and returned the result.  Probably need more critical thinking exercises.

# Day 165 (8/12/2022)

## C#, Codewars

Added to the calculator app.  Did a codewars challenge today.  The challenge was to return the area of a triangle inside a rectangle/square.

## Thoughts

Finally made progress on the calculator app.  Able to get basic calculator functionality but still needs a little more error checking.  Will add more features later.  The code challenge was very easy because the triangle in the rectangle/square is set based off the diagonals of the encompassing rectangle/square.  All I needed to do was find the formula for the area of a triangle and then divide the height of the rectangle/square by 2 and plug it in to the formula.

# Day 166 (8/15/2022)

## C#

Worked on the calculator app.

## Thoughts

Fixed a lot of bugs in the caluclator app.  Added some functionality but now it's causing some bugs and not sure how to fix.  Will continue to work on this application.

# Day 167 (8/16/2022)

## C#

Worked on the calculator app.

## Thoughts

Added some features on the calculator app.  Added a divde into 1, square, square root, and fixed more bugs.

# Day 168 (8/17/2022)

## C#

Worked on the calculator app.

## Thoughts

Slow progress on the application.  Fixed some bugs and adjusted code logic.  Wanted to add a delete button but realized that I need to then change how the display works.

# Day 169 (8/18/2022)

## C#

Worked on the calculator app.

## Thoughts

Redid the display and operand/operand display logic.  Added a backspace feature.  Redid the visual layout to make it look better.  Achieved basically the same functionality as a standard calculator app on a computer.

# Day 170 (8/19/2022)

## Calculator app deploy and Codewars

Worked on the calculator app.  Did a codewars challenge.  The challenge was to replace instances of a char with another char in a string and return it.

## Thoughts

Published the application and now is a .exe file.  Once the repository is cloned, the user can navigate to the path listed in the README.md and will be able to open the application.  The codewars challenge was really easy but I didn't do it the Python way.  The one line return statement used maketrans().  Didn't know that method existed.

# Day 171 (8/22/2022)

## Codewars and Docker review

Read some Docker and Microsoft docs and did a basic review.  Did a codewars challenge.  The challenge was to create a string that prints out a square with height and width the same as the input integer.

## Thoughts

The documentation that I read was for using Docker with MS applications but it was mainly review which seems like a good sign.  For the code challenge, did a simple nested for loop and was able to solve the code challenge.  There were other interesting solutions like using .joing() and another solution where you can use ('i' * n) and it will create a string with repeating char/string just like a for loop.

# Day 172 (8/23/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return the sum of a list but ignore duplicates.

## Thoughts

Able to do a single line return statement.  Used the sum() method and did a for loop in a list with a conditional that determines if the element in a list is a duplicate.

# Day 173 (8/24/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return a number based on a comparison of two exponents.

## Thoughts

Ran into execution timeouts because of the very large integer inputs/exponents.  Used a log() method and it computed way faster.  Looks like I need to go back and learn math.

# Day 174 (8/25/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return the unique number in a list.

## Thoughts

This was another challenge that had a runtime limit because it had large lists.  Turned the initial list input as a set and did a conditional to return the proper number.  Could've done it better but figured out a jenk way of doing it.

# Day 175 (8/26/2022)

## Codewars

Did a codewars challenge today.  The challenge was to return the largest integer between a range that's divisible by one of the input integers.

## Thoughts

Did a basic for loop and conditional.  There're solutions that are 1-2 lines long and I didn't know that there's basically a formula to solve this challenge.

# Day 176 (8/29/2022)

## Kubernetes

Started to learn about Kubernetes.

## Thoughts

Learned about the use of Kubernetes and why it is used, basic structure of kubernetes, and commands from the kubectl command list.  Kubernetes is a container orchestration tool which emphasizes the usage of containers and microservices over monolith design.  It is made up of master nodes and worker nodes.  The master node contains the important processes that enable kubernetes like the api server(entrypoint), scheduler(where to put pods), controller manager(manage the status of nodes), and the etcd(key value storage/database backup for cluster).  The worker nodes contain pods which are abstractions over containers, each pod has a service so the pods can communicate with each other, container runtime which run the containers(docker) and the worker node commands(kubelet), ConfigMap(external configuration of application), and Secret(used to store secret data/environmental variables).  Minikube is a software that "containerizes" the master and worker node in one node to run it on a machine.  Kubectl is the command line commands that you can run on the terminal to execute the master node processes.  Also, went over the CRUD functionality of kubectl and learned about deployments, pods, replicasets, logs, and editing deployment yaml files.

# Day 177 (8/30/2022)

## Kubernetes

Continue to learn about Kubernetes.

## Thoughts

Practiced building a mongo and mongo-express app using Kubernetes.  Worked through the yaml files to create deployments of a mongo application.  Ran into an authorization issue while adding mongo-express.  Currently cannot solve the issue.

# Day 178 (8/31/2022)

## Kubernetes

Continue to learn about Kubernetes.

## Thoughts

Finished the video walkthrough for Kubernetes demo.  There's A LOT of information that I need to review.  But the mongo and mongo-express app that wasn't working yesterday started working without any kind of intervention and was able to start the service.  It seems like a lot of Kubernetes is breaking large applications into smaller pieces and having those pieces be able to communicate with each other.  Kubernetes doesn't inately handle stateful data so the user needs to create a persistent volume (which is a similar name that Docker has) and then attach the volume to the pods.  And as the application contains more services, it seems like it's best practice to try to keep everything separate to avoid any kind of mixups.  There's also a lot of information on using ports and IP addresses, whether it's from an external service like Ingress or an internal service.  Still lots to learn but I'm willing to keep diving in.

# Day 179 (9/1/2022)

## Kubernetes and C

Reviewed some Kubernetes and started to relearn C.

## Thoughts

Worked on volume yaml files in Kubernetes and started to relearn C.  Started using VIM and will eventually get around to learning the tool later but decided to continue learning C using Code Block.  Much easier IDE to work with.

# Day 180 (9/2/2022)

## Codewars

Did a codewars challenge today.  The challenge was to compare "version numbers" and see which one is most up to date.

## Thoughts

Solved it by creating a class with methods to check for any edge cases like array lengths and converting to integers.  Then created a method that looped through two arrays that contain the version numbers and then returned a boolean.  It was overly complicated but it gave me some decent practice with OOP.  Did not realize that you can literally compare two arrays using comparison operators and it will compare every value like a loop does.

# Day 181 (9/5/2022)

## C

Continued learning about C.

## Thoughts

Pretty much all review from what I already knew to it seems like a good sign.  The things I need more refresher on is string manipulation, pointers, and other more advanced topics.  Had a little trouble with using scanf() and fgets() which means I need more practice using those methods.

# Day 182 (9/7/2022)

## Pointers and codewars

Did a refresher on pointers and did a codewars challenge.  The challenge was to return a list of the input string but with a capitalized letter starting from the beginning of the string.

## Thoughts

Pointers seems confusing but it seems like a thing that you just get better at the more you're exposed to it.  For the codewars challenge, just did a basic for loop and then had to look up how to capitalize the nth letter but also keep the original string so I found a solution on stack overflow.

# Day 183 (9/8/2022)

## Pointers

Learned about pointer arithmetic, pointers to pointers, and function call by reference/value.

## Thoughts

Did not realize you can use arithmetic on pointers since they were addressses instead of integer values.  The arithmetic uses bytes instead of int values.  Knew pointers to pointers existed but didn't have too much experience with it.  Now it's been more de-mystified so I'm starting to feel more comfortable with pointers.  And finally, I didn't realize in C that you cannot pass variables to functions and have it reference the value of that variable (example of call by value) and instead you need to pass a pointer to said variable (call by reference).