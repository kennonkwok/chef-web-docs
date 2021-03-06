.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

Use the ``limits_conf`` |inspec resource| to test configuration settings in the ``/etc/security/limits.conf`` file. The ``limits.conf`` defines limits for processes (by user and/or group names) and helps ensure that the system on which those processes are running remains stable. Each process may be assigned a hard or soft limit.

* Soft limits are maintained by the shell and defines the number of file handles (or open files) available to the user or group after login
* Hard limits are maintained by the kernel and defines the maximum number of allowed file handles

Entries in the ``limits.conf`` file are similar to:

.. code-block:: bash

   grantmc     soft   nofile   4096
   grantmc     hard   nofile   63536

   ^^^^^^^^^   ^^^^   ^^^^^^   ^^^^^
   domain      type    item    value
