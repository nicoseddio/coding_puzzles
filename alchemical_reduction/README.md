_taken from https://programmingpraxis.com/2019/09/10/alchemical-reduction/_


# Alchemical Reduction
### September 10, 2019

Today’s exercise is from the 2018 Advent of Code, Day 5:

You’ve managed to sneak in to the prototype suit manufacturing lab. The Elves are making decent progress, but are still struggling with the suit’s size reduction capabilities.

While the very latest in 1518 alchemical technology might have solved their problem eventually, you can do better. You scan the chemical composition of the suit’s material and discover that it is formed by extremely long polymers (one of which is available as your puzzle input).

The polymer is formed by smaller units which, when triggered, react with each other such that two adjacent units of the same type and opposite polarity are destroyed. Units’ types are represented by letters; units’ polarity is represented by capitalization. For instance, r and R are units with the same type but opposite polarity, whereas r and s are entirely different types and do not react.

For example:
– In aA, a and A react, leaving nothing behind.
– In abBA, bB destroys itself, leaving aA. As above, this then destroys itself, leaving nothing.
– In abAB, no two adjacent units are of the same type, and so nothing happens.
– In aabAAB, even though aa and AA are of the same type, their polarities match, and so nothing happens.
Now, consider a larger example, dabAcCaCBAcCcaDA:
1. dabAcCaCBAcCcaDA  The first 'cC' is removed.
1. dabAaCBAcCcaDA    This creates 'Aa', which is removed.
1. dabCBAcCcaDA      Either 'cC' or 'Cc' are removed (the result is the same).
1. dabCBAcaDA        No further actions can be taken.
After all possible reactions, the resulting polymer contains 10 units.

How many units remain after fully reacting the polymer you scanned?

# My Solution(s)
**Python:** run with `python3 alchemical_reduction.py`
