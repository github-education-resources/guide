### Using repositories

First, follow the instructions to [set up assignment repositories][repository-setup].  Once created, the repositor(ies) should be "seeded" with boilerplate content.  This may just be a simple README, but could include a starter source code file, `main()` function, etc.

#### Automated testing

[Automated testing][automated-testing] (often referred to as part of [continuous integration][ci], or "CI") is a great way to quickly verify students' solutions.  Your test suite could include any of the following:

* Static analysis / linting
    * [HTML validation][html-validator]
    * [JSHint][jshint]
    * [Cppcheck][cppcheck]
    * *and [many others][static-analysis]*
* Unit tests
    * Tests can be written by you, and/or by the students
    * Hidden from the student (a.k.a. an "autograder") or not

There are lots of tools and services that can run automated tests, including:

* [Travis CI][travis]
* [Jenkins CI][jenkins]
* [Web-CAT][web-cat]
* [CodeClimate][code-climate]
* [Coveralls][coveralls]

These tools can be configured to run the tests every time new code is pushed up to a student's repository using [webhooks][webhooks], though some do the setup automatically.

### Collecting assignments

* https://github.com/education/teachers/issues/7
    * Since commits can be modified after the fact, don't rely on the timestamps
* Script to clone/download all repos
    * https://github.com/education/teachers-pet#pulling-repositories-for-grading
* Don't put grades on github.com, due to FERPA regulations
    * Only when students can see one another's repos?
    * Feedback ok?
    * Enterprise ok
* Encouraging collaboration
    * Peer code review via PRs

<!-- Links -->
[repository-setup]: /guide/repository_setup
[automated-testing]: https://en.wikipedia.org/wiki/Test_automation
[ci]: https://en.wikipedia.org/wiki/Continuous_integration
[html-validator]: http://validator.w3.org/source/
[jshint]: http://www.jshint.com/about/
[cppcheck]: http://cppcheck.sourceforge.net
[static-analysis]: https://en.wikipedia.org/wiki/List_of_tools_for_static_code_analysis
[travis]: http://docs.travis-ci.com
[jenkins]: http://jenkins-ci.org
[web-cat]: http://web-cat.org
[code-climate]: https://codeclimate.com
[coveralls]: https://coveralls.io
[webhooks]: https://developer.github.com/webhooks/
