# Big O Assessment

 ### O Boy! It's time to evaluate your understanding of Big O Notation!

 ##

  PART ONE: Please answer the following questions:

 1. Describe the purpose of Big 0.

    > Big O is a mathematical notation describing the efficiency of a function at a particular value.

---


 2. What 2 things does it measure?

    > time and space.

---


 3. Which of the following shows Big O time complexity in order?

    a) O(1), O(n log n), O(log n), O(n), O(n^2)

    b) O(1), O(log n), O(n), O(n log n), O(n^2)

    c) O(1), O(log n), O(n log n), O(n), O(n^2)

    > B is the answer.

---



4. Which of these algorithm(s) run in O(log n) time?

   Binary Search

   Bubble Sort

   Quick Sort (average case)

   Linear Search

   > Binary search runs in O(log n) time.

---



5. Select the best time complexity that even the most efficient sort algorithm can have.

    O(log n)

    O(n log n)

    O(n)

    O(n^2)

    > O(n) is the best time complexity that sorting algorithms can have. In this list O(log n) is faster, however it is generally used for searching rather than sorting.

---


 6. Describe what sets these these 3 complexities apart from each other: O(1), O(n) and O(n^2)

    > O(1) - Constant - takes the same amount of time regardless of input size because only one operation is performed.
    O(n) - linear - running time increases proportionally to the size of input.
    O(n^2) - quadratic - running time increases as the square of the size of input.

---


7. How would you recognize O(log n) and O(n log n) time complexities in a function?

    > O(log n) functions are divide and conquer algorithms such as binary search. They keep dividing sorted data in half to quickly get a result. They have logarithmic time complexity, which is really good in terms of time complexity and on par with O(1).

    > With O(n log n) functions, on the other hand, data is divided in half and each half is processed again independently using recursive functionality. These functions are good for sorting. O(n log n) has a time complexity higher than O(log n) because it has to run more operations (using both of their worst to compare) to achieve its goals.  

---

  ##

  PART TWO: In a new file, write examples of algorithms/functions for each of the Big O complexities below.
    Upload your file to your repository when complete and submit in Learn --> Exercises.

    1. O(1)

    const getLast = (items) => {
       return items[items.length-1];
    };

    2. O(n)

  const findIndex = (items, match) => {
    for (let i=0, total=items.length; i < total; i++) {
      if (items[i] == match)
         return i;
         }
   return -1;
    };

    3. O(n^2)

    const buildSquareMatrix = (items) => {
   let matrix= [];
   for (let i=0, total=items.length; i < total; i++){
      matrix[i] = [];
      for (let j=0, total=items.length; j < total; j++)
         matrix[i].push(items[j]);
   }
   return matrix;
};
