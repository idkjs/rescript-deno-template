
This is a repo showing how to use [ReScript](https://github.com/rescript-lang/rescript-compiler) with
[Deno](https://deno.land/#installation).

It assumes you are already familiar with both.

# Build
```
./node_modules/bs-platform/bsb -w # build and watch
```

Note here we only use npm as a downloader, you don't have to use npm, you can just grab the package from npmjs.com and put it in
`node_modules` directory

# Calling function from .ml file
`demo.res`
```ocaml
Example.demo
Js.log(List.length(list{1,2,3}))
```
# Run

```
deno run ./lib/es6_global/src/demo.js
```

# Run `.ml` file

```
deno run ./lib/es6_global/src/Example.js
```
