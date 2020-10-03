# VyOS Easy Deployment Template

## Synopsis

Provide a base configuration to "jump-start" VyOS with supporting configuration, to allow easy automated templating and deployment.

### This Will

- Set up interface `eth0` as a DHCP client
- Set up VRF `mgmt` to keep eth0 separate. This will allow consumers to keep an easy, automatically bootstrapped out-of-band point of administration.
- Set up SSH/API for remote administration once it's on-line

## To use these examples

- Perform a new VyOS installation: <https://docs.vyos.io/en/latest/install.html>
- Install the provided configuration into that virtual router
- Update VyOS (if applicable), and load any custom software.
- Package into OVA or VM Template
- Deploy everywhere!

From there, it's possible to perform get and post invocations.

## Tested Platforms

- VyOS Rolling

## TODO

- IPv6

## Notes

- Set a date every time you re-build this router for easy checking.
- Set your own password - that is not included in this configuration.
- Cleaning up the log file will save space. VyOS logging is extremely straightforward, with input primarily going to `/var/log/messages`.
  - `echo "" > /var/log/messages`
  - <https://wiki.vyos.net/wiki/Logging>

## Authors

- *Nick Schmidt*
