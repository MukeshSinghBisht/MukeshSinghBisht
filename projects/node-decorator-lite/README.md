# Node Decorator Lite

> Minimalistic custom decorator support for Node.js — bring the power of decorators to plain JavaScript apps without needing TypeScript.

## 🚀 Overview

This library allows developers to define and use decorators in native JavaScript (Node.js) to write cleaner, modular, and annotation-driven code — mimicking the power of TypeScript decorators in pure JS environments.

## ✨ Features

- Lightweight and dependency-free
- Class and method-level decorators
- Useful for modularizing logging, validation, permission checks, etc.
- Works with native Node.js or any framework (Express, Nest-lite clones)

## 🔧 Example

```js
const { decorate, defineDecorator } = require('node-decorator-lite');

// Define a custom logger decorator
const Log = defineDecorator((fn, context) => {
  return function (...args) {
    console.log(`[${context.methodName}] args:`, args);
    const result = fn.apply(this, args);
    console.log(`[${context.methodName}] result:`, result);
    return result;
  };
});

class MyService {
  @Log
  computeSum(a, b) {
    return a + b;
  }
}

const service = new MyService();
service.computeSum(2, 3);
