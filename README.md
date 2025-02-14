A 5E compatible system that can be used inside your own Renpy project by downloading this repo and extract it in your "Game" folder

# LICENSES:
* The content of the [game](game/) folder is under GNU GPL 3 License
* The [sheet_5e folder](sheet_5e/) is a fork of [this project](https://github.com/tassaron/dnd-character) by [tassaron](https://github.com/tassaron), and it comes with its own license.
* This work includes material taken from the System Reference Document 5.1 (“SRD 5.1”) by Wizards of the Coast LLC and available at https://dnd.wizards.com/resources/systems-reference-document. The SRD 5.1 is licensed under the Creative Commons Attribution 4.0 International License available at https://creativecommons.org/licenses/by/4.0/legalcode.
* The [Creative Commons Attribution 4.0 International License (“CC-BY-4.0”)](SRD_CC_v5.1.pdf) mainly refers to the content of the [json_data_5e folder](json_data_5e/) and the content of [5e_system.rpy file](game/5e_system.rpy) which implements game mechanics heavily inspired by the SRD5 document. For more informations, please refer to this page: https://www.dndbeyond.com/resources/1781-systems-reference-document-srd

# CREDITS:
A special thanks to:
* [tassaron](https://github.com/tassaron) for the very useful python library to manage 5e characters sheets

# NOTES:
* The 5e_system.rpy must be put inside the "Game" folder. The sheet_5e and json_data_5e folders can be placed in the Renpy base folder or inside the "Game" folder, on PC it will work anyway, BUT for Android builds...
* For Android builds: put the sheet_5e and json_data_5e folders inside "renpy-*.*.*-sdk\lib\python3.*" so that the Renpy Android packager can properly add it among the python libraries that will be packaged in the APK file. Do not put it inside the "game" directory, otherwise the build will search it there during execution but will not find the json cache files inside, because for some reasons they are not packaged together with it, returning an error. If it still refuse to work, try deleting all the content of renpy-*.*.*-sdk\tmp.
