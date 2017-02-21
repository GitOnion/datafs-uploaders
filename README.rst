=============================
DataFS Batch Uploader Library
=============================

.. image:: https://readthedocs.org/projects/datafs-uploaders/badge/?version=latest
        :target: https://datafs-uploaders.readthedocs.io/en/latest/?badge=latest
        :alt: Documentation Status

.. image:: https://pyup.io/repos/github/climateimpactlab/datafs-uploaders/shield.svg
        :target: https://pyup.io/repos/github/climateimpactlab/datafs-uploaders/
        :alt: Updates

Library of DataFS batch uploaders

Example Uploaders
-----------------

Base Template
~~~~~~~~~~~~~

* `template.py <http://github.com/ClimateImpactLab/datafs-uploaders/blob/master/uploaders/template.py>`_

Additional uploaders
~~~~~~~~~~~~~~~~~~~~

* `hddcdd.py <http://github.com/ClimateImpactLab/datafs-uploaders/blob/master/uploaders/hddcdd.py>`_ - script for uploading ACP HDDCDD data - Michael Delgado


Instructions
------------

1.  Fill out user-defined parameters

2.  Modify user-defined functions to ensure that the archive names, tags,
    metadata, and dependencies will be correct

    - Check out the library functions to pull metadata automatically from 
      netCDF, metaCSV, and fgh files

3.  Do a "dry run":

    .. code-block:: bash
        
        python my_script_name.py -d

4.  Do a live run by running

    .. code-block:: bash

        nice nohup python my_script_name.py &

5.  Look for the output logs in nohup.out


Contributing your own
---------------------

1. Fork this repository, then clone it to your system

2. Copy & rename one of the files most similar to your use case, giving it a
   descriptive name so others will be able to understand what it is for. Modify
   the file to suit your needs.

3. Include a link to your example and some descriptive text in the list above

4. Commit your changes, and push to your forked repo

5. File a pull request to merge the changes back into the master list.