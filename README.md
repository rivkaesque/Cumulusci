# README #

This example requires the installation of Python 2 and [CumulusCI](https://github.com/SalesforceFoundation/CumulusCI) and probably shuold use also a virtualenv environment for windows/mac/linux.

### How Do I Run It ###

* Setup a python environment (e.g. a virtualenv environment)
* Launch your terminal / virtual environment
* Install CumulusiCI (e.g. pip install cumulusci)
* Connect to an org:
    * cci org conect *yourorgalias*
* Set default org:
    * cci org default *yourorgalias*
* Run the flow (Warning: the delete task will delete all data from the objects in the test data):
    * cci flow run sandbox_data
* Or... run the tasks:
    * cci task run sandbox_data_delete
    * cci task run sandbox_data

### Related Resources ###

* [NPSP Repo Sample Cumulus.yml file](https://github.com/SalesforceFoundation/Cumulus/blob/master/cumulusci.yml)
    * Includes sample delete tasks and other interesting task
* [NPSP Repo testdata folder](https://github.com/SalesforceFoundation/Cumulus/tree/master/testdata)
    * Includes other larger test data sets for use in non-developer instances. 
* The mapping.yml file in this repo is based on the [mapping.yml](https://github.com/SalesforceFoundation/Cumulus/blob/master/testdata/mapping.yml) from the Cumulus repo -- which is intended to be used in an instance as an unmanaged package so all custom fields that are referenced in the mapping file in this repo have been updated to use the npsp prefix.