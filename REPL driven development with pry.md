### REPL driven development with Pry

This talk was amazing!

- PRY started as a 1 line of code project, it's now 12,000+
- While using PRY we can use `? var/method`. This is the same as doing `show-doc var/method` and shows the documentation for the method/var
- While using PRY we can use `$ var/method`. This is the same as doing `show-source var/method` and shows the code for the method/var
- While using PRY we can use `ls object`. It shows the methods for a given object
- `pry-plus` is where the cool stuff is. `minitest` and `spec` are great for TDD. By using `minutest` it will stop when test fails.
  - `break method` will add a break point
  - `try-again` will run the test again
  - `play -l line_number` will run a given line number but lease the pointer in the same place
  - `edit -m` will open the editor and enable us to change the method. This is great because we don't need to stop and run things again.
  - This is really great to fix tests or understand why they are failing!
- using `binding.pry`. It will create a breakpoint where you placed it
  - `up` and `down` to move up and down the stack
  - `cd` will let us move sideways on the breakpoint. On the method `reques.thing` `cd request` will go into the `request` object.
  - `whereami` will tell the context of the code where we are at the moment
  - `help` will show all of these commands plus others!
  
### Links

- https://bugsnag.com/ - Nice tool to handle bugs