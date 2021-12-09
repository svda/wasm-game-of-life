## About

Browser implementation of Conway's Game of Life using Rust and Webassembly (WASM).

## Getting started

First make sure you have Rust, wasm-pack and NPM installed.

Cmpile the Rust source:

```
wasm-pack build
```

This will generate a `pkg` folder with the compiled Rust code that is used by the browser.

Install Javascript dependencies and run the webpack development server:

```
cd ./www
npm install
npm start
```

It should open a browser window with a running life instance.

## 🔋 Batteries Included

* [`wasm-bindgen`](https://github.com/rustwasm/wasm-bindgen) for communicating
  between WebAssembly and JavaScript.
* [`console_error_panic_hook`](https://github.com/rustwasm/console_error_panic_hook)
  for logging panic messages to the developer console.
* [`wee_alloc`](https://github.com/rustwasm/wee_alloc), an allocator optimized
  for small code size.
