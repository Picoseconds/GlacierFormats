# GlacierFormats
GlacierFormats is a project to create human-readable schemas with [Kaitai Struct](https://kaitai.io/) for as many Glacier Engine resource formats as possible, and to create code in multiple languages to write these formats.

## Converters
Converters from Glacier Engine formats to more commonly-used formats such as GLTF or wav files will be added in this repository with converters from those formats to Glacier Engine resource files (for asset replacement mods).

## Supported formats
### RPKGv2
GlacierFormats has almost full support for the RPKG v2 files used in HITMAN III, including patch files. JavaScript samples to read and write files by hash and name from any .rpkg file are present in examples/.
There is also support for automatically converting these files to TAR/GZIP files for easy distribution.

### PRIM (mesh primitive)
GlacierFormats has rudimentary support for reading (but not writing) Glacier PRIM model files, and a one way converter to GLTF files is available at examples/converters/prim2gltf.js.

### XTEA-encrypted packagedefinition.txt files
A sample in JavaScript decrypting and modifying packagedefinition.txt filesis available in examples/xtea.js.

### RTLV subtitle files
RTLV files containing subtitles can be read and written with the tools in this repo. The files can be converted to video subtitle files in the WebVTT and SRT formats.
