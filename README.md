JBoss AS Quickstart for MongoDB
===============================

This is a simple Red Hat OpenShift example containing a JavaEE6
servlet that illustrates some of the steps in the MongoDB Java
Tutorial: <http://www.mongodb.org/display/DOCS/Java+Tutorial>

To use:

1. Run: rhc app create -a testmongo -t jbossas-7
2. Run: rhc app cartridge add -a testmongo -c mongodb-2.0
3. Update the resulting testmongo repository by running:

    cd testmongo
    git remote add upstream -m master git://github.com/openshift/jbossas-mongoDB-quickstart.git
    git pull -s recursive -X theirs upstream master


4. Push up to OpenShift, by running:

    git push

5. The application will deploy.  You can access the test servlet by
appending /mongoDB to your application URL. For example:

    <http://testmongo-$yournamespace.rhcloud.com/mongoDB>

The quickstart code is licensed under the Apache License, Version 2.0:
<http://www.apache.org/licenses/LICENSE-2.0.html>

