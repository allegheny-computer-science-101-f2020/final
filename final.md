# CMPSC 101 Final Exam

## Your Name

**1\. [5 points]** State two key differences between an iterative and recursive data processing technique.

TODO

**2\. [12 points]** A software engineer must assess the trade-offs associated with using different data structures inside of a Java program. Answer the following questions by comparing the following data structures in these pairs, highlighting the strengths and weaknesses of each data structure.

- (a) `Array` compared to `ArrayList`

  TODO

- (b) `ArrayList` compared to `SinglyLinkedList`

  TODO

- (c) `SinglyLinkedList` compared to `DoublyLinkedList`

  TODO

**3\. [6 points]** You could use a `java.util.TreeMap` to effectively perform a "word counting" operation as we did in practical 8\. Answer the following questions about the implementation of a `WordCount` program.

- (a) What is the input of the `WordCount` program?

  TODO

- (b) What is the output of the `WordCount` program?

  TODO

- (c) How does the `WordCount` program use a `TreeMap`?

TODO

**4\. [12 points]** Give three examples of a reference data type (i.e., an Object), explaining the purpose of each and showing how to construct it by calling one of its constructors.

TODO

**5\. [10 points]** The code given below implements a factorial function.

```
public static int factorial(int n) {
   if(n < 0)
      throw new IllegalArgumentException();
   if (n == 0)
      return 1;
   else
      return n * factorial(n - 1);
}
```

- (a) Perform a "recursion trace" to explain the Java method calls that would take place if a main method called this method with the input of `4`. That is, show each step of the method execution, including each recursive call with input argument until it reaches the base case.

  TODO

- (b) What is the worst case time complexity of the `factorial` method?

  TODO

**6\. [12 points]** It is possible to implement an `ArrayList` that contains `n` elements and is realized by a fixed-size array. Using the big-Oh notation, furnish the worst-case time complexity for the following `ArrayList` methods. Provide justification for the chosen worst-case time complexity.

- (a) `size()`

  - Worst-Case Time Complexity: TODO
  - Justification: TODO

- (b) `get(i)`

  - Worst-Case Time Complexity: TODO
  - Justification: TODO

- (c) `add(i,e)`

  - Worst-Case Time Complexity: TODO
  - Justification: TODO

- (d) `remove(i)`

  - Worst-Case Time Complexity: TODO
  - Justification: TODO

**7\. [12 points]** The code below processes an array and runs a method that does something mysterious. Answer the questions below based on this code. Hint: The key idea of recursion is break down the problem into series of sub-problems. Note the base case and recursive case indications in the comments.

```
/** Mystery Class.
*/
public class Mystery {

  /** doMystery method that does something mysterious.
  */
  public static int doMystery(int[] array, int num1, int num2) {
    if (array.length - num1 == -1) { //base case
      return num2;
    } else { // recursive case
      if (array[array.length - num1] > num2) {
        num2 = array[array.length - num1];
      }
      return doMystery(array, num1 + 1, num2);
    }
  }

  /** main method to call doMystery method.
  */
  public static void main(String[] args) {
    int[] array = {10, 18, 5, 17, 3};
    int output = doMystery(array, 1, 0);
    System.out.println(output);
  }
}
```

- (a) What does a `doMystery` method do in general terms, that is, what is its function?

  TODO

- (b) What is the output of `Mystery` program?

  TODO

- (c) Does the `Mystery` program function the same way if we change the base case to `if (array.length - num1 == 0)`. Explain your answer.

  TODO

**8\. [5 points]** ( **True or False.**) The order of growth tells us by which factor to expect the running time to increase.

TODO: Put "X" inside brackets [ ] of the correct answer.

- [ ] True.
- [ ] False.

**9\. [5 points]** Two algorithms, `Alg1` and `Alg2`, which solve the same problem, are analyzed, and it is found that `Alg2`'s asymptotic running time is greater than `Alg1`'s. What prediction can be made regarding the algorithms' running times?

TODO: Put "X" inside brackets [ ] of the correct answer.

- [ ] No prediction can be made without knowing the hardware and software used for testing.
- [ ] As the size of the input data increases, `Alg2` is more and more likely to run faster than Alg1.
- [ ] As the size of the input data increases, `Alg1` is more and more likely to run faster than `Alg2`.
- [ ] `Alg1` and `Alg2` have the same running times.

**10\. [10 points]** It is possible to implement a `Map` using unsorted list. Using the big-Oh notation, furnish the requested time complexity for the following `Map` abstract data type methods. Justify your responses.

- (a) `put` method

  - Worst-Case Time Complexity: TODO
  - Justification: TODO

- (b) `get` method

  - Worst-Case Time Complexity: TODO
  - Justification: TODO

**11\. [5 points]** What is the worst time complexity to add a node at the end of singly linked list, if the pointer is initially pointing to the head of the list?

TODO: Put "X" inside brackets [ ] of the correct answer.

- [ ] `O(1)`
- [ ] `O(n)`
- [ ] `O(log n)`
- [ ] `O(n^2)`

**12\. [6 points]** Name three new things you learned in this class.

TODO
