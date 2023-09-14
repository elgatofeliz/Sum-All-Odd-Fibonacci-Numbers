# Sum-All-Odd-Fibonacci-Numbers

    JavaScript Algorithms and Data Structures
    Intermediate Algorithm Scripting

Sum All Odd Fibonacci Numbers

Given a positive integer num, return the sum of all odd Fibonacci numbers that are less than or equal to num.

The first two numbers in the Fibonacci sequence are 0 and 1. Every additional number in the sequence is the sum of the two previous numbers. The first seven numbers of the Fibonacci sequence are 0, 1, 1, 2, 3, 5 and 8.

For example, sumFibs(10) should return 10 because all odd Fibonacci numbers less than or equal to 10 are 1, 1, 3, and 5.

--- Here's the Code ---

function sumFibs(num) {

  let previousNumber = 0
  let currentNumber = 1
  let result = 0
  
  while(currentNumber <= num){
    if(currentNumber %2 !== 0){
    result += currentNumber
    }
  currentNumber += previousNumber
  previousNumber = currentNumber - previousNumber
  }
return result
}

sumFibs(4);
