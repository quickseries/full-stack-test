# Instructions

1. Fork this repo to your work station.
2. Answer the following questions by creating a JavaScript file for each of the questions.
3. Commit and push your code to your fork.
4. Create a pull request back to the master branch of the origin repo.

# Questions

1. Create a function that takes an unlimited amount of number parameters, and returns an array of all the permutations possible. For example, `myFunction(4, 7, 2) {}` should return `[472, 427, 724, 742, 247, 274]`.

2. Create a function that can find the Nth smallest number in an array. The array can be very very big, so you are not allowed using the `Array.sort()` method. Try to build a function that would perform fast. Also, explain why using `Array.sort()` isn't a good idea when sorting large arrays.


# Answers

2. `Array.sort()` In the case of V8, it implement some variation of quicksort by adding some use cases to prevent worst case scenarios and this increase the complexity of this function(More than O(n power 2)).
For short arrays (length <= 10), V8 use insertion sort.
And for this reason all the native algorithms(in our case sorting) need to handle a big amount of edge cases and this will make the peroformance worse.


# Install & Test

npm i
npm test (it will take about 20 seconds, because of the test of sort performance)