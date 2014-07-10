ruby_loc_counter
================

Simple script that counts total lines and LOC in one or more Ruby files and outputs the results as an ASCII table.

The main script is located at `bin/ruby_loc_counter` and takes a single argument which may be any of the following:

* A single filename
* A directory name
* A string representing a Glob

In each case, the script will find all matching Ruby files and count the number of total lines and non-comment, non-whitespace lines.  These results will be written to the console as a table like the following:

```
--------------------------------------------------------------------------------------------
| Filename                                                               | Lines  | LOC    |
--------------------------------------------------------------------------------------------
| /home/chris/Projects/minitest/design_rationale.rb                      |     52 |     35 |
| /home/chris/Projects/minitest/lib/hoe/minitest.rb                      |     26 |     18 |
| /home/chris/Projects/minitest/lib/minitest.rb                          |    765 |    425 |
| /home/chris/Projects/minitest/lib/minitest/assertions.rb               |    661 |    352 |
| /home/chris/Projects/minitest/lib/minitest/autorun.rb                  |     12 |      9 |
| /home/chris/Projects/minitest/lib/minitest/benchmark.rb                |    423 |    160 |
| /home/chris/Projects/minitest/lib/minitest/expectations.rb             |    281 |     32 |
| /home/chris/Projects/minitest/lib/minitest/hell.rb                     |     11 |      9 |
| /home/chris/Projects/minitest/lib/minitest/mock.rb                     |    220 |    131 |
| /home/chris/Projects/minitest/lib/minitest/parallel.rb                 |     40 |     35 |
| /home/chris/Projects/minitest/lib/minitest/pride.rb                    |      4 |      3 |
| /home/chris/Projects/minitest/lib/minitest/pride_plugin.rb             |    142 |     84 |
| /home/chris/Projects/minitest/lib/minitest/spec.rb                     |    294 |    145 |
| /home/chris/Projects/minitest/lib/minitest/test.rb                     |    285 |    124 |
| /home/chris/Projects/minitest/lib/minitest/unit.rb                     |     45 |     32 |
| /home/chris/Projects/minitest/test/minitest/metametameta.rb            |     80 |     57 |
| /home/chris/Projects/minitest/test/minitest/test_minitest_benchmark.rb |    137 |     87 |
| /home/chris/Projects/minitest/test/minitest/test_minitest_mock.rb      |    500 |    369 |
| /home/chris/Projects/minitest/test/minitest/test_minitest_reporter.rb  |    313 |    219 |
| /home/chris/Projects/minitest/test/minitest/test_minitest_spec.rb      |    838 |    626 |
| /home/chris/Projects/minitest/test/minitest/test_minitest_unit.rb      |   1865 |   1415 |
--------------------------------------------------------------------------------------------
```
