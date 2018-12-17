## 07 - Combine Multiple State ADT Instances With The Same Input

When combining multiple State ADT instances that depend on the same input,
using `chain` can become quite burdensome. We end up having to play leapfrog
with values inside of nested chain statements. Very reminiscent of the old
callback nastiness we had to deal with before `Promises` graced our existence.

But fear not, but taking advantage of the Applicative Functor portion of the
`State` ADT in combination with the `converge` combinator, we can apply these
types of transitions in unison, passing the value to both virtually
simultaneously.

The lesson on egghead can be found [here][5]

### Requirements
This code example runs on a POSIX based system (Linux, OSX, etc) in a [nodejs][2] environment
requiring a version greater than `4.2.x` to be run. If you *have* to work in another environment,
this lesson also has a "sandbox" hosted on [Code Sandbox][3] that can be run in browser and can be found
here:

[Lesson Sandbox][4]

### Using This Example
This code example and environment is provided on its own branch. To run this locally, just clone
this repository down, check out this branch and run the following commands:

#### Setup Your Dependencies
To setup the lesson, execute this command in the project folder:

```
$ npm run setup
```

#### Run The Code
Once all dependencies have been pulled down, you can then run the example code.

This code runs in a node environment and logs to the console that the code was run in. Once
started, the environment will listen to changes to the files and re-run the code. This allows
you to have immediate feed back to the changes you made. To exit out of the code example,
just press the keystroke `Ctrl+C`.

To run the lesson, execute the following in the project folder:

```
$ npm start
```

[1]: https://egghead.io/instructors/ian-hofmann-hicks
[2]: https://nodejs.org/
[3]: https://codesandbox.io/

[4]: https://codesandbox.io/s/github/eggheadio-projects/redux-and-the-state-adt/tree/master/07
[5]: https://egghead.io/lessons/redux-combine-multiple-state-adt-instances-with-the-same-input
