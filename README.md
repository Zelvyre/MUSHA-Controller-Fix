🎯 Target ROM

This patch is designed for:

MUSHA (USA)
SHA-1: 821eea5d357f26710a4e2430a2f349a80df5f2f6

Always verify your ROM’s SHA-1 before applying the patch.
It will not work correctly with other regions or modified dumps.

---

🔧 How to Apply

Obtain a clean MUSHA (USA) ROM matching the SHA-1 above.

Use an IPS patching tool (e.g. Lunar IPS).

Apply the patch to the clean ROM.

Run the patched ROM on emulator or real hardware.

---

🧪 Tested On

Original Sega Mega Drive hardware

EverDrive flash cartridge

BlueRetro Bluetooth adapter

---

⚙ Technical Overview

This patch:

Fixes unintended button presses while using BlueRetro and other wireless adapters during gameplay.

- Disables the ability to pause while holding A, B, or C, resolving the unintended pause behaviour introduced when using certain wireless controllers.
- Adds a safeguard so that if the game detects A + B + C + Start simultaneously (an input state that appears to occur intermittently due to high polling rate interactions with wireless adapters), the input is suppressed.    This prevents phantom button presses that can otherwise trigger unintended behaviour such as formation changes via the A button.

**Flash Cartridge Note**: If using flash cartridges such as EverDrive that provide an in-game menu hotkey, it is recommended to configure the menu combination to include a directional input (for example: A + B + C + Down). While this patch suppresses phantom input states within the game logic, flash cartridges that monitor controller input independently (e.g., via V-blank polling) may still detect transient input spikes at the hardware level.

---

📜 Disclaimer

This patch is provided for preservation and hardware compatibility purposes.
You must supply your own legally obtained copy of MUSHA.

---

❤️ Credits

Reverse engineering, hardware testing, and implementation performed through collaborative debugging and real hardware validation.

Special thanks to Fern for guidance and debugging support.
