# vpnc-script

This is a fork of the openconnect project's [vpnc-script](http://git.infradead.org/users/dwmw2/vpnc-scripts.git/) that makes the following changes:

1. Focused on macOS for use with `openconnect-keychain`.
2. Strips all non-macOS config to make it easier to grok. (`openconnect-keychain` requires macOS anyways)
2. Tweaks the Unbound config to enable its use on macOS.
3. By default, it does not allow the VPN server to set your DNS servers. (Can be re-enabled by setting `VPNSCRIPT_NODNS=0`)
4. Drops support for obsolete versions of Mac OS X (10.4 and earlier).
