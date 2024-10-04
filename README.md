# Introducing the Ultimate Game Trainer, a Versatile and High-Performance Tool for Game Hacking.
## Features:

1. **Dynamic Code Injection**: Our trainer automatically injects code into memory bytes, eliminating the need for pointer addresses. It dynamically obtains new addresses with every game update.  
2. **Customizable Hotkey Combinations**: Use any combination of hotkeys without limitations, including combinations of more than four keys.  
3. **Flexible Memory Management**: Configure the trainer for NOP memory bytes or code injection to dynamically obtain addresses. Customize hotkeys for any address according to your preferences.  
4. **Comprehensive Teleport Menu**: Select a game folder containing specific game coordinates, save and load player positions with unlimited save slots, and manage saved locations in transferable and editable text files.  
5. **Dynamic Hotkey Display**: The trainer automatically displays your hotkeys and your addresses description in the GUI menu, adapting seamlessly to any game you choose.  
6. **Flexible Hotkey Modes**: Set hotkeys to hold or toggle, address value type...etc based on your requirements.  
7. **Process Name Configuration**: Write the process name in a text file to use it seamlessly with the trainer.  
8. **Automatic Address Updates**: The trainer automatically updates byte addresses in the file when the game is updated, removing the need for manual updates, unless the bytes themselves have changed. 

**Note**: Users are required to find specific game cheats independently and configure them in the text file or use 'Games tables files' for some games i made. To effectively locate the correct bytes for specific addresses in any game and to use the trainer proficiently, please refer to the instructional video that details the process of finding the opcodes for your addresses. 

**Note**: I'll add more games cheat tables in future, also don't hasitate to create your owen cheat for games using Cheat Engine and share the cheat table with us (Make sure you provide the game version).

---

## Usage:

First, please follow the instructions provided in the accompanying [video to guide](https://youtu.be/RpzsigSjH3s) you on how to use this tool. Additionally, join my [Discord server](https://discord.com/invite/jRnaeTJ) where you can ask any questions you may have about it.

---

## Note:
#### This Tool represents over five months of dedicated effort and will continue to be enhanced over time. You can try it for free for 7 days, after which you will need to purchase the permanent version for $30. Currently, there is no website for this tool, but one will be available soon. In the meantime, please contact me personally if you are interested in making a purchase.


---

## Other tools:
1. **BytesOccurrences:**
This tool is designed to determine the frequency of repeated bytes sequences within a process's memory. It is particularly useful for identifying unique bytes patterns in cases where [Cheat Engine](https://www.cheatengine.org/) may fail with longer byte sequences.
This tool might be required for our specific trainer because [Cheat Engine](https://www.cheatengine.org/) uses different method.

**Example Cheat Engine:**
- Process.exe+55DDD0 - 50 8B 07 - mov rax,[rdi]
- Process.exe+55DDF8 - 48 8D 4E C8 - lea rcx,[rsi-38]
- Process.exe+55DDCB - 83 FA FF - cmp edx,-01

If you inject at 'Process.exe+55DDF8' with [Cheat Engine](https://www.cheatengine.org/) it might generate you this bytes to make it unique: '07 48 8D 4E C8' Do you see it starts with the byte '07' which is the byte of the above address, this will not work with my trainer, for my trainer you must generate unique bytes that starts from the bytes of your target address.

**Example MyTrainer:**
- Process.exe+55DDD0 - 50 8B 07 - mov rax,[rdi]
- Process.exe+55DDF8 - 48 8D 4E C8 - lea rcx,[rsi-38]
- Process.exe+55DDCB - 83 FA FF - cmp edx,-01
  
If you want to inject at 'Process.exe+55DDF8' then you must generate unique bytes starts from '48' so you gonna use '48 8D 4E C8 83 FA' as you see its oky to add the bytes of the next address.


2. **ReadAssemblyRegistry:**
This [tool](https://www.mediafire.com/file/udpjcyp3g6jjjez/ReadAssemblyRegistry.exe/file) assists in identifying an opcode that exclusively contains the player’s address. It is capable of reading the address accessed in a registry, which includes specific opcodes such as 'rcx', 'rbx', 'edx' of the below instructions. This tool surpasses [Cheat Engine](https://www.cheatengine.org/) in that it can directly debug these registeries operands without offsets, exemplified by:


- Process.exe+55DDA8 - mov rcx,rbx
- Process.exe+55DDCB - 83 FA FF - cmp edx,-01

Conversely, Cheat Engine’s debugger is limited to indirect memory reference registers, such as: (Cheat Engine can read operands without offsets but it requires injection)

- Process.exe+55DDD0 - 50 8B 07 - mov rax,[rdi]
- Process.exe+55DDF8 - 48 8D 4E C8 - lea rcx,[rsi-38]

---

## Usage Policies:
1.**Prohibition of Use in Online Games:** The use of this trainer in online games is strictly prohibited. I bear no responsibility for any individual who employs it in online games.

2.**Strict Prohibition of Tampering:** Any attempt to tamper with, steal, or infringe upon this tool in any manner is strictly forbidden.
