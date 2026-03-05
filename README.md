# a54-twrp
Untested TWRP Image for the Samsung Galaxy a54 Device
Here is that information formatted as a clean, professional Markdown table ready for your GitHub **README.md**:

## Compatible Devices (Samsung Galaxy A54 5G)

| Model Number | Region | Chipset | Bootloader Status |
| --- | --- | --- | --- |
| **SM-A546B** | Global / Europe | Exynos 1380 | ✅ Unlockable |
| **SM-A546E** | Asia / Middle East | Exynos 1380 | ✅ Unlockable |
| **SM-A5460** | China / Hong Kong | Exynos 1380 | ✅ Unlockable |
| **SM-A546S** | South Korea (Quantum 4) | Exynos 1380 | ✅ Unlockable |
| **SM-A546M** | Latin America | Exynos 1380 | ✅ Unlockable |
| **SM-A546U / U1** | USA (Carrier / Unlocked) | Exynos 1380 | ❌ **Locked (No TWRP)** |
| **SM-A546W** | Canada | Exynos 1380 | ❌ **Locked (No TWRP)** |
| **SM-A546V** | Verizon USA | Exynos 1380 | ❌ **Locked (No TWRP)** |

---

### Important Notes for Users:

* **USA/Canada Models:** If you own a **U, U1, W, or V** model, the bootloader is permanently locked by the carrier. **Do not attempt** to flash this recovery, as Odin will fail with a "Block by FAP/OEM Lock" error.
* **OEM Unlocking:** For all unlockable models, you must first enable **Developer Options** and toggle **OEM Unlocking** to the "On" position before entering Download Mode.
* **Knox Warranty:** Remember that flashing a custom recovery will permanently trip your Knox fuse (0x1), which disables Samsung Pay and Secure Folder forever.

🛠️ Build Yourself
If you want to compile this TWRP image manually using GitHub Actions, follow these steps:

Fork this Repository: Click the Fork button at the top right of this page to create your own copy.

Switch Branch: Navigate to the specific branch for the version you want to build (e.g., v12.1-a54x).

Setup Workflow:

Ensure the recovery_build.yml file is located in the .github/workflows/ directory of your repository.

If you are starting a new repo, manually create the folder path: .github/workflows/ and upload the YAML file there.

Enable Actions: Go to the Actions tab in your GitHub repository and click "I understand my workflows, go ahead and enable them."

Run the Build:

Select the "Recovery Build" workflow from the left sidebar.

Click the Run workflow dropdown menu.

Select your branch and click the green Run workflow button.

[!TIP]
Once the build finishes (usually 45-60 minutes), the flashable recovery.tar will be available for download in the Artifacts section at the bottom of the summary page.
