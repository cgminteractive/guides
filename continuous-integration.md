Continuous Integration
======================

[Martin Fowler](https://martinfowler.com/articles/continuousIntegration.html) has an extensive description of Continuous Integration. The basics are:

* We have a test suite that each developer runs on their own machine.
* When they commit their code to a shared version control repository, the tests are run again, "integrated" with code from other developers.

This helps ensure there's nothing specific to the developer's machine making the tests pass. The code in version control needs to run cleanly in production later so before the code is allowed to be deployed to production, it is run on a CI server or service.

When a build fails, we get alerts via email. Click the alert and we see a backtrace that gives us a hint of how to "fix the build."

When we write the fix and commit to version control again, we'll get a "passing build" alert via email. Click the alert and we see the passing build.

Green is good.

A solid test suite is an absolute requirement for a web application. However, one major problem with test suites is that they get slow as they get large.

CI can ease the pain by distributing the test runs in parallel.

We use Travis CI Free for open source projects. We use Travis CI Pro for private repositories because of its consistent UI, simple configuration and its close integration with GitHub.

CI test runs are triggered by GitHub post-receive hooks.