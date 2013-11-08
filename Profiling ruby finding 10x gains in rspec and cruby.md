### Profiling Ruby: Finding 10x Gains In RSpec and CRuby

Author: [Xavier Shay](http://rubyconf.org/program#xavier-shay)

- Speed up slow things (yay \o/)
- Not about tools but about the mindset
- Steps :
  - Hypothesize
  - Isolate
  - Instrument
- Believe that you are going to find something
- "Rails is slow to boot up" (fuck yes!)
  - Hypothesise: Loads gems, loads rails, etc
  - Isolate: 
    - try stuff to narrow down where the problem might be
    - use global stamps to profile code
    - use caller (gives your current stack trace)
    - there's a PR [https://github.com/rails/rails/pull/12745](https://github.com/rails/rails/pull/12745)
    - [gnuplot](http://rubygems.org/gems/gnuplot) is a great app to generate graphs for profiling comparison
- "My 'unit' tests are slow"
  - RSpec released version 3 beta which should be faster
  - ruby-prof is a good profiling tool
  - didn't speak anything specific about actually speeding up tests, more about how he sped up RSpec itself
  
  