multi modular maven assembly plugin and release plugin example
==============

Just sandbox for playing around with maven multi-module project assembly and release.
It does contain though a final, currently recommended solution by the Apache Maven guys for projects which require the following:

* multimodular
* has inter-modular dependencies
* want to have one big zip deployed to the repository, containing
  * dependencies in separate folder (lib) 
  * module jars (deployables) in separate folder
  * script,... folders copied

The work was, after lots of googling, and headbanging was finally based on [The Maven team's recommended solution for these cases](http://maven.apache.org/plugins/maven-assembly-plugin/examples/multimodule/module-binary-inclusion-simple.html)

You can just simply run, and it will work (please update your repository url-s/user scm-s :))

`` mvn release:clean release:prepare release:perform -B
