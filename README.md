This is an attempt to create a matched decompilation for Persona 2: Innocent Sin (Japan) for the PSX. The decompilation matched well in [decomp.me](https://decomp.me) with PSYQ 4.3 (gcc 2.8.0 + aspsx 2.77)

SLPS_021 sha1: `f477d5135dc515489f5caeb86ff0d4a9a6f97ce4`

Thanks to the [Sillent Hill 1 decompilation project](https://github.com/Vatuu/silent-hill-decomp) for most of the reference.

## Dependencies
You will need [splat](https://github.com/ethteck/splat) installed. Do `python3 -m pip install -U splat64[mips]`
## How to build
First, extract the game files from the game disc. You can use [mkpsxiso](https://github.com/Lameguy64/mkpsxiso) for this. Then, place `SLPS_021.00` on the root of the project. Run `make generate` and then `make`. The output will be in the `build` folder.

## TODO
- [ ] Make the project setup easier (add splat to tools/ etc)
- [ ] Write an script to disassemble the overlays that are useful to us (the D folder with bin files)
- [ ] Finish mapping all libaries function
- [ ] Finish mapping all the main executable functions
- [ ] Find where and how the game loads the overlays
- [ ] Setup splat for overlays
- [ ] ...