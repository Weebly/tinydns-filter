Plans
=====

Extended Record Types
---------------------

* `PTR`: Add different methods for generating the FQDN from the IP (direct,
  DeGroot, RFC4183, RFC2317). The support code for this is already in place,
  but a method for extending the `PTR`, `A+PTR`, and `AAAA+PTR` types needs to
  be determined.

New Record Types
----------------

* `CERT`
* `DNAME`
* DNSSEC (`DLV`, `DNSKEY`, `DS`, `NSEC`, `NSEC3`, `NSEC3PARAM`, `RRSIG`, `TA`)
* `LOC`
* `NAPTR`
* `RP`
* `SSHFP`
* `TLSA`
* `URI`

Pseudo-Record Types / Directives
--------------------------------

* C-style `#if`, `#ifdef`, `#ifndef`, `#elif`, `#else`, and `#endif` along with
  CLI arguments to pass data to the processor. Not sure the use-case yet, but
  they could prove useful.
