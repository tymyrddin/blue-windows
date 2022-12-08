Hardening Windows
================================================

Version 0.1: These mitigations are all based on Windows 10.
Supposedly, `Windows 11 has better security <https://www.thewindowsclub.com/new-security-features-in-windows-11>`_.
Some of these mitigations are still applicable and useful.
When we have an 11 (waiting for a key) we will test it, and add mitigations.

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Accounts and authentication

   docs/authentication/README.md
   docs/authentication/login.md
   docs/authentication/resuming.md
   docs/authentication/passwords.md
   docs/authentication/password-manager.md
   docs/authentication/mfa.md
   docs/authentication/standard-user.md
   docs/authentication/ssh-mfa.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Services and applications

   docs/services/README.md
   docs/services/restrict-services.md
   docs/services/restrict-access.md
   docs/services/block-internet-access.md
   docs/services/max-uac.md
   docs/services/odd-applications.md
   docs/services/browsers.md
   docs/services/messaging.md
   docs/services/email-services.md
   docs/services/ssh.md
   docs/services/vpn.md
   docs/services/vpn-fail-open.md
   docs/services/dns-servers.md
   docs/services/tor-proxy.md
   docs/services/change-mac.md
   docs/services/renew-lease.md
   docs/services/edit-hosts-file.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Data

   docs/data/README.md
   docs/data/restore-point.md
   docs/data/disk-encryption.md
   docs/data/file-encryption.md
   docs/data/cfa.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Privacy

   docs/privacy/README.md
   docs/privacy/location-tracking.md
   docs/privacy/ad-tracking.md
   docs/privacy/devices.md
   docs/privacy/metadata.md
   docs/privacy/metadata-images.md
   docs/privacy/hexeditors.md
   docs/privacy/bleachbit.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Malware

   docs/malware/README.md
   docs/malware/clean-machine.md
   docs/malware/clean-registry.md
   docs/malware/analysing-trojans.md

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Operations security

   docs/opsec/README.md
   docs/opsec/email-use.md
   docs/opsec/check-mail.md
   docs/opsec/browsing.md
   docs/opsec/integrity-downloads.md
   docs/opsec/*

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Guards! Guards!

   docs/guards/README.md
   docs/guards/soup.md
   docs/guards/*

.. toctree::
   :caption: Links

   Blue Team <https://blue.tymyrddin.dev/>
