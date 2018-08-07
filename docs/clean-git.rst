Clean git history
========================

jgitver has been created with `DRY`_ & `KISS`_ principles in mind especially to keep a clean git history.

Having this in mind, jgitver has been built to allow to **NOT** modify any project descriptor (pom.xml or build.gradle).

The benefits from the above:

* no pollution of git history for unnecessary commits. Your git log contain **ONLY** business changes ; `tag & deploy` actions are enough for your project
* project version follows defined *(but configurable)* guidelines
* version can be automatically change when working in branch

To summarize if you are familiar with the following unnecessary commits _(in red)_ from `maven release` plugin

.. image:: images/maven-release-occourence-git-history.jpg

Then be happy to hear that `git tag` and `mvn deploy` are enough using jgitver.

.. _DRY: https://en.wikipedia.org/wiki/Don%27t_repeat_yourself
.. _KISS: https://en.wikipedia.org/wiki/KISS_principle