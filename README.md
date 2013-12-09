Reverse
=======

Reverse is a backup program that with a focus on the following requirements:

* Deduplication of identical files
* Handle renames
* Allow for occasional sneakernet transfers when the size of the backup is over
  a threshold
* After the initial backup, all subsequent backups are incremental.

It backs up to a remote SFTP server.


Installation
============

```bash
apt-get install ruby ruby-net-sftp
git clone https://github.com/bragfire/reverse.git
```

Usage
=====

```bash
cd reverse
./reverse -v --source /home/user/important-stuff --dest user@server:path
```
