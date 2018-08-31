---
layout: project
type: project
image: images/ factor.png
title: "Sum of Even Numbers"
date: 2017-09-06
labels:
  - Java
  
summary: This was the first assignment for ICS 314
---
This was the fist assignment for ICS. What we needed to do was create a function that took a positive number and make it our limit. From there it would create a pattern where the third number would be equal to the two previous numbers and so on. The limit we put in our function would be where it stopped. After it stops the function finds the sum of all the even numbers in the list of numbers.

Here is my sample code:

```
function projectEulerTwo(limit) {

  let prev = 1;
  let curr = 2;
  let sum = 0;

  while (curr < limit) {
    if ((curr % 2) === 0) {
      sum += curr;
    }
    let next = prev + curr
    prev = curr;
    curr = next;
  }

  return sum;
}

console.log( projectEulerTwo(4000000));
```
