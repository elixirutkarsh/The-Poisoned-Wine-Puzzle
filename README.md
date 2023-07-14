# The-Poisoned-Wine-Puzzle
Problem Statement:
You are a king and have 1000 bottles of wine. One of the bottles is poisoned, and anyone who drinks even a little amount will die within 24 hours. You have 10 prisoners whom you can use to test the wine. However, you don't want to sacrifice all the prisoners, and you want to identify the poisoned bottle in as few tests as possible. How can you determine which bottle is poisoned using the minimum number of prisoners and tests?

Solution:
To solve this puzzle, you can assign each bottle a unique number from 1 to 1000. Convert the numbers to binary form and let the prisoners drink from the bottles corresponding to the positions of the 1s in their binary representation. For example, prisoner 1 drinks from all bottles where the least significant bit of the number is 1 (i.e., 1, 3, 5, 7, ...). Prisoner 2 drinks from bottles where the second least significant bit is 1 (i.e., 2, 3, 6, 7, ...), and so on.

After 24 hours, only the prisoners who drank from bottles with the poisoned one will die. By looking at the pattern of dead prisoners, you can convert it back to binary representation to determine the bottle number. This solution guarantees that you can identify the poisoned bottle using only 10 tests (equal to the number of prisoners) instead of testing each bottle individually.
