.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

|reporting| is automatically enabled in the |chef client| (version 11.6.0 or later).  In order to check
if reporting data is being sent, you can check the output of the chef client INFO logging level for the
log message confirming the data has been sent.   At the end of the run:

   .. code-block:: bash

    $ chef-client -l info
    ...
    ...
    [date] INFO: Chef Run complete in 1.069059018 seconds
    [date] INFO: Running report handlers
    [date] INFO: Report handlers complete
    Chef Client finished, 2 resources updated
    [date] INFO: Sending resource update report (run-id: 51ceb817-ba7e-47e5-9bca-096fe9ef9740)

This includes the run id of the run, which can be used in the |subcommand knife reporting| plugin or the
management console to access the reporting information generated during the run.
