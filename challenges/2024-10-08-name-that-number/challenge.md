# Name That Number

User experience! At least, that's what your project manager told you when they introduced this user story. "As a user, I need to be able to read all numbers displayed in the application as English words without needing to translate them myself." Seems like a bit of unnecessary hand-holding to you, but all you get to vote on is how many story points this feature will be worth. Oh well, at least it's a good opportunity to practice your TDD on company time. For this task, you'll need to write a function that takes in a six-digit number and returns its string representation as English words. For example, `578119` becomes `"five hundred and seventy eight thousand one hundred and nineteen"`.

## Business Rules/Errata

- The input will always contain exactly six digits, but it may include leading zeroes (such as `00149723`).
- The output will only contain words separated by spaces, no hyphens.
- The ten's or ten thousand's place may consist of two words (`34` as `"thirty four"`) or one word (`12` as `"twelve"`).
- Numbers with at least three digits will include the word "hundred", for example `450` as `"four hundred and fifty"`.
- Numbers with at least four digits will include the word "thousand", for example `2861` as `"two thousand eight hundred and sixty one"`.

## Examples

```
NameNumber(000000) -> "zero"
NameNumber(010101) -> "ten thousand one hundred and one"
NameNumber(500020) -> "five hundred thousand and twenty"
NameNumber(123456) -> "one hundred and twenty three thousand four hundred and fifty six"
```

## Tackling This Challenge

1. Make sure you've got the required software on your machine: .NET SDK 8.0+
1. If you haven't already, fork the CodingDojo repository ([INSTRUCTIONS](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo)).
1. Checkout a new branch using `git checkout -b yourgithubusername-wip`.
1. Add your code to the solution file to make the puzzle function work as expected.
1. Confirm your solution by running tests. Execute the `run-tests` script (use `./run-tests` from the challenge root directory.
1. If you've passed all the tests, the `run-tests` script with help you commit it. Otherwise, try again to pass all tests.
1. Navigate to [GitHub](https://github.com/codeconnector/CodingDojo), and submit your pull request.
1. One of the CodingDojo maintainers will help you get your PR merged.

## Requirements

- .NET SDK 8.0+