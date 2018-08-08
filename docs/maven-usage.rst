Maven usage
========================

jgitver operates as a maven core extension and needs a per project installation.

Installing is as simple as running the following command from the root directory of your project *(see below for othe methods)*:

.. code-block:: none

    sh -c "$(curl -fsSL https://raw.githubusercontent.com/jgitver/jgitver-maven-plugin/master/src/doc/scripts/install.sh)"

Congratulations, your project now uses jgitver, run `mvn validate` to be convinced that jgitver works

.. code-block:: none

    $ mvn validate
    [INFO] no suitable configuration file found, using defaults
    [INFO] Scanning for projects...
    [INFO] Using jgitver-maven-plugin [1.3.0] (sha1: ef8eec9f820d662e63a84f1210c377183e450cbd)
    [INFO] jgitver-maven-plugin is about to change project(s) version(s)
    [INFO]     fr.brouillard.oss::jgitver::0 -> 0.7.0-SNAPSHOT


Installation methods
--------------------

All the installation scripts below will use the latest version available ; if you are updating find the `latest version here`_ or `there`_.

**curl**
^^^^^^^^

.. code-block:: none

    sh -c "$(curl -fsSL https://raw.githubusercontent.com/jgitver/jgitver-maven-plugin/master/src/doc/scripts/install.sh)"

**wget**
^^^^^^^^

.. code-block:: none

    sh -c "$(wget https://raw.githubusercontent.com/jgitver/jgitver-maven-plugin/master/src/doc/scripts/install.sh -O -)"

manual installation
^^^^^^^^^^^^^^^^^^^

* Create a directory `.mvn` under the root directory of your project.
* Create file `.mvn/extensions.xml`
* Put the following content to `.mvn/extensions.xml` (adapt to `latest version`_).

.. code-block:: none

    <extensions xmlns="http://maven.apache.org/EXTENSIONS/1.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xsi:schemaLocation="http://maven.apache.org/EXTENSIONS/1.0.0 http://maven.apache.org/xsd/core-extensions-1.0.0.xsd">
      <extension>
        <groupId>fr.brouillard.oss</groupId>
        <artifactId>jgitver-maven-plugin</artifactId>
        <version>1.3.0</version>
      </extension>
    </extensions>

.. _latest version here: http://search.maven.org/#search%7Cga%7C1%7Cg%3A%22fr.brouillard.oss%22%20AND%20a%3A%22jgitver-maven-plugin%22
.. _latest version: http://search.maven.org/#search%7Cga%7C1%7Cg%3A%22fr.brouillard.oss%22%20AND%20a%3A%22jgitver-maven-plugin%22
.. _there: http://search.maven.org/solrsearch/select?q=g:%22fr.brouillard.oss%22+AND+a:%22jgitver-maven-plugin%22&core=gav&rows=1&wt=json