tinydns-filter
==============

A filter for tinydns data files allowing for more natural use of TXT records
and adding support for AAAA, CAA, SPF (type 99), SRV, and ALIAS records.

Copyright and License
---------------------

Copyright (c) 2016 [Weebly, Inc](http://weebly.com), All Rights Reserved

This software is licensed under the BSD 3-Clause License; included with this
program in LICENSE.md.

Author
------

Jeff Walter (jwalter@weebly.com, http://jwalter.weebly.com)

Contributors
------------

_None yet_

Features
--------

### Extended Records

* `TXT`: Wrap record rdata in double-quotes to avoid escaping most characters.

### New Records

* `AAAA`: Record types for just a AAAA and AAAA with a PTR
* `CAA`: A Certification Authority Authorization record for when you run your
         own PKI
* `SPF`: A type 99 SPF record (deprecated, but still supported by some mail
         transfer agents)
* `SRV`: Service record for SIP, XMPP, and other services

### New Pseudo-Records

* `ALIAS`: A `CNAME`-like pseudo record that copies the records of the target
           and changes the hostname to the FQDN in the `ALIAS` record.

Requirements
------------

* Perl 5.x (untested under Perl 6.x)

Contributing
------------

To contribute simply:

1. Fork [weebly/tinydns-filter](https://github.com/weebly/tinydns-filter)
2. Make your changes (please use a lot of comments and make use of the existing
   coding style)
3. Commit
4. Push
5. Open pull request

Your changes **MUST** not touch:

* Any part of the copyright notice
* Any part of the license
* `$NAME`, `$VERSION`, `$COPYRIGHT`, `$OWNER`, `$AUTHOR`, or `@CONTRIBUTORS`

Your pull request message **SHOULD** include (at minimum):

* What problem it solves or what feature it adds
* What the code does
* How the code should work
* How the user will utilize the fix/feature
