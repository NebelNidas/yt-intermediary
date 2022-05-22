# Intermediary mappings

This repository contains the match information between different versions of the Android YouTube app created by the ReVanced project, as well as the "intermediary" mappings we use, that is an intermediary naming form which tries to keep names the same across versions and mapping changes.

Like most of our deobfuscation tools, this repo is forked from [FabricMC](https://github.com/FabricMC/intermediary).


## Files included in this repo
- **mappings/<mcversion>.tiny**: Intermediary mappings in the Tiny mapping format.
- **matches/*.match**: Matches between YouTube versions, created by the ReVanced project with the aid of [Matcher](https://github.com/NebelNidas/Matcher).


## Generating / updating mappings
In general, you're going to want to use the following tools:

- [Matcher](https://github.com/NebelNidas/Matcher) by sfPlayer1 (or our fork for a better decompiler) can be used to create a match file between two JARs. In addition, it can load Enigma-format mappings, which can be used as an aid in figuring out changes.
- [Stitch](https://github.com/NebelNidas/stitch) is a toolset for generating mappings based on match files. "generateIntermediary" is used to start a fresh chain of intermediary mappings, while "updateIntermediary" is used to add a new entry to the chain based on the previous entry and a matches file.


## License
As with the named mappings, we provide the intermediary mappings under the Creative Commons Zero license, so all can benefit.
