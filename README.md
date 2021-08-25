# sync-input

A small library that provides synchronous input function for NodeJS. 

It is used in educational JavaScript projects for [Hyperskill](https://hyperskill.org).

This is simplified version of [prompt-sync](https://github.com/heapwolf/prompt-sync) library and intended to be used not with an actual keyboard, but with an stdin pipe.

## Installation

You can install this library using the following command. You don't need `git` to be installed to perform this command.

```shell
npm install https://github.com/hyperskill/sync-input/archive/main.tar.gz
```

Or you can add the following line into your `package.json` file.

```json
"dependencies": {
    "sync-input": "https://github.com/hyperskill/sync-input/archive/main.tar.gz"
}
```

## Usage

To import the function you can use `require` function:

```javascript
const input = require('sync-input');
```

To use, just call this `input` function. It pretty much behaves like `Python`'s `input` built-in function. 

```javascript
let name = input();
let age = Number(input());
```

You can also pass prompt that will be printed before requesting input.

```javascript
let name = input("Print your name: ");
let age = Number(input("Print your age: "));
```