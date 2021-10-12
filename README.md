# Remote Code Execution via a crafted mkp file

**Application:** CheckMK Management Web Console

**Software Revision:** Less than or equal to 2.0.0p11

**Attack type:** RCE

**Solution:** TBD or the MKPs shared on [https://exchange.checkmk.com/] are manually reviewed by CheckMk and they look for malicious code or suspicious imports, etc.

**Summary:** The web management console of CheckMk Enterprise Edition (versions 1.5.0 to 2.0.0p11) does not properly sanitise the uploading of ".mkp" files which are Extension Packages, making remote code execution possible. Successful exploitation requires access to the web management interface, either with valid credentials or with a hijacked session of a user with administrator role.

**Technical Description:** TBD

**Timeline:**
   * 2021-09-01 Issues discovered.
   * 2021-09-06 First contact with vendor via e-mail.
   * 2021-09-08 Vendor response. RCE vulnerabilities were already detected, and would be patched in the next release.
  

**Reference:**
   * https://exchange.checkmk.com/

# DEMO
  **PoC CheckMk version 2.0.0p11 Enterprise Edition**
