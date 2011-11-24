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

    git remote add upstream -m master git://github.com/openshift/jbossas-mongoDB-quickstart.git
    git pull -s recursive -X theirs upstream master
4. Edit the src/main/webapp/WEB-INF/web.xml init-param values to
reflect the correct host, port, password based on the output from step 2.

Now you should be able to commit and push the changes, and once deployed,
access the test servlet by appending /mongoDB to your application URL, for
example:
http://testmongo-sstark.dev.rhcloud.com/mongoDB

The quickstart code is licensed under the Apache License, Version 2.0:
<http://www.apache.org/licenses/LICENSE-2.0.html>

