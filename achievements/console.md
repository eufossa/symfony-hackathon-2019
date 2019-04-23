# Symfony Console achievements

We fixed some bugs in the Symfony Console component including:

- [STTY not reset when aborting in QuestionHelper::autocomplete()](https://github.com/symfony/symfony/pull/30883)
- [Inconsistent result for choice questions in non-interactive mode](https://github.com/symfony/symfony/pull/30878)
- [Broken formatting of Table that has a trailing backslash](https://github.com/symfony/symfony/pull/30911)
- [Inability to run most tests independently from each other](https://github.com/symfony/symfony/pull/30986)

We also started to think about how we could refactor the current word-wrapping algorithm
which has some known design issues.
The fact that the core team members and contributors met helped a lot to move forward.
