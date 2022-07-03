### In VSCode

1. Install the ESLlint extension
2. Extensions - ESLint - Enable ESLint as a formatter
3. Text Editor - Set ESLint as default formatter
4. Enable Format on Save



### In project

```
npm init -y
```



```
npx eslint --init
```
```
You can also run this command directly using 'npm init @eslint/config'.
Need to install the following packages:
  @eslint/create-config
Ok to proceed? (y)
√ How would you like to use ESLint? · style
√ What type of modules does your project use? · esm
√ Which framework does your project use? · none
√ Does your project use TypeScript? · No / Yes
√ Where does your code run? · browser
√ How would you like to define a style for your project? · guide
√ Which style guide do you want to follow? · airbnb
√ What format do you want your config file to be in? · JSON
Checking peerDependencies of eslint-config-airbnb-base@latest
Local ESLint installation not found.
The config that you've selected requires the following dependencies:

@typescript-eslint/eslint-plugin@latest eslint-config-airbnb-base@latest eslint@^7.32.0 || ^8.2.0 eslint-plugin-import@^2.25.2 @typescript-eslint/parser@latest
√ Would you like to install them now? · No / Yes
√ Which package manager do you want to use? · npm
Installing @typescript-eslint/eslint-plugin@latest, eslint-config-airbnb-base@latest, eslint@^7.32.0 || ^8.2.0, eslint-plugin-import@^2.25.2, @typescript-eslint/parser@latest
```


Add this rule 
```
"linebreak-style": ["error", "windows"]
```
https://eslint.org/docs/latest/rules/linebreak-style

The linebreaks (new lines) used in windows operating system are usually carriage returns (CR) followed by a line feed (LF) making it a carriage return line feed (CRLF) whereas Linux and Unix use a simple line feed (LF). The corresponding control sequences are "\n" (for LF) and "\r\n" for (CRLF).

This rule has a string option:
    "unix" (default) enforces the usage of Unix line endings: \n for LF.
    "windows" enforces the usage of Windows line endings: \r\n for CRLF.
