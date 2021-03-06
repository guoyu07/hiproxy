# Contributing
We are open to, and grateful for, any of your contributions.  By contributing to HiProxy, you agree to abide by the [code of conduct](https://github.com/hiproxy/hiproxy/blob/master/CODE_OF_CONDUCT.md).

## Reporting Issues and Asking Questions
Before opening an issue, please search the [issue tracker](https://github.com/hiproxy/hiproxy/issues) to make sure your issue hasn't already been reported.

## New Features
Please open an issue with a proposal for a new feature or refactoring before starting on the work. We don't want you to waste your efforts on a pull request that we won't want to accept.

## Contribution Content
Hiproxy is currently under development, you can choose the following content to contribute:

1. **Features**: add new features for hiproxy, such as new commands, directives and new pages.
2. **Documentation**: At present, hiproxy's documentation is not perfect, you can first understand the use of hiproxy, and then write the usage documentation or technical documentation. Now many documents are Chinese version, you can also help translate into English version.
3. **Test**: At present, hiproxy's test case is not perfect, there are many test cases missing, you can first understand the use scenes of hiproxy, and then write the test.
4. **Website**: hiproxy currently does not have its own domain name and website, you can help hiproxy design or develop a website.

## Code Style

hiproxy use [semistandard](https://github.com/Flet/semistandard) code style. The main rules:

- **semicolons**
- **2 spaces** – for indentation
- **Single quotes for strings** – except to avoid escaping
- **No unused variables** – this one catches *tons* of bugs!
- **Never start a line with `(`, `[`, or `` ` ``**
  - This is the **only** gotcha with omitting semicolons – *automatically checked for you!*
  - [More details](https://github.com/feross/standard/blob/master/RULES.md#semicolons)
- **Space after keywords** `if (condition) { ... }`
- **Space after function name** `function name (arg) { ... }`
- Always use `===` instead of `==` – but `obj == null` is allowed to check `null || undefined`.
- Always handle the node.js `err` function parameter
- Always prefix browser globals with `window` – except `document` and `navigator` are okay
  - Prevents accidental use of poorly-named browser globals like `open`, `length`,
    `event`, and `name`.
    
For more details, check <https://github.com/feross/standard>

## Test

Before you submit a pull request. You should pass the auto test case. And if you change some code, you should also add new test case for the changed code or function.

You can use the following command to perform the test:

```
npm test
```

## Steps for Contributing
1. [Create an issue](https://github.com/hiproxy/hiproxy/issues/new) for the bug you want to fix or the feature that you want to add.
2. Create your own [fork](https://github.com/hiproxy/hiproxy) on github, then checkout your fork.
3. Write your code in your local copy. It's good practice to create a branch based off the `master` branch for each new issue you work on, although not compulsory.
4. To run the test suite, first install the dependencies by running `npm install`, then run `npm test`.
5. If the tests pass, you can commit your changes to your fork and then create a pull request from there. Make sure to reference your issue from the pull request comments by including the issue number e.g. `#123`.

Please try to keep your pull request focused in scope and avoid including unrelated commits.

After you have submitted your pull request, we'll try to get back to you as soon as possible. We may suggest some changes or improvements.

Thank you for contributing!


