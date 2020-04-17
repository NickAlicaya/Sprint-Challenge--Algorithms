#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)  0(n) The runtime is O(n)  because it is a loop and the run time of depends on the value of n. Since it is a loop if the value of 'n is small then it will be very short. If the value of 'n' is bigger'the value added to 'a' while it satisfies the while  condition is constant.

    <!-- Constant time means the running time is constant, it’s not affected by the input size.
    code starts at 'a' value zero -->
        while(LOOP) that number is less than N^3
            a's value increases by N^2
            a CONSTANT value of N^2 keeps getting added per iteration until the value of 'a' is not less than N^3



b) 0(n^2) because it is a nest for loop

logn for everytime J is doubled sum is increased by 1. Hence J is the log of sum
TO what power(sum) to you raise 2 to get to the value of J

sum is constant 
loop is 0(n)



c) O(n) 
      recursive because it has a base case
      it calls itself
      value changes towards itself
      <!-- The first function is being called recursively n times before reaching base case so its O(n), often called linear. -->
      its complexity depends on 'n'
  0(2n) or O(n) first it executes the recursive call for bunnies value until it hits zero 
  then it repeats an iterative of +2 for the same number of bunnies

## Exercise II

<!-- Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution. -->

We will use Binary search for this:
The 1st floor will be the beginning while the nth(last) floor will be the end. 
step 1 Go to the middle floor between the 1st floor and nth floor and then drop an egg.
step 2 If the egg breaks consider that the floor is too high and move to the middle floor between the first floor and your current position(the middle of the tower). Drop an egg again
step 3 Else if the egg does not break consider that the current floor is too low and move to the middle floor between my current position and the top or nth floor. Drop an egg again
step 4  Continue steps 2 or 3 moving up or down the middle position relative to your current location. Essentially dividing the number of floors each time to narrow the search range. Continue doing this until you are at the floor where dropping the egg doesn't break it  AND if you only go up one level(f level) it breaks the egg. This is the floor under f.
step 5 Else if you cannot find any floor where the egg doesn't break after dropping it, the floor doesnt exist.


