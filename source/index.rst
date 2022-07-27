Windows PC mitigations
================================================

Version 0.1: These mitigations are all based on Windows 10. Supposedly, `Windows 11 has better security <https://www.thewindowsclub.com/new-security-features-in-windows-11>`_. Some of the below is still applicable and useful. When we have an 11 we will test it, and split and update these mitigations.

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
   docs/authentication/standard-user.md

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

.. toctree::
   :glob:
   :maxdepth: 1
   :includehidden:
   :caption: Data

   docs/data/README.md
   docs/data/restore-point.md
   docs/data/disk-encryption.md
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
   :caption: Social engineering

   docs/social-engineering/README.md
   docs/social-engineering/browsers.md
   docs/social-engineering/check-mail.md

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

   All mitigations <https://tymyrddin.github.io/mitigations/>
