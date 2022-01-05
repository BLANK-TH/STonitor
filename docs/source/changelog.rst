Changelog
============
All notable changes to this project will be documented in this file.

The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_,
and this project adheres to `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.

[Unreleased]
--------------
Fixed
^^^^^^
* KeyError on invalid weapon name (MFD Detection)
* Status getting stuck wo/ ``#end``

[1.1.2] - 2022-01-01
------------------------
Fixed
^^^^^^
* Damage regex not triggering if damage was headshot

[1.1.1] - 2021-12-31
------------------------
Added
^^^^^^
* Ability to retrieve server playtime using GameME

[1.0.1] - 2021-12-31
------------------------
Added
^^^^^^
* Ability to wipe output.log on error to try to automatically resolve errors arising from corrupted logs

Changed
^^^^^^^^^^
* Exempt potential FK/FD during LR and LG instead of just LG
* TTT now uses caching similar to status and JB
* Parsed arrays are now cleared as soon as output.log is cleared to minimize unneeded memory usage

Fixed
^^^^^^^
* LR detection reporting wrong death
* IndexError in case of corrupted TTT logs
* TTT full logs not being parsed if sm_logs was run during the round to retrieve partial log

Deprecated
^^^^^^^^^^^^
* ``session.json`` is no longer used, and can be removed

[1.0.0] - 2021-12-30
------------------------
Initial release, no changes