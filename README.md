# hackintosh-x454lab
## Intro
![About This Mac](https://cdn.discordapp.com/attachments/974199826063425556/1046725810524004362/Screen_Shot_2022-11-28_at_4.53.35_PM.png)

|          | Version                 |
|----------|-------------------------|
| OpenCore | 0.8.6                   |
| macOS    | Mojave 10.14.6 |

- Supported macOS versions: High Sierra, Mojave, Catalina (Big Sur and above has not been tested)

## Info / Disclaimer
### Info
- This is just a quick config that I whipped up in like, 15 minutes for fun, with many unfixed issues. Probably not suited for daily use.
- `boot-args` used: `-v keepsyms=1 debug=0x100 alcid=3`
- `alcid`: `3`
- Recommended SMBIOS: `MacBookAir7,2`
### Usage
- You can use it however you like, except for commercial purposes (such as work enviroments and reselling your Hackintosh), refer to the [Psystar case](https://en.wikipedia.org/wiki/Psystar_Corporation). TLDR, you'll get your ass sued if you do so.
- Reminder that this is only a base for your OpenCore setup, it is strongly recommended that you follow the entire OpenCore guide [here](https://dortania.github.io/OpenCore-Install-Guide/)
- There will be differences probably even for the same line of machine, however if you're feeling lazy I guess you can just copy the config, just remember to add in information such as the MLB or the ROM in `PlatformInfo` (please don't use mine), and try to use different Apple IDs if you're booting multiple macOS verions on the same PlatformInfo as my account got flagged sus by not doing so.
- Remember to disable Apple Secure Boot before installing any version older than Big Sur (Enabled by default).
### Issues
- Sleep doesn't work (can't really test anyway because my power button is wacky)
- Audio over HDMI not tested
- Most kexts are DEBUG versions
- Card reader doesn't work
- Touchpad doesn't work (probably fine since it's trash anyway)
- No Bluetooth
- No brightness control using hotkeys
### Notes
- Don't use case-sensitive APFS if you want to use Steam or Adobe tools.
- After installation, open System Preferences and go to Displays -> Color, uncheck `Show profiles for this display only`, then select `sRGB IEC61966-2.1`, this will make your colors look *somewhat* right (definitely not calibrated or anything but yeah, not an oversaturated mess)
 
![color](https://media.discordapp.net/attachments/885809091459575828/966112499487346718/unknown.png)
## Hardware
- CPU: Intel Core i3-5005U (2c/4t, 0.8/2.0GHz, 3MB L3 cache)
- iGPU: Intel HD Graphics 5500
- RAM: 4GB DDR3 1600MHz
- Storage: Seagate 500GB HDD (use an HDD if you want pain)
- WiFi: Qualcomm Atheros AR9485
- Bluetooth: Qualcomm
- Audio: Connnexant smth (i forgor 💀)

## Credits
Special thanks to:
- [acidanthera](https://github.com/acidanthera) - the maker of OpenCore and your favourite kexts, for making this Hackintosh possible in the first place
- [dortania people](https://github.com/orgs/dortania/people) for the OpenCore Install Guide