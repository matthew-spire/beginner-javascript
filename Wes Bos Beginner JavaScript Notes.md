### Lesson 5 - Code Quality Tooling with Prettier and ESLint

- Tools to help with formatting and maintaining a consistent opinion
- ESLint
  - [ESLint](https://eslint.org/)
  - JavaScript linter tool for identifying and reporting potential issues in your code
  - Can configure to your style
  - Plugable (Vue, React, Angular) for whatever flavor of JavaScript
- Prettier
  - [Prettier](https://prettier.io/)
  - An opinionated code formatter
    - Helps with consistent formatting (i.e. all '' or all "", etc.)
  - Use the plugin for ESLint
- Use Wes's config, then modify as you become accustomed to a style
  - [No-Sweat™ Eslint and Prettier Setup](https://github.com/wesbos/eslint-config-wesbos)
  - Follow the instructions to install locally
  - VS Code
    - Install ESLint package
    - Configure the settings.json
- Will format your code and inform you of errors, but will not fix the errors

### Lesson 6 - Types: Introduction

- There are seven (7) types in JavaScript
- Can be remembered using the mnemonic SNOB'N'US
  - S = String
    - E.g.: "text", 'text', etc.
  - N = Number
    - E.g.: 1, 1.5, etc. (i.e. numbers that do and do not have decimal places)
  - O = Object
    - Special &rarr; everything in JavaScript is an object
  - B = Boolean
    - True or False
  - N = Null
    - Nothing
  - U = Undefined
    - Nothing
  - S = Symbol
    - Guaranteed unique identifier &rarr; helpful when trying to come up with a unique ID inside of an object and avoid overwriting something

### Lesson 7 - Strings

- Strings &rarr; used for holding text
- Three (3) different ways to create a string
  - Single quotes, i.e. `const first = 'Wes';`
  - Double quotes, i.e. `const middle = "Topher";`
  - Back ticks, i.e. `` const last = `Bos`; ``
- Single quotes and double quotes are the same thing
- Mixing of double quotes and single quotes
  - E.g.: `"Jack's dog"`
- Backslash to escape
  - Escaping &rarr; tell the compiler that the next character is text and not JavaScript syntax
  - E.g.: `'Jack\'s dog`
  - String across multiple lines using single quotes:  
    <code>
    const song = 'Ohhh\\  
    \\  
    ya\\  
    I like\\  
    Miso';
    </code>
- Use back ticks

  - E.g.: `` const sentence = `'Jack's dog is the "best"` ``
  - String across multiple lines using back ticks:  
    <code>
    const song = `Ohhh

    ya  
    I like  
    Miso`;
    </code>

    - No need to use \ to escape
    - Maintains the line breaks

- Concatenation
  - When two or more strings are combined into one
  - E.g.: `` const hello = `Hello! My name is ` + name + `. Nice to meet you`; ``
- Interpolation
  - When you put a variable inside of a string
  - E.g.: `` const hello = `Hello! My name is ${name}. Nice to meet you`; ``
  - Less chance for bugs &rarr; not using an operator, i.e. +, that is also used for working with numbers
- Get use to using back ticks
