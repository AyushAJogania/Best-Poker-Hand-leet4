# Best-Poker-Hand-leet4


**Problem Description**__
You are given an integer array ranks and a character array suits. Each element in ranks represents the rank of a card, and each element in suits represents the suit of a card. The ranks and suits are provided in reverse order, with the first element corresponding to the last card.

Your task is to determine the best type of poker hand that can be made from the given cards and return it as a string. The possible hand types, from best to worst, are:

"Flush": Five cards of the same suit.
"Three of a Kind": Three cards of the same rank.
"Pair": Two cards of the same rank.
"High Card": Any single card.
Note that the return values are case-sensitive.


**
_Example**___

Input: ranks = [4, 4, 2, 4, 4]
suits = ['d', 'a', 'a', 'b', 'c']
Output: "Three of a Kind"


_**Explanation:**___

The given hand consists of cards with ranks [4, 4, 2, 4, 4] and suits ['d', 'a', 'a', 'b', 'c']. There are three cards with rank 4, which satisfies the condition for "Three of a Kind". Hence, the output is "Three of a Kind".


_**Approach**_

To solve this problem, we can use a sequential approach to check the conditions and determine the best hand type. Here's the step-by-step approach:

Count the occurrences of each rank and suit in the given cards.
Check if there is a "Flush" by verifying if there are five cards of the same suit.
Check if there is a "Three of a Kind" by verifying if there are three or more cards of the same rank.
Check if there is a "Pair" by verifying if there are two or more cards of the same rank.
If none of the above conditions are met, consider it as a "High Card".
By sequentially checking these conditions, we can determine the best hand type for the given cards.


_**Time Complexity Analysis**_

The time complexity of this solution is O(n), where n is the number of cards in the input. This is because we iterate through the ranks and suits arrays to count the occurrences and perform the necessary checks.

**_Space Complexity Analysis_**

The space complexity of this solution is O(m), where m is the number of unique ranks or suits in the input. We use two unordered maps to store the count of ranks and suits, which can have a maximum size of the unique ranks or suits present in the input.

_**Summary**_

The "Best Hand in Poker" problem asks us to determine the best type of poker hand that can be made from a given set of cards. By counting the occurrences of ranks and suits and sequentially checking the conditions, we can identify the best hand type. This solution has a time complexity of O(n) and a space complexity of O(m), where n is the number of cards and m is the number of unique ranks or suits.
