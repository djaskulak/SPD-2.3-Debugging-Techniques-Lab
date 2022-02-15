# Debug Log

**Explain how you used the the techniques covered (Trace Forward, Trace Backward, Divide & Conquer) to uncover the bugs in each exercise. Be specific!**

In your explanations, you may want to answer:

- What is the expected vs. actual output?
- If there is a stack trace, what useful information does it contain?
- Which technique did you use, on which line numbers?
- What assumptions did you have about each line of code, and which ones were proven to be wrong?

_Example: I noticed that the program should show pizza orders once a new order is made, and that it wasn't showing any. So, I used the trace forward technique starting on line 13. I discovered the bug on line 27 was caused by a typo of 'pzza' instead of 'pizza'._

_Then I noticed another bug ..._

## Exercise 1

- What was supposed to happen was order was supposed to be placed into our server. But I instead received an error with my server.
- If there is a stack trace, what useful information does it contain?
Looking at the stack trace there was an error in the pizza_order_submit area.
- We added print statements to see what was being passed and what wasn’t.
- After a ton of review, it turns out it was an error with the topping for a loop. Once we changed the variable there and committed it to our DB this program worked.

## Exercise 2

For this exercise, we were supposed to input our city and temp type and then get back that information.
BUT. This didn’t work, there were errors all over.
To fix this we needed to make sure our strings were set to correct. I needed to make sure we changed our URL into an f string to pass through our city.
Then it was reviewed what we set our variables as to get them working with HTML (user city, and temp). From here it worked!

## Exercise 3

For this exercise, it took me some time to go over each util because they each had some code that was slightly off. For the merge sort, there was an error with where one of our pointers. To fix this we changed it from looking at the index of the right by I to the index of j. For binary search, we needed to pay close attention to the error we got. On that line, we see there was something with the division. Taking a closer look we see that we were doing floating division when we needed integer division. This was accomplished by adding a second slash.
