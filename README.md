#README for pam_nfc

<!---
[![start with why](https://img.shields.io/badge/start%20with-why%3F-brightgreen.svg?style=flat)](http://www.ted.com/talks/simon_sinek_how_great_leaders_inspire_action)
--->
[![GitHub release](https://img.shields.io/github/release/elbosso/pam_nfc/all.svg?maxAge=1)](https://GitHub.com/elbosso/pam_nfc/releases/)
[![GitHub tag](https://img.shields.io/github/tag/elbosso/pam_nfc.svg)](https://GitHub.com/elbosso/pam_nfc/tags/)
[![GitHub license](https://img.shields.io/github/license/elbosso/pam_nfc.svg)](https://github.com/elbosso/pam_nfc/blob/master/LICENSE)
[![GitHub issues](https://img.shields.io/github/issues/elbosso/pam_nfc.svg)](https://GitHub.com/elbosso/pam_nfc/issues/)
[![GitHub issues-closed](https://img.shields.io/github/issues-closed/elbosso/pam_nfc.svg)](https://GitHub.com/elbosso/pam_nfc/issues?q=is%3Aissue+is%3Aclosed)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/elbosso/pam_nfc/issues)
[![GitHub contributors](https://img.shields.io/github/contributors/elbosso/pam_nfc.svg)](https://GitHub.com/elbosso/pam_nfc/graphs/contributors/)
[![Github All Releases](https://img.shields.io/github/downloads/elbosso/pam_nfc/total.svg)](https://github.com/elbosso/pam_nfc)

pam_nfc is a NFC-based PAM authentification module.

Using pam_nfc, you can use NFC (Near Field Communication) cards / tags to
autohrise users into PAM (Pluggable Authentication Modules).

#Security consideration

Since tag IDs cannot be trusted, you SHOULD not only rely on them to grant
access to the machine to users.  You SHOULD only consider this PAM module as a
convenient way for a user to tell his own machine who he is.

Basically, the NFC reader is physically connected to the computer, so if an
user has a physical access to the NFC intiator, he also has physical access to
the computer, and thus strong authentification is already of no luck.
