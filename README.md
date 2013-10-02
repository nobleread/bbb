TurnKey BigBlueButton - Video Conference Appliance
==================================================

[BigBlueButton](http:///www.bigbluebutton.org/) (BBB) is an open source web conferencing system for on-line learning. BigBlueButton enables you to share documents (PDF and any office document), webcams, chat, audio, and your desktop. It can also record sessions for later playback.

BBB is not intended as a standalone server, but to be [integrated with other systems (such as Moodle, WordPress, Drupal and others](http://www.bigbluebutton.org/open-source-integrations/) via an API. It is not recommended to install other software alongside BBB (i.e. Moodle/WordPress/Drupal/etc should be running on another server).

Requirements:
- 64 bit only (amd64)
- 2GB RAM (may run on less but not well)
- Dual Core CPU (min 2.4GHz
- Good upstream and downstream bandwidth

Recommendations:
- 4GB+ RAM
- Quad Core CPU (2.6GHz+)
- 100Mbps+ (up/down)
- 500GB Storage (for recordings)
- Bare metal install (or Server grade virtualisation)
- Static IP
- 48 hours of [Stress Testing](https://code.google.com/p/bigbluebutton/wiki/StressTesting) prior to production

AWS EC2:
- c1.medium (or greater CPU) EBS instance
- elastic IP

This appliance includes all the standard features in [TurnKey Core](http://www.turnkeylinux.org/core), and on top of that:
- BBB configurations:
    - BBB installed from upstream package repository
    - NginX front end
    - BBB API demo app preinstalled (allows creation of demo conference) - Remove before production!
    - API secret regenerated on first boot *TODO*

Credentials *(passwords set at first boot)*
-------------------------------------------

- Webmin, SSH: username **root**