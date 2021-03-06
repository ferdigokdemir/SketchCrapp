<p align="center">
  <img height="200" src="https://i.imgur.com/laXau20.png">
</p>

## SketchCrapp

Sketch.App Patch Tool, brought to you by [@duraki](https://github.com/duraki) & [@elijahtsai](https://github.com/elijahtsai). This script provides you a quick and dirty way to patch Sketch.app for Unlimited Trial. You can always patch manually using Ghidra by following [this tutorial](https://duraki.github.io/posts/o/20200214-sketch.app-patch-in-ghidra.html). Offsets available [here](https://gist.github.com/Bhavdip/76c581d7ac03bdce6d226a2e8c522df4#gistcomment-3370035).

**Download Sketch.App version of your choice here:** https://www.sketch.com/updates/

## Usage

* Open your MacOS Terminal (`Cmd+Space`, type **Terminal**)
* Type the commands below
* Download or clone this repository
  * `cd $HOME && git clone https://github.com/duraki/sketchcrapp`
* Make script executable
  * `cd $HOME/sketchcrapp && chmod +x sketchcrapp.sh`
* Run the script to patch Sketch.app
  * `cd $HOME/sketchcrapp && ./sketchcrapp.sh`

**Notice**→ The application should automatically detect your Sketch.App version. If not, you can pass `-a` argument for your Sketch.app Application Bundle.

```bash
crackb0x:SketchCrapp duraki$ ./sketchcrapp.sh -h
           __       __      __
      ___ / /_____ / /_____/ /  ___________ ____  ___
    ( _-</  '_/ -_) __/ __/ _ \/ __/ __/ _ `/ _ \/ _ \
    /___/_/\_\\__/\__/\__/_//_/\__/_/  \_,_/ .__/ .__/
                                          /_/  /_/
         Sketch.App Patch Tool (https://github.com/duraki/SketchCrapp)
         by @elijahtsai & @duraki

Usage:
./sketchcrapp [-h] [-a] <applicationPath>
Supported versions: v63.1, v64.0, v65.1, v66.1, v67.1, v67.2
```

```
crackb0x:SketchCrapp duraki$ ./sketchcrapp.sh
           __       __      __
      ___ / /_____ / /_____/ /  ___________ ____  ___
    ( _-</  '_/ -_) __/ __/ _ \/ __/ __/ _ `/ _ \/ _ \
    /___/_/\_\\__/\__/\__/_//_/\__/_/  \_,_/ .__/ .__/
                                          /_/  /_/
         Sketch.App Patch Tool (https://github.com/duraki/SketchCrapp)
         by @elijahtsai & @duraki

SketchCrapp is finding application bundle path ...
[+] Selected Sketch.app path is </Applications> (auto-detected) ... OK
[+] Selected Sketch.app version is 67.2 ... SketchCrapp starting ... OK
[+] Patching offsets for 67.2 ...
[+] Patching address at offset: 0x50a78f with value: \00
1+0 records in
1+0 records out
1 bytes transferred in 0.000035 secs (28728 bytes/sec)
[+] Patching address at offset: 0x50a792 with value: \00
1+0 records in
1+0 records out
1 bytes transferred in 0.000021 secs (47663 bytes/sec)
[+] Patching address at offset: 0x50946a with value: \00\00
2+0 records in
2+0 records out
2 bytes transferred in 0.000031 secs (64528 bytes/sec)
[+] Patching address at offset: 0x5095a9 with value: \165
1+0 records in
1+0 records out
1 bytes transferred in 0.000025 secs (39946 bytes/sec)
security: SecKeychainSearchCopyNext: The specified item could not be found in the keychain.
[+] Generating self-signed certificate ...
Generating a 521 bit EC private key
writing new private key to 'pk.pem'
-----
[+] Creating pkcs package...
[+] Importing private key and self-signed certificate
1 identity imported.
[+] Signing the patched *.app bundle. This may require sudo.
[+] If asked, enter your login password. Choose "Always Allow" to not be asked again.
    @/Applications/Sketch.app: replacing existing signature
[+] Cleaning up certificate file(s)
[+] Cleaned
[+] SketchCrapp process completed. Sketch.app has been patched :)
[+] -- Notice: 
[+] If a dialogue shows up with message: “Sketch 3.app” can’t be opened
[+] please right-click the application and select open, or go to Settings -› Security
[+] and allow opening Sketch.app application.

[+] SketchCrapp (A Sketch.app cracking tool)
[+] https://github.com/duraki/SketchCrapp [by @duraki & @elijahtsai]
```

## Issues

If you have troubles using the script, please contact the team via GitHub Issues.

---

**Build with ❤️ by [@elijahtsai](https://twitter.com/elijahtsai_) & [@duraki](https://twitter.com/0xduraki)**

> [Original idea and thread](https://gist.github.com/Bhavdip/76c581d7ac03bdce6d226a2e8c522df4)
