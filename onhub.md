# Objective
Install OpenVPN client on Google OnHub router. 2 potential routes to investigate:
1. Root to gain access on the device, then install via ssh
1. Create a custom image in VM to test, then load it to device

## Observations
- The rooting procedures between Google OnHub and Google Wifi router differ very little, namely
  - Newer Google Wifi routers need a USB-C adapter to both supply power, attaching USB keyboard and USB drive.
  - Older rooting procedure by _exploiteers_ appears to have been automated into the newer _galeforce_ script. Hence no need for USB keyboard and CTRL+D in the beginning. (Need confirmation)
- Unlike Google Wifi mesh router (gale) which lacks the board, both TP-Link and Asus manufactured OnHub routers (Whirlwind and Arkham, respectively) have published base board (Storm), which _may_ allow building Chromium OS from source.

## References
- Chrome OS Build Instructions (Chromium OS on Linux) ([chromium.googlesource.com](https://chromium.googlesource.com/chromium/src/+/master/docs/chromeos_build_instructions.md)) 
- Checking out and building Chromium on Linux ([chromium.googlesource.com](https://chromium.googlesource.com/chromium/src/+/master/docs/linux_build_instructions.md))
- Developer Information for Chrome OS Devices ([chromium.org](https://www.chromium.org/chromium-os/developer-information-for-chrome-os-devices))
- OpenVPN on Chrome OS ([chromium.org via Google Docs](https://docs.google.com/document/d/18TU22gueH5OKYHZVJ5nXuqHnk2GN6nDvfu2Hbrb4YLE/pub))
- Rooting The Google OnHub ([exploitee.rs](https://www.exploitee.rs/index.php/Rooting_The_Google_OnHub))
