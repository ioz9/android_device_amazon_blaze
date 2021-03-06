###01/16/2012:
* Added HISTORY.md

###01/17/2012:
* Renamed cyanogen_blaze.mk to cyanogen_blaze.mk.bak

###01/24/2012:
* Changed configs : set no sdcard and disabled screen-off animation (causes issues w/ certain kernels, easier to leave disabled and let people enable at their own risk depending on kernel).
* Removed recovery from values-ru (Russian I think, not sure lol; kind of odd we only have one translation).
* Created CWM branch and added recovery option back into reboot for this branch (CWM recovery by the DoomLord sets bootmode properly so no recovery loop issues).

###01/26/2012:
* Added README.md

###01/29/2012:
* Updated README.md
* Changed History layout slightly
* Updated README.md: Corrected symlinks and added an extra information section towards the end (put keyboard fix information in there, please add other fixes like this section).

###01/30/2012:
* Updated README.md: More extra information for after flash.

###01/31/2012:
* Updated README.md: Credits and discussion/build threads.

###02/01/2012:
* Changed blaze.mk; removed inherit of languages_full this is already inherited in full_base, using less_full_base.mk which I added to the build directory (this removes camera, voicedialer and protips; still looking into removing other things without causing FCs in certain apps).
* Updated README.md; can't believe I missed that. Whistlestop hasn't (may not, unsure) merged my CWM branch so to build from it we need to pull from my repos. Also corrected symlinks and added an extra information section towards the end (put keyboard fix information in there, please add other fixes like this to this section).

###01/30/2012:
* Updated README.md: more extra information for after flash.

###01/31/2012:	
* Updated README.md: Credits and discussion/build threads.

###02/01/2012:
* Changed blaze.mk; removed inherit of launguages_full this is already inherited in full_base, using less_full_base.mk which I added to the build directory (this removes camera, voicedialer and protips; still looking into removing other things without causing FCs in certain apps).
* Updated README.md; can't beleive I missed that.
* Changed blaze.mk; moved locales for mdpi to set after inheritting base.mk (fixes keyboard allowing it to load proper language on boot, en_US instead of MD_US)
* Added market permissions to allow more downloads (fix derived from sitics market fix for CM9, thank you sitic)

###02/08/2012:
* Updates made to other repos in tree effecting this device, check the [changelog](https://github.com/IngCr3at1on/android/blob/gingerbread/CHANGELOG.md) markdown for the project manifest for more information.
* Added idle/standby information to extra info.
* Updated build threads.
* Updated credits.
* **Fixed by CM** CyanogenMod broke their build, see turkish translations for [packages/apps/settings](https://github.com/CyanogenMod/android_packages_apps_Settings/blob/4f83c6a302a1af1de31fd004b555399311f8e95b/res/values-tr/strings.xml#L1391), changed in commit [4f83c6a302a1af1de31fd004b555399311f8e95b](https://github.com/CyanogenMod/android_packages_apps_Settings/commit/4f83c6a302a1af1de31fd004b555399311f8e95b). Specifically note the repeat entry of 'device_settings_title'. Added an overlay to fix this (hopefully we can remove this in the future...). **Ok, so Overlays didn't work anyway... that's what I get for not testing it as an overlay before uploading it lol... anyway just as I was in the process of forking the cm/settings repo they pushed the fix themselves, it's been 2 days so that's not too surprising I just wasn't in the mood to wait again, ironically annoying timing.**

### 02/21/2012
* Broke device and vendor directories into separate repos.
* Updated README.md: Updated to match new build information, updated support list, added to extra info and updated thanks.

### 02/22/2012
* Updated readme markdown: add in discussion thread and more extra information and thanks.
* Fix the curl repo instructions.

### 02/24/2012
* Updated readme markdown: add in pngcrush as a dependency (really google, you left that out?)

### 02/27/2012
* Fully deprecate Skimp Killahs thread and build; the domain is broken and the rom is not available (even if it were it is almost as old as the last Whistlestop build).

### 03/02/2012
* Imported needed changes to build recovery properly.
* Added recovery information to readme and updated thanks.
* Updated readme to use HTTP (this is githubs preferred delivery system and has proven to be more stable than normal git) (this has been tested by the CyanogenMod organization and I can confirm more stable syncs with this method).

### 03/14/2012
* Minor build prop changes to try to improve battery life.
