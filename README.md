# dataflow-p2-site

This Maven POM is used to setup a local Eclipse update site for the Actian DataFlow components needed to build custom DataFlow operators.

## Building

The update site is built using [Apache Maven 3.0.5 or later](http://maven.apache.org/).

To build, run:

    mvn clean package

## Configuration

After building the update site you will need to define a couple of environment variables to allow the DataFlow operator projects to find the site and to determine the DataFlow version to use.  The version number can be determined from the output of the Maven build.

    export DATAFLOW_REPO_HOME=/Users/myuser/dfops/dataflow-p2-site
    export DATAFLOW_VER=6.5.0.117


