
🎯 **Target ROM**

This patch is designed for:

MUSHA (USA)
SHA-1: 821eea5d357f26710a4e2430a2f349a80df5f2f6

Always verify your SHA-1 before applying.

---

🔧 **How to Apply**

Obtain a clean MUSHA (USA) ROM matching the SHA-1 above.

Use an IPS patching tool (e.g. Lunar IPS).

Apply the patch to the clean ROM.

---

🧪 **Tested On**

- Real Sega Mega Drive hardware

- EverDrive flash cartridge

- BlueRetro Bluetooth adapter

---

⚙ **Technical Overview**

The patch:

Redirects the controller read routine to a code cave.

Preserves original input handling.

Filters the Start "new press" bit conditionally based on A/B/C state.

Returns execution cleanly to the original flow.

Maintains original timing characteristics.

No gameplay logic is modified.

---

📜 **Disclaimer**

This patch is provided for preservation and hardware compatibility purposes.
You must supply your own legally obtained copy of MUSHA.

---

❤️ **Credits**

Reverse engineering, hardware testing, and implementation performed through collaborative debugging and real hardware validation.
