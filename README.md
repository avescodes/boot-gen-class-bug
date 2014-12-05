## With Leiningen

```
$ lein repl
> (require 'repro)
nil
> (repro/-main)
"Hello, World"
nil
```

## With Boot

```
$ boot repl
> (require 'repro)

clojure.lang.Compiler$CompilerException: java.lang.RuntimeException: Unable to resolve symbol: repro in this context, compiling:(repro.clj:1:1)
             java.lang.RuntimeException: Unable to resolve symbol: repro in this context
```

Uncommenting the `repro`-based task in `build.boot` causes `boot repl` to fail altogether.
