# a16x-twrp

**Untested TWRP Image for the Samsung Galaxy A16 5G (Exynos Variant)**


---

## Compatible Devices (Samsung Galaxy A16 5G - Exynos 1330)

| Model Number | Region | Chipset | Bootloader Status |
| --- | --- | --- | --- |
| **SM-A166B** | Global / Europe | Exynos 1330 | ✅ Unlockable |
| **SM-A166E** | Asia / Middle East | Exynos 1330 | ✅ Unlockable |
| **SM-A166M** | Latin America | Exynos 1330 | ✅ Unlockable |
| **SM-A166U / U1** | USA (Carrier / Unlocked) | Exynos 1330 | ❌ **Locked (No TWRP)** |
| **SM-A166W** | Canada | Exynos 1330 | ❌ **Locked (No TWRP)** |

> [!NOTE]
> This repository is specifically for the **Exynos 1330 (a16x)** variant. If you have the MediaTek (Dimensity 6300) version, this recovery will not boot. Check your model number in **Settings > About Phone** before proceeding.

---

### Important Notes for Users:

* **Bootloader Unlock:** You must have an unlockable model (B, E, or M). USA and Canadian models are traditionally locked and cannot flash custom binaries.
* **OEM Unlocking:** You must enable **Developer Options**, toggle **OEM Unlocking** to "On," and then perform the long-press Volume Up process in Download Mode to fully unlock the bootloader.
* **VBMETA Requirement:** To boot this recovery, you **must** flash a patched `vbmeta.img` with verification disabled. Failing to do so will result in a "Security Check Fail" or boot loop.
* **Knox Warranty:** Flashing this will permanently trip your Knox bit (0x1). This disables Samsung Pay, Secure Folder, and Samsung Pass forever.

---

### 🛠️ Build Yourself

If you want to compile this TWRP image manually using the integrated GitHub Actions workflow:

1. **Fork this Repository:** Click the **Fork** button to create your own copy.
2. **Enable Actions:** Go to the **Actions** tab and click "I understand my workflows, go ahead and enable them."
3. **Run the Build:**
* Select the **"Recovery Build"** workflow from the left sidebar.
* Click the **Run workflow** dropdown.
* Ensure the inputs match your device (Default: `a16x`).
* Click the green **Run workflow** button.



> [!TIP]
> After the build completes (approx. 45-60 minutes), the `recovery.img` or `recovery.tar` will be available in the **Artifacts** section or the **Releases** page of your fork.

---
