.. _dev_getting_started:

Contributing to the Open Archaeology Data API
=============================================

.. todo::
   
   Document the following:

   - Setting up the environment

Want to get involved with the Open Archaeology Data API? Here's how you can help!

Please take a moment to review this document in order to make the contribution process easy and effective for everyone involved.

Using the issue tracker
-----------------------

The `issue tracker <https://github.com/openstate/open-archaeology-data/issues>`_ is the preferred channel for submitting bug reports, feature requests and pull requests.

Bug reports
-----------

Spot an error in the way data is formatted? Getting unexpected error when making a call to the API? Than please submit a bug report. Good bug reports are extremely helpful in order to improve the code, and the project in general.

Some guidelines when submitting a bug report:

- Check if the issue hasn't already been reported.
- Be as detailed as possible, people reading the report shouldn't have to chase you up for more information. Describe the problem thoroughly, so others can try to reproduce it.
- Verify that the problem only occurs within the Open Archaeology Data API, and not in the original source. You can do this by requesting the original document(s) via the REST API (``/(source_id)/(object_id)/source``). Problems in the source data will not be fixed by us and should be reported to the data publishers.

Feature requests
----------------

Feature requests are welcome, but take a moment to find out whether your idea fits the scope and goals of the project. It's up to you to make a strong case to convince others of the merits of feature your are requesting. Please provide as much detail and context as possible.

Pull requests
-------------

We really like to receive good pull requests for patches, new features or improvements.

Our advice is to first discuss changes, before you start working on a large pull-request (for instance, when implementing new features or significant refactoring of the code). Otherwise you risk spending time on something that won't be (directly) merged into the project.

Please adhere to the :ref:`dev_coding_conventions` used throughout the project.

To submit a pull request, follow this process:

1. `Fork the project <http://help.github.com/fork-a-repo/>`_ and clone your fork::

   $ git clone https://github.com/<your-username>/open-archaeology-data.git
   $ cd open-archaeology-data
   $ git remote add upstream https://github.com/openstate/open-archaeology-data.git

2. Always make sure you are working with a recent version. To get the latest changes from upstream::

   $ git checkout master
   $ git pull upstream master

3. Create a new topic branch (off the main project development branch) to contain your feature, change, or fix::

   $ git checkout -b <topic-branch-name>

4. Push your topic branch up to your fork::

   $ git push origin <topic-branch-name>

5. Open a `Pull Request <https://help.github.com/articles/using-pull-requests/>`_ with a clear title and description against the master branch.

.. _dev_coding_conventions:

Coding conventions
------------------

- We currently target Python 2.7 as a minimum version
- The `PEP 8 <http://legacy.python.org/dev/peps/pep-0008/>`_ styleguide is used for all Python code. 
- ... some more conventions should be added here in the future.
