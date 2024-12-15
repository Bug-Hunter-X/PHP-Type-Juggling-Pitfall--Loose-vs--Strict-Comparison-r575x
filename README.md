# PHP Type Juggling Pitfall: Loose vs. Strict Comparison

This repository demonstrates a subtle but important difference in PHP's comparison operators: loose (`==`) versus strict (`===`).  The example showcases how loose comparison can lead to unexpected behavior when comparing strings and integers, potentially resulting in logic errors.

## The Problem

PHP's loose comparison (`==`) performs type juggling.  If you compare a string that looks like a number with a numeric value, PHP will automatically convert the string to a number before comparison.  This can lead to unexpected results if you are not aware of this behavior. Strict comparison (`===`), on the other hand, checks for both value and type equality.

## How to Use

1. Clone the repository.
2. Run `bug.php` to observe the unexpected behavior.
3. Examine `bugSolution.php` to see how to avoid this issue using strict comparison.