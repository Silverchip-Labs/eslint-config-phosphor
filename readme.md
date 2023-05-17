# eslint-config-phosphor

eslint-config-phosphor is a custom ESLint configuration package that provides a set of rules and configurations to enforce consistent code style and quality in your TypeScript/React(& Native) projects. It is designed to be flexible, extensible, and highly customizable, allowing you to tailor the linting rules to suit your specific needs.

## Features

  * Consistent Code Style: eslint-config-phosphor helps maintain a consistent code style across your codebase, ensuring that all team members follow the same conventions and best practices.
  * Code Quality Assurance: The package includes a set of rules that helps identify potential errors, bugs, and problematic patterns in your code, helping you write higher-quality and more reliable software.
  * Extensible and Customizable: eslint-config-phosphor provides a solid foundation for linting your code, but it also allows you to customize and extend the rules to fit your project's requirements. You can easily override rules, add your own rules, or include other plugins and shareable configs.

## Installation

To start using eslint-config-phosphor, you need to follow these simple steps:

1. Install the package as a development dependency in your project:

```bash
npm install --save-dev eslint-config-phosphor
```

2.    Create an .eslintrc file in the root of your project or update your existing .eslintrc file.

3.    Extend the eslint-config-phosphor configuration in your .eslintrc file:

```json

{
  "extends": "eslint-config-phosphor"
}
```

4.  Customize the configuration to meet your project's needs by adding or modifying rules.

## Usage

eslint-config-phosphor provides a comprehensive set of linting rules out of the box. However, you can easily override or modify any rule to fit your project's specific requirements. Here are some common scenarios:
Extending the Configuration

To extend the default configuration with additional rules or configurations, modify your .eslintrc file:

```jsonc

{
  "extends": [
    "eslint-config-phosphor",
    "plugin:@typescript-eslint/recommended"
  ],
  "rules": {
    // Additional or overridden rules
  }
}
```

## Overriding Rules

To override specific rules provided by eslint-config-phosphor, simply update the rules section in your .eslintrc file:

```jsonc

{
  "extends": "eslint-config-phosphor",
  "rules": {
    "indent": ["error", 4], // Override the indent rule
    // Other rule overrides
  }
}
```
## Adding Custom Rules

eslint-config-phosphor allows you to add your own custom rules or plugins. To add custom rules, first, create a custom plugin or rule file in your project, and then add it to your .eslintrc file:

```json

{
  "extends": "eslint-config-phosphor",
  "plugins": ["my-custom-plugin"],
  "rules": {
    "my-custom-plugin/rule-name": "error"
  }
}
```
Make sure to install any necessary dependencies for your custom rules or plugins.
## Contributing

Contributions are welcome! If you have suggestions, bug reports, or would like to contribute improvements or new features, please open an issue or submit a pull request on the GitHub repository.

Before contributing, please read our Contribution Guidelines for more information on how to get started.
## License

eslint-config-phosphor is licensed under the MIT License.