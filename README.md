The purpose of this repo is to setup clojurescript nrepl using clojure cli (deps.edn) with calva as minimal as possible.

Start repl _assuming your are in project dir_

```
clj -A:nrepl
```

Open the project in vscode and connect to running repl

`ctrl+alt+c` `ctr+alt+c`

Select `Clojure CLI`

**ISSUE**

Go to `src/etudes_cljs/core.cljs`
Then put the cursor at the end line `(def hello "hello")`
And press `ctrl+alt+c` `ctrl+alt+e` (to send evaluation to repl)

You will get this error

```
Error evalution require form: class

java.io.FileNotFoundException

Source: Calva: Clojure & ClojureScript Interactive Programming (Extension)
```

**What is missing in this setup?**



TODO
====
[] setup a custom connection sequence in calva that promotes clj repl to cljs repl
[docs](https://calva.readthedocs.io/en/latest/connect-sequences.html)
[built-in samples](https://github.com/BetterThanTomorrow/calva/blob/master/src/nrepl/connectSequence.ts)
