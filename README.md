## Node.js v7 async/await demo

### What is this?

Node.js v7.x.x ships with experimental async/await support, greatly simplifying boilerplate required for writing modern server side code. This project is a demonstration of the minimal setup in order to use the new async/await features in Node.

NOTE: async/await are not officially supported in Node.js v7.x at this point. You are welcome to try things out, but there may be no support if you encounter bugs.

### Node.js v7 - setup using node version manager (nvm) - recommended

Go to http://nvm.sh and follow the instructions on installing nvm for your platform.
Then add v7 mirror to NVM:
```
NVM_NODEJS_ORG_MIRROR=https://nodejs.org/download/test
```
After you added the v7 mirror, install v7 version using NVM:
```
nvm install 7
nvm use 7
```

### Node.js v7 - manual setup
Download and install node.js v7 nightly version for your platform
```
https://nodejs.org/download/test/v7.0.0-test201610107f7d1d385d/
```

### Run the demo
Currently async / await support ships under --harmony-async-await flag.
npm start command executes `node --harmony-async-await index.js`

```
npm install
npm start
```

### What does not work

While async/await is a great addition, some things like ES6 module support (`import x from 'x'`) and arrow function support in class declaration (`class A { b() => {} }`) are still not supported.

If you use these features you might still want to keep a ES6/ES7 -> ES5 transpiler like Babel.
