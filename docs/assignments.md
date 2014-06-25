### Using repositories

First, follow the instructions to [set up assignment repositories][repository-setup].  Once created, the repositor(ies) should be "seeded" with boilerplate content.  This may just be a simple README, but could include a starter source code file, `main()` function, etc.

#### Project pages

If the students need to provide background materials, documentation, or blog posts about their project, you can have them:

* Commit [Markdown][markdown] files directly to the repository
* Use the [repository wiki][wikis]
* Build a project/class homepage using [GitHub Pages][pages]

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

The recommended mechanics use for collecting assignments depends on whether you use the [fork][forks] or [sandbox][sandboxing] strategy.  In either case, feedback can be given inline in pull requests or [commits][commit-comments], or by opening [issues][issues] in the student's repository for them to fix.  This can be done by instructors, though you may consider incorporating peer code review as a way for students to practice giving and receiving feedback.  Note that you may need to grant students [read-only access][access-permissions] to one another's repositories to allow them to see the contents and leave comments.

One GitHub feature that may come in handy is using the [Network][network] and [contributors][graphs] graphs, as well as the list of commits.  As was [pointed out in our teacher community][community-graphs],

> Having the github analytics have been great -- I just have to look at the contributors graph and quickly scan the commit logs.  I can see who did how much and when in just a couple of seconds. I can also see the ebb and flow of work on the project.

Note, however, that commit authors and timestamps can be modified after the fact.

<!-- Links -->
[repository-setup]: /guide/repository_setup
[markdown]: https://guides.github.com/features/mastering-markdown/
[wikis]: https://guides.github.com/features/wikis/
[pages]: https://pages.github.com
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
[forks]: /guide/forks
[sandboxing]: /guide/sandboxing
[commit-comments]: https://help.github.com/articles/adding-commit-comments
[issues]: https://guides.github.com/features/issues/
[access-permissions]: https://help.github.com/articles/permission-levels-for-an-organization-repository
[network]: https://github.com/blog/39-say-hello-to-the-network-graph-visualizer
[graphs]: https://help.github.com/articles/using-graphs
[community-graphs]: https://github.com/education/teachers/issues/7
