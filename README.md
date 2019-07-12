# G-CLI-VI-Package-API
A G CLI tool for interacting with VI Package Manager

# Requirements

* LabVIEW 2011 or higher.
* VI Package Manager Pro


# VIPBuild

## Parameters

### Optional

-buildNumber: Sets the build number for the specification, keeping the others as they already are.

-versionNumber: Sets the full version number in the format "d.d.d.d"

### Required

* VIPB Path

### Example Call

g-cli --lv-ver 2018 vipBuild -- -buildNumber 4 myPackage.vipb

# VIPCApply

## Parameters

* VIPC Path
* LV Version - e.g. "2014"
* Bitness - either "64" or "32". Blank will assume 32


### Example Call

`g-cli --lv-ver 2018 vipcApply -- myDependencies.vipc 2018 32`


