JBoss AS Quickstart for MongoDB
===============================

This is a simple quickstart that replaces the default jbossas-7.0 express
application type with one containing a servlet that illustrates some of
the steps in the MongoDB Java Tutorial:
<http://www.mongodb.org/display/DOCS/Java+Tutorial>

To use:
1. Run: rhc-create-app -a testmongo -t jbossas-7.0
2. Run: rhc-ctl-app -a testmongo -e add-mongodb-2.0
3. Update the resulting testmongo repository by running:


The quickstart code is licensed under the Apache License, Version 2.0:
<http://www.apache.org/licenses/LICENSE-2.0.html>

