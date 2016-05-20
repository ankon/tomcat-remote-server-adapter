
About
=====

This is an attempt of building a JST server adapter for a remotely running Tomcat. Unfortunately the documentation
of Eclipse in terms of how to actually create those, or just how to even build the existing adapters locally is extremely
insufficient, so this also should serve as a on-going braindump for the steps taken until that initial goal was reached
eventually.

> Eclipse Guys: If you want more contributions, maybe start by actually documenting trivial things!

Goals
-----
- [ ] Create a "do nothing" server based off the ["Generic Server"][wtp-doc-generic-server]
- [ ] Create a "publisher" that works against the Tomcat Manager application. This would use hardcoded settings for URL, username, and password
- [ ] Create a "UI" component so that the tomcat can be configuration

Tools
-----

Likely this project will use Tycho, as that seems to be the easiest to actually automate. This way it should be possible
to produce an update site somewhere, so this plugin(s) can be consumed easily.

Notes
=====

Cloning the base modules:
~~~~
git clone --recursive http://git.eclipse.org/gitroot/webtools/webtools.releng.aggregator.git
~~~~



References
==========
[eclipse-git] http://wiki.eclipse.org/Git
[wtp] https://eclipse.org/webtools/
[so-git-clone-with-modules] http://stackoverflow.com/a/4438292/196315
[eclipse-forum-parent] https://www.eclipse.org/forums/index.php/t/511645/
[wtp-doc-generic-server] https://eclipse.org/webtools/jst/components/server/tutorials/genericServers/ServerDefinitionExplained.html
