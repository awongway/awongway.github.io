---
layout: project
type: project
image: images/ factor.png
title: "Sum of Even Factors"
date: 2017-09-06
labels:
  - Java
  
summary: This was the first assignment for ICS 314
---

Here is my sample code:

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

