.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

The |resource user| resource is used to add users, update existing users, remove users, and to lock/unlock user passwords.

.. note:: System attributes (including user attributes) are collected at the start of every |chef client| run by |ohai|. By design, the actions available to the |resource user| resource are processed **after** the start of the |chef client| run. This means that attributes added during a |chef client| run must be reloaded before they can be made available to the |chef client|. This can be done in two ways: by picking up the values at the start of the (next) |chef client| run or by using the :doc:`ohai resource </resource_ohai>` to reload these attributes so that they can be available during the current |chef client| run.
