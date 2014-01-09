The IntelliJ IDEA JavaScript analyzer seems to be hanging on Q chained
.then() clauses.

# Steps to reproduce

```
$ git clone https://github.com/leedm777/intellij-bugs.git --branch analyzer-hanging
$ cd intellij-bugs
$ npm install
```

* Open the intellij-bugs project.
* Open `app.js`.

# Expected results

Analyzer should report all green.

# Actual results

The analyzer hangs and never finishes processing. If you pay attention
to the syntax highlighting of the `.then()` functions, you can roughly
see where it's hanging.

# Environment

 * OS X 10.9.1
 * Node v0.10.24
 * IntelliJ IDEA 13.0.1
   * JRE 1.6.0_65
