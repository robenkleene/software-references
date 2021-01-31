# Time Machine

When files are deleted, they are immediately moved to local Time Machine backups, so you don't immediately get back the disk space. These local backups are to make deleted files accessible for 24 hours, even without access to the Time Machine drive.

To reclaim the disk space immediately, run:

    tmutil thinlocalsnapshots / 10000000000 4

(The parameters are 10 GB purge amount and priority 4.)
