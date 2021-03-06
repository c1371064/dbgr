Changelog
=========

[1.3.0] 2019-09-21
------------
Added
~~~~~
- Added spell-checker for documentation
- Possibility to hide output of recursive calls

Fixed
~~~~~
- Fixed spelling mistakes in documentation


[1.2.0] - 2019-06-16
--------------------
Removed
~~~~~~~
- Removed unused steps ``publish_test`` and ``changelog``

Added
~~~~~
- Added Sphinx documentation
- Added request headers and data to terminal output

Fixed
~~~~~
- Strip whitespaces from request name in interactive mode.
- DBGR now shows a message when ``dbgr list`` doesn't find module or request.


[1.1.0] - 2019-06-09
--------------------
Added
~~~~~
- Added example with slow responding server to examples

Changed
~~~~~~~
- Achieved 100% code coverage. Build now requires coverage to pass.
- Python requirement relaxed to >= 3.6.


[1.0.6] - 2019-06-07
--------------------
Added
~~~~~
- Added support for calendar types ``datetime.datetime``, ``datetime.time``, ``datetime.date``.
- Added ``CHANGELOG.md``.


[1.0.5] - 2019-06-03
--------------------
Fixed
~~~~~
- The session object is not closed after each request in interactive mode.


[1.0.4] - 2019-06-02
--------------------
Fixed
~~~~~
- Dbgr doesn't crash when default argument cannot be converted to annotated type.

Changed
~~~~~~~
- Arguments ``env`` and ``session`` are now optional in ``dbgr.response``.
- Methods annotated with ``@dbgr.request`` don't have to accept ``env`` and ``session`` arguments if they don't need them.

Added
~~~~~
- In ``dbgr --list-environments`` the default argument is now highlighted.
- Added command to review all variables in environment: ``dbgr e <env_name>``


[1.0.3] - 2019-05-31
--------------------
Added
~~~~~
- Enabled listing of individual requests with ``dbgr list module:request``.
- Added ``secret`` type for password inputs from terminal.


[1.0.2] - 2019-05-28
--------------------
Fixed
~~~~~
- Fix issue where recursive calls via ``dbgr.response`` didn't pass extra arguments to request.

Added
~~~~~
- Added developer documentation file ``CONTRIBUTORS.md``.


[1.0.1] - 2019-05-27
--------------------
Fixed
~~~~~
- Re-enabled terminal autocomplete.

Added
~~~~~
- Added ``dbgr --version`` to display software version.


[1.0.0] - 2019-05-25
--------------------
Initial release.
