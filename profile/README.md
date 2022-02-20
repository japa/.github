Japa is an API-first testing framework. It focuses only on testing Node.js (backend) applications, thus resulting in a fast, small, and simple tests runner.

In this guide, we will go through the Japa features and learn about the rationale behind the project.

## Features
Despite being a small and a simple tests runner, Japa has a ton of features you expect from a great testing framework. It includes:

- Support for [test groups](https://japa.dev/grouping-tests), timeout, todo tests and [regression tests](https://japa.dev/underlying-test-class#fails).
- Support for [Datasets](https://japa.dev/datasets).
- Assertion libraries with support for [assertion planning](https://japa.dev/assertion-planning).
- Ability to [filter](https://japa.dev/filtering-tests) and run specific or only failing tests.
- Re-imagined [lifecycle hooks](https://japa.dev/lifecycle-hooks).
- Multiple [reporters](https://japa.dev/plugins/spec-reporter) to display tests progress.
- Great CLI experience with pretty diffs and formatted error stacks.
- Works with **ESM** and [TypeScript](https://japa.dev/usage-with-typescript) both with zero additional setup.

## Why Japa?
There are many testing frameworks available in the JavaScript ecosystem. So let's explore what makes Japa different.

### Node only
Most mainstream testing frameworks in JavaScript are heavily influenced by the frontend ecosystem, or we can say they are frontend first.

Even though JavaScript can run almost everywhere, the needs and approaches of different ecosystems do vary. For example:

- Jest, process all of your source files through the `@jest/transform` package, which uses `babel-jest` internally by default. Also, you can register additional transformers for TypeScript, Vue, and so on.
- Similarly, Vitest uses Vite under the hood for code transformation.

The code transformation layer is not at all required when writing backend applications for Node.js. **So why pay the penalty of doing so?**

Also, much community effort goes into creating plugins/extensions required by frontend applications. Whereas with Japa, we focus on **growing the ecosystem around the needs of backend testing**.

To conclude, I am not saying Jest or Vitest are technically inferior. It's just Node.js deserves its own first-class testing experience.

### Extensible
Japa is extensible to its core. Not only you can create **plugins** and **reporters** for Japa, you can also extend the [Test](https://japa.dev/underlying-test-class#extending-test-class), [TestContext](https://japa.dev/test-context#adding-custom-properties-to-the-context), and [Group](https://japa.dev/grouping-tests) classes to add additional behavior.
