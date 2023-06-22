[20-06-2023]
- Initial Testing Begin
- Testing "upgrade" image built by OpenWRT from the [Installation](https://openwrt.org/toh/gl.inet/gl-e750#installation) page.
    - File Used: [openwrt-22.03.5-ath79-nand-glinet_gl-e750-squashfs-sysupgrade.bin](https://downloads.openwrt.org/releases/22.03.5/targets/ath79/nand/openwrt-22.03.5-ath79-nand-glinet_gl-e750-squashfs-sysupgrade.bin)
    - Attempted sysupgrade without keeping Settings/Configuration
        - Boots, WebUI Loads, LAN works, in LuCI WebUI
        - Woo!
        - for now we're stuck with "booting" or "updating" on the display
- uhoh it looks like WWAN is going to be more painful then I thought....
- testing with `opkg install kmod-usb-net-cdc-mbim umbim kmod-usb-serial-option kmod-usb-serial kmod-usb-serial-wwan luci-proto-qmi nano`
- use `luci-proto-qmi` for LuCI config

[22-06-2023]
- i am sick, irrelevent to the project but i feel like shit :3
- testing a custom build today, prepackaged with the tools needed for WWAN