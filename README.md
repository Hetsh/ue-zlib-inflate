# ue-mod-unpack
Bash scripts for decompressing Unreal Engines .z files and generating matching .mod file.


# Usage
`inflate.sh` decompresses a `.z` file and `modgen.sh` generates the required `<mod_id>.mod` file:
```bash
$ ./inflate.sh workshop/<mod_id>/WindowsNoEditor/file.z
$ ./modgen.sh ARK/ShooterGame/Content/Mods/<mod_id> "<mod_name>"
```
More detailed examples shown in this [Dockerfile](https://github.com/Hetsh/docker-ark-modded/blob/master/Dockerfile).

# Tested
This project is designed for and tested with mods for ARK: Survival Evolved.
The following mods are tested with my [ARK docker image](https://hub.docker.com/r/hetsh/ark-modded) and confirmed working:
* [Structures Plus](https://steamcommunity.com/sharedfiles/filedetails/?id=731604991) (Mod-ID: 731604991)
* [Bridges](https://steamcommunity.com/sharedfiles/filedetails/?id=558651608) (Mod-ID: 558651608)
* [Castles, Keeps and Forts: Remastered](https://steamcommunity.com/sharedfiles/filedetails/?id=1814953878) (Mod-ID: 1814953878)
* [Castles, Keeps and Forts: Science Fiction](https://steamcommunity.com/sharedfiles/filedetails/?id=2121156303) (Mod-ID: 2121156303)
* [Super Spyglass](https://steamcommunity.com/sharedfiles/filedetails/?id=793605978) (Mod-ID: 793605978)
* [eco's Trees](https://steamcommunity.com/sharedfiles/filedetails/?id=670764308) (Mod-ID: 670764308)
* [eco's Garden Decor](https://steamcommunity.com/sharedfiles/filedetails/?id=880871931) (Mod-ID: 880871931)
* [eco's Role Play Decor](https://steamcommunity.com/sharedfiles/filedetails/?id=741203089) (Mod-ID: 741203089)
* [Rare Sightings](https://steamcommunity.com/sharedfiles/filedetails/?id=1300713111) (Mod-ID: 1300713111)
* [Olympus Map](https://steamcommunity.com/sharedfiles/filedetails/?id=970855993) (Mod-ID: 970855993)
* [Sleepable Beds](https://steamcommunity.com/sharedfiles/filedetails/?id=1650069767) (Mod-ID: 1650069767)
* [Classic Flyers](https://steamcommunity.com/sharedfiles/filedetails/?id=895711211) (Mod-ID: 895711211)
* [Immersive Taming](https://steamcommunity.com/sharedfiles/filedetails/?id=1251632107) (Mod-ID: 1251632107)

# Inspiration
This project is partially based on other work:
* `inflate.sh` <- python script in [ARK_Mod_Downloader](https://github.com/barrycarey/Ark_Mod_Downloader/blob/971e509d73cbfbac1b55b3a6bd2d8429ec612fbd/arkit.py)
* `modgen.sh` <- embedded perl script in [ark-server-tools](https://github.com/arkmanager/ark-server-tools/blob/a21496e39a4df30b7aadd6edfdc5d5297ba0a9f0/tools/arkmanager#L2749).