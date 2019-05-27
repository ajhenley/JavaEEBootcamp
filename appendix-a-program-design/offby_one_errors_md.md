# Fencepost Problem and Off-By-One Errors

An off-by-one error \(OBOE\) is a logic error. It occurs in computer programming when an iterative loop iterates one time too many or too few.

This problem may arise when the programmer uses "is less than or equal to" instead of "is less than". It also happens when one fails to take into account that a sequence starts at zero rather than one.

In Java, arrays start at 0. The first element is also known as the 0th element.

Imagine you are building a fence. How many fenceposts do you need? How many gaps exist between fenceposts?

As shown below, there are five fence posts but they only span four rails. Or, put differently, if you wish to span four rails you need to buy five posts. If you count the first post as 0 then the last post matches the number of rails.

\|-\|-\|-\|-\|

