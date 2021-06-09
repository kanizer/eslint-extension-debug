# eslint-extension-debug

VSCode extension error sample for issue [#1227](https://github.com/microsoft/vscode-eslint/issues/1227).

Executing `eslint .` from the command line works as expected, but the extension in Code produces output errors and no meaningful linting feedback.

## Output panel error

```
[Info  - 10:05:12] ESLint server is running.
(node:34209) UnhandledPromiseRejectionWarning: Unhandled promise rejection (rejection id: 1): SyntaxError: Unexpected token ...
(node:34209) DeprecationWarning: Unhandled promise rejections are deprecated. In the future, promise rejections that are not handled will terminate the Node.js process with a non-zero exit code.
(node:34209) UnhandledPromiseRejectionWarning: Unhandled promise rejection (rejection id: 2): SyntaxError: Unexpected token ...
```

## System

- MacOS 11.4
- Code v1.22.2
- Node v8.9.4 - v14.11.0
- eslint v6.5.1
- ESLint plugin v1.4.10 (this is the version auto-installed; manually installed newer releases do not work?)
