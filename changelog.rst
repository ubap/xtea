Changelog
---------

Version 0.6.0; Oct 16, 2016
~~~~~~~~~~~~~~~~~~~~~~~~~~~

[0.6.0] Made Python 3 compatible | removed counters can return integers | cipher objects remember state

 - Python 3 does work now
 - [BREAKING CHANGE] counters cannot return numbers any more, they must return bytestrings now
 - [BREAKING CHANGE] Cipher objects remember change, so two consecutive calls to XTEA.encrypt should not return the same
 - improved documentation

Version 0.5.0; Oct 15, 2016
~~~~~~~~~~~~~~~~~~~~~~~~~~~

[0.5.0] Removed CBCMAC

Version 0.4.1; Jul 30, 2015
~~~~~~~~~~~~~~~~~~~~~~~~~~~

[0.4.1] Fixed installer

Version 0.4.0; Jul 12, 2014
~~~~~~~~~~~~~~~~~~~~~~~~~~~

[0.4.0] Buggless & PEP compliant CTR | added CBCMAC

 - CTR mode works with strings now
 - raises DeprecatedWarning if a number is returned
 - CBCMAC class added (use static method CBCMAC.new(args) to create)

Version 0.3.2; Jul 11, 2014
~~~~~~~~~~~~~~~~~~~~~~~~~~~

[0.3.2] Minor Fixes

Version 0.3.1; Jul 11, 2014
~~~~~~~~~~~~~~~~~~~~~~~~~~~

[0.3.1] Minor Fixes

 - Fixed that the length of data will not be checked

Version 0.3.0; Jul 11, 2014
~~~~~~~~~~~~~~~~~~~~~~~~~~~

[0.3.0] Added CFB mode

 - Added CFB mode
 - Fully working with PEP 272
 - Raising NotImplementedError only on PGP-CFB (OpenPGP) mode
 - Wheel support and changelog (0.2.1)

Version 0.2.1 - dev; Jul 10, 2014
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Never released...

 - Added better wheel support for uploading (just for me) with a setup.cfg
 - Added this file (auto uploading on pypi/warehouse and github)
 - (upload.py for github)

Version 0.2.0; Jul 9, 2014
~~~~~~~~~~~~~~~~~~~~~~~~~~

[0.2.0] Added a test feature; warning in CTR

 - Added a test feature
 - Raises warning on CTR, added a handler that CTR will not crash anymore ;) 

Version 0.1.1; Jul 9, 2014
~~~~~~~~~~~~~~~~~~~~~~~~~~

[0.1.1] NotImplementedError on CFB

 - Module raises a NotImplementedError on CFB
 - Minor changes

Version 0.1; Jun 22, 2014
~~~~~~~~~~~~~~~~~~~~~~~~~

[0.1] Initial release

 - Supports all mode except CFB
 - Buggy CTR ( "�" = "\\xc3\\x9f" )
 - Working with PEP 272, default mode is ECB
