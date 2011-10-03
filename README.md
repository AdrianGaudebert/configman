configman
=========

(c) Mozilla

General tool for setting up configuration options per namespaces.
Supports reading and writing configs generally from and into config
files.


Running tests
-------------

We use [nose](http://code.google.com/p/python-nose/) to run all the
unit tests. To run the whole suite just run: 

    nosetests
    
If you want to run a specific test in a testcase class you might
consider this command:

    nosetests configman.tests.test_config_manager:TestCase.test_write_flat
    
To run with test coverage calculation run ``nosetests`` like this:

    nosetests --with-coverage --cover-html \
     --cover-package=config_manager,converters,datetime_util,\
     config_exceptions,dotdict,namespace,option,options_by_conf,\
     options_by_configparser,options_by_getopt
     
