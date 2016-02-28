# afl-cve
A collection of vulnerabilities discovered by the AFL fuzzer (afl-fuzz)

## Introduction
`afl-cve` is a collection of known vulnerabilities that can be attributed to the
AFL fuzzer [afl-fuzz](http://lcamtuf.coredump.cx/afl/). All vulnerabilities in
this list either already have a CVE assigned, or a CVE has been requested from a
[CVE Numbering Authority](https://cve.mitre.org/cve/cna.html#participating_cnas).

## Why is This Necessary?
Because CVE descriptions are not generally being written to mention AFL as the
tool that enabled particular bugs to be found. This is primarily due to the fact
that CVE descriptions do not require the underlying discovery tool or technique
to be disclosed. Nor should it necessarily - many security researchers have their
own methods, and it might hurt the vulnerability reporting process if researchers
were required to disclose such techniques. Further, most security researchers do
acknowledge AFL in some form (twitter post, afl-users mailing list, etc.) when
it finds a bug, and `afl-cve` attempts to track this more formally.

Also, the `afl-fuzz` website does a great job of tracking *bugs* found by AFL.
But not all bugs get assigned a CVE, and hence there is a need to specifically
track those that do because having a CVE is at least a tacit acknowledgment of
potential exploitability. So, the bugs AFL has found are therefore frequently
*important* for anyone concerned about security.

## Fuzzing Revisited
AFL has discovered a huge number of bugs in all sorts of projects from compilers
to image processing libraries. AFL seems to be succeeding where other fuzzers have
failed, or at least not been generally embraced or made operational by the security
community for whatever reason. Another way to see this is to try to determine which
fuzzer has the most CVE's. Is there a different fuzzing project that comes close to
AFL in terms of the number of vulnerabilities found? It would be instructive to see
which fuzzer comes in second place and by how much.

## The Vulnerabilities
This is likely a partial list, but please send a pull request or contact me below
to include any CVE that is not included below:

| Project / Software | CVE Number | Metasploit |
| ------------------ | ---------- | ---------- |
| bash | [CVE-2014-6277](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-6277) | NA |
| bash | [CVE-2014-6278](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-6278) | [scanner](https://github.com/rapid7/metasploit-framework/blob/master/modules/auxiliary/scanner/http/apache_mod_cgi_bash_env.rb),[exploit1](https://github.com/rapid7/metasploit-framework/blob/master/modules/exploits/multi/http/apache_mod_cgi_bash_env_exec.rb),[exploit2](https://github.com/rapid7/metasploit-framework/blob/master/modules/exploits/multi/http/cups_bash_env_exec.rb) |
| libjpeg | [CVE-2013-6629](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2013-6629) | NA |
| libpng | [CVE-2014-9495](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9495) | NA |
| BIND | [CVE-2015-5477](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5477) | NA |
| BIND | [CVE-2015-5722](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5722) | NA |
| BIND | [CVE-2015-5986](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5986) | NA |
| Xerces-C | [CVE-2015-0252](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0252) | NA |
| Xerces-C | [CVE-2016-0729](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-0729) | NA |
| ImageIO | [CVE-2015-5781](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5781) | NA |
| ImageIO | [CVE-2015-5782](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5782) | NA |
| libtiff | [CVE-2014-8127](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8127) | NA |
| libtiff | [CVE-2014-8128](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8128) | NA |
| libtiff | [CVE-2014-8129](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8129) | NA |
| libtiff | [CVE-2014-8130](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8130), [Debian Advisory](https://security-tracker.debian.org/tracker/CVE-2014-8130) | NA |
| firefox | [CVE-2014-1564](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-1564) | NA |
| firefox | [CVE-2014-1580](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-1580) | NA |
| firefox | [CVE-2014-8637](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8637) | NA |
| flash | [CVE-2015-0329](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0329) | NA |
| flash | [CVE-2015-0323](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0323) | NA |
| mutt | [CVE-2014-9116](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9116) | NA |
| clamav | [CVE-2015-1463](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1463) | NA |
| clamav | [CVE-2015-2170](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2170) | NA |
| clamav | [CVE-2015-2221](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2221) | NA |
| clamav | [CVE-2015-2222](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2222) | NA |
| X.org | [CVE-2015-1802](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1802) | NA |
| X.org | [CVE-2015-1803](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1803) | NA |
| X.org | [CVE-2015-1804](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1804) | NA |
| libwmf | [CVE-2015-0848](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0848) | NA |
| libwmf | [CVE-2015-4695](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4695) | NA |
| libwmf | [CVE-2015-4696](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4696) | NA |
| tidy | [CVE-2015-5522](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5522) | NA |
| tidy | [CVE-2015-5523](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5523) | NA |
| patch | [CVE-2014-9637](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9637) | NA |
| openssl | [CVE-2015-1788](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1788) | NA |
| openssl | [CVE-2015-0288](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0288) | NA |
| openssl | [CVE-2015-3193](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3193) | NA |
| gnutls | [CVE-2014-8564](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8564) | NA |
| libmspack | [CVE-2014-9556](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9556) | NA |
| libmspack | [CVE-2014-9732](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9732) | NA |
| libmspack | [CVE-2015-4467](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4467) | NA |
| libmspack | [CVE-2015-4468](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4468) | NA |
| libmspack | [CVE-2015-4469](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4469) | NA |
| libmspack | [CVE-2015-4470](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4470) | NA |
| libmspack | [CVE-2015-4471](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4471) | NA |
| libmspack | [CVE-2015-4472](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4472) | NA |
| Qt | [CVE-2015-1858](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1858) | NA |
| Qt | [CVE-2015-1859](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1859) | NA |
| Qt | [CVE-2015-1860](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1860) | NA |
| unace | [CVE-2015-2063](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2063) | NA |
| ARJ | [CVE-2015-2782](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2782) | NA |
| t1utils | [CVE-2015-3905](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3905) | NA |
| Android (libstagefright) | [CVE-2015-1538](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1538) | NA |
| Android (libstagefright) | [CVE-2015-1539](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1539) | NA |
| Android (libstagefright) | [CVE-2015-3824](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3824) | NA |
| Android (libstagefright) | [CVE-2015-3826](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3826) | NA |
| Android (libstagefright) | [CVE-2015-3827](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3827) | NA |
| Android (libstagefright) | [CVE-2015-3828](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3828) | NA |
| Android (libstagefright) | [CVE-2015-3829](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3829) | NA |
| antiword | [CVE-2014-8123](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-8123) | NA |
| ArduinoJson | [CVE-2015-4590](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-4590) | NA |
| CUPS | [CVE-2014-9679](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9679) | NA |
| Cap'n Proto | [CVE-2015-2310](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2310) | NA |
| Cap'n Proto | [CVE-2015-2312](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2312) | NA |
| libtasn1 | [CVE-2015-3622](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-3622) | NA |
| UnRTF | [CVE-2014-9274](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9275) | NA |
| UnRTF | [CVE-2014-9275](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9275) | NA |
| unzip | [CVE-2015-1315](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1315), [Debian Advisory](https://security-tracker.debian.org/tracker/CVE-2015-1315) | NA |
| unzoo | [CVE-2015-1845](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1845), [Red Hat Advisory](https://bugzilla.redhat.com/show_bug.cgi?id=CVE-2015-1845) | NA |
| unzoo | [CVE-2015-1846](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1845), [Red Hat Advisory](https://bugzilla.redhat.com/show_bug.cgi?id=CVE-2015-1846) | NA |
| Ghostscript | [CVE-2015-3228](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1845), [Red Hat Advisory](https://bugzilla.redhat.com/show_bug.cgi?id=CVE-2015-3228) | NA |
| GnuPG | [CVE-2015-1606](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1606) | NA |
| GnuPG | [CVE-2015-1607](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1607) | NA |
| libksba | [CVE-2014-9087](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-9087) | NA |
| Microsoft Windows | [CVE-2014-6355](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2014-6355) | NA |
| Microsoft Windows | [CVE-2015-0061](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0061) | NA |
| NTP | [CVE-2015-7855](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-7855) | NA |
| libxml2 | [CVE-2015-7941](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-7941) | NA |
| libxml2 | [CVE-2015-8035](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8035) | NA |
| libxml2 | [CVE-2015-8241](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8241) | NA |
| libxml2 | [CVE-2015-8242](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8242) | NA |
| libxml2 | [CVE-2015-8317](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8317) | NA |
| PuTTY | [CVE-2015-5309](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5309) | NA |
| PowerDNS | [CVE-2015-5311](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-5311) | NA |
| PHP | [CVE-2015-0232](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0232) | NA |
| pngcrush | [CVE-2015-2158](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-2158) | NA |
| dpkg | [CVE-2015-0860](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-0860) | NA |
| PCRE | [CVE-2015-8380](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-8380) | NA |
| LHA for UNIX | [CVE-2016-1925](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2016-1925) | NA |
| libXfont | [CVE-2015-1803](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1803) | NA |
| libXfont | [CVE-2015-1804](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2015-1804) | NA |

## Contact
All updates to the above list of CVE's are managed through any of three methods:
github issues tracking, email contact (michael.rash_AT_gmail.com), or reaching me
through Twitter ([@michaelrash](https://twitter.com/michaelrash)).
