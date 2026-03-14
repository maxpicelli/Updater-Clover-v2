# Updater Clover Tutorial

## Overview

Updater Clover is a macOS app used to update essential Clover files on an EFI partition, create full backups, restore EFI backups, and inspect system information.

## Language and theme

- `BR` switches the interface to Brazilian Portuguese.
- `EN` switches the interface to English.
- The theme buttons let you use light mode, dark mode, or the system setting.

## Update Clover tab

This is the main area for Clover updates.

### What the app updates

The app copies only the files required for a safe update:

- `EFI/BOOT/BOOTX64.efi`
- `EFI/CLOVER/CLOVERX64.efi`
- `ApfsDriverLoader.efi`
- `OpenRuntime.efi`
- `VBoxHfs.efi`

In full mode, it also syncs:

- `EFI/CLOVER/tools`

### Expected source layout

The app first looks for drivers in:

```text
EFI/CLOVER/Drivers/Off/UEFI
```

If the source is a simple backup containing only the `EFI` folder, it also accepts:

```text
EFI/CLOVER/Drivers/UEFI
```

### How to use it

1. Click `Select Clover v2` to choose an extracted folder or a `.zip` file.
2. Select the desired EFI partition.
3. Mount the EFI if needed.
4. Choose the update mode.
5. Run the update.

## EFI Backup tab

This area is used to browse saved backups and restore an EFI.

### Features

- list backups in `~/EFI_BACKUPS`
- refresh the backup list
- open the backups folder
- copy a backup path
- restore a backup to the selected EFI

### How to restore

1. Open the `EFI Backup` tab.
2. Select a valid backup from the list.
3. Choose the correct EFI partition.
4. Run the restore action.

## Info System tab

Shows a summary of hardware and current boot status.

### Displayed information

- current bootloader
- selected EFI
- EFI partition
- macOS version
- Mac model
- CPU
- GPU
- memory
- main disk
- external disks

### Screenshot

Hover over the information icon and click it to save a screenshot of the `Info System` screen to the `Downloads` folder.

## Open Sym

The `Open Sym` button opens the `sym` folder configured in the app.

If the folder has not been authorized yet, select it again when the app asks.

## Administrative permission

Some actions require an administrator password to mount or modify the EFI.

### What you may see

- the app may show its own password prompt
- macOS may show a native Keychain Access prompt

That system prompt follows the user's macOS language.

## Donation

The donation button opens the PayPal link configured in the app with the suggested amount of `US$ 4.99`.

## Important tips

- always confirm the target EFI before updating or restoring
- keep backups in `~/EFI_BACKUPS`
- use the `Info System` tab to verify the current boot state before changing the EFI
- if something looks wrong, close the app and confirm the selected source

## Troubleshooting

### EFI not found

- refresh the list
- confirm the disk is connected
- check whether the EFI is already mounted

### sym folder not found

- select the `sym` folder again
- confirm the path still exists

### The app opened in Portuguese and I want English

- click `EN`

### The tutorial did not open

- close and reopen the app
- make sure you are using the latest compiled version
