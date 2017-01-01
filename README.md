# ZScript

Scripting language for Meta Zen, Zen Spaces.

Why ES6?

I started by developing a prototype in C++, which is my strongest language.  C++ takes a lot of work and gets very ugly even though I feel that I write beautiful code.

I also used Python and then Lisp and then Clojure for awhile, developing more prototypes to experiment with other aspects, but those implementations also was were quite ugly.

For another project, I ran across Aurelia, which introduced me to ES6/ES2015 and Babel.  I had already used Node.js for a few things and I liked how easy it was to create network applications using these tools, and then I ran across MAL, which has an implementation of Lisp in ES6.

So, I put it all together, started with MAL, Node.js, and Aurelia as my base implementation for ZScript and associated editors (at least that was the plan) and the result was this project.... a functioning implementation of ZScript.

I'm re-implementing Zen Spaces and Meta Zen using ZScript which allows me to write beautiful natural code directly targeting the Zen Spaces platform.  This bootstrap code will allow me to bootstrap the next generation of Zen Spaces.

## Building the Code

To build the code, use the following steps.

Ensure that [NodeJS](http://nodejs.org/) (6.0 or greater) is installed.

Install libedit-dev (for command-line repl)
```shell
sudo apt install libedit-dev
```

Install the project dependencies using NPM:
```shell
npm install
```

Install [Gulp](http://gulpjs.com/) if it's not already installed.
```shell
sudo npm install -g gulp
```

Generate the code
```shell
gulp build
```

5. Run ZScript
```shell
node dist/zscript/main.js {your zs file}
```
