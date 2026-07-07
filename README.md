# Rayman Raving Rabbids: TV Party Decompilation
Decompilation of Rayman Raving Rabbids: TV Party for the Wii.

**(THIS DOES NOT INCLUDE THE ASSETS FROM THE GAME. UBISOFT WOULD KILL US FOR THAT.)**

You should preferably use USA Rev 1 (https://redump.info/disc/70511) when extracting assets. Rev 0 and other regions have not been tested.

# How?
When Rayman Raving Rabbids: TV Party (the game you're looking at right now) was shipped, Ubisoft failed to strip the debugging symbols from the disc.

This resulted in it shipping with ELF files named "EnjimeWii_NO*_g.elf" (* depends based on the disc's region; a USA disc will have an A (NOA), Europe, Japan and Korea discs have currently not been checked). Those ELF files can be opened in Ghidra using an extension like https://github.com/cuyler36/ghidra-gamecube-loader. (hey, it also works for Wii games, despite being called "Ghidra-***GameCube***-loader")

They also did not strip the symbols when releasing Revision 1 (the revision this decompilation is based off of).

# What else?
The game stores it's Flash (actually [Scaleform GFx](https://en.wikipedia.org/wiki/Scaleform_GFx) but whatever) files in a BIN file inside it's BF file named "FlashPackages.bin". The 2D assets used in the game... (including the ones shown below:)
<img width="1920" height="990" alt="Screenshot of American Choppy's instructions (with an idiot rabbid on the right)" src="https://github.com/user-attachments/assets/08e16f56-5190-41ea-b7eb-eeb91a85f13a" />
<img width="1920" height="990" alt="Cool Rabbid!" src="https://github.com/user-attachments/assets/3bc08158-6e25-451a-9da0-3e339eb09f69" />
...are really just Adobe Flash files. Dolphin cannot dump the textures from these scenes, so a program like JPEXS must be used. They must manually be carved out using a tool like QuickBMS.

# NO AI.
This decompilation does not accept AI-generated/LLM content. Your code !!!MUST!!! be human-made. Or Rabbid-made. One of those, anyways. As long as it's not made with Claude (which some decompilations are guilty of), Gemini, ChatGPT, DeepSeek, etc, it'll be accepted.

Content from this creature will also not be accepted:

<img width="203" height="196" alt="Beep-O" src="https://github.com/user-attachments/assets/600c43e5-1ae2-4a9e-b8ef-fd8c07d83776" />
