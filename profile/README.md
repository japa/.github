Japa comes with everything you need to test your backend applications. Be it writing JSON API tests using an Open API schema or writing browser tests using Playwright.

Unlike other testing frameworks born out of the frontend ecosystem, Japa focuses only on testing backend applications and libraries. Therefore, Japa is **simpler**, **faster**, and **bloatware free**.

## Features
Despite being a small and a simple tests runner, Japa has a ton of features you expect from a great testing framework. It includes:

- Support for [asynchronous tests](https://japa.dev/docs/testing-async-code).
- Support for [snapshot testing](https://japa.dev/docs/plugins/snapshot).
- Support for [Datasets](https://japa.dev/docs/datasets).
- Official plugins for [chai assert](https://japa.dev/docs/plugins/assert) and [jest expect](https://japa.dev/docs/plugins/expect) assertion libraries.
- [Coverage reporting](https://japa.dev/docs/coverage) using nyc and c8.
- Ability to pin and run only selected tests.
- Multiple [reporters](https://japa.dev/docs/test-reporters) to display tests progress.
- Great CLI experience with pretty diffs and formatted error stacks.
- Works with [ESM and TypeScript](https://japa.dev/docs/introduction#works-with-your-existing-project-setup) both with zero additional setup.

## Why Japa?
There are many testing frameworks available in the JavaScript ecosystem. So let's explore what makes Japa different.

### No overhead of transpiling source code
Popular testing frameworks like Jest (uses Babel) and Vitest (uses Vite) use transpilers to process your source code. No matter how quick the underlying transpilers are, they will always have additional overhead compared to tools with no transpilers.

If you are building libraries or applications to work with Node.js runtime (not the browser), there is no need to use a transpiler. As a result:

- You will have a better debugging experience.
- Your application and tests will boot faster.
- No additional configuration to manage.

### Works with your existing project setup
Since Japa does not have to use transpilers, it works with your existing project setup. Moreover, Japa does not even have a CLI tool. You run your tests using the `node` or `bun` command.
