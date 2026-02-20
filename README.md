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

Redirects the controller read routine to a code cave.

Preserves the original input handling logic.

Conditionally filters the Start "new press" bit when A/B/C are held.

Returns execution cleanly to the original flow.

Maintains original timing behaviour.

No gameplay logic, physics, or audio routines are modified.

---

📜 Disclaimer

This patch is provided for preservation and hardware compatibility purposes.
You must supply your own legally obtained copy of MUSHA.

---

❤️ Credits

Reverse engineering, hardware testing, and implementation performed through collaborative debugging and real hardware validation.

Special thanks to Fern for guidance and debugging support.
