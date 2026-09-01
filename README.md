# Hi, I'm Scott

I build small, focused Linux utilities with an emphasis on **Btrfs, Snapper, GRUB, and system recovery**.

> **Install Linux normally. Extend it with focused tools.**

My projects improve the native Btrfs and Snapper experience without replacing the tools, configuration, or installation process provided by the distribution. Each addresses a specific gap and can be used independently or as part of a larger, repeatable workflow.

## Featured Project

### [BootPrep](https://github.com/mcsgeek/bootprep)

BootPrep is the activation layer for GRUB-based Linux systems using a nested Btrfs snapshot layout.

It prepares a selected writable snapshot for the next boot, either automatically after a Snapper rollback or through a direct activation workflow. BootPrep works with the system's existing Btrfs, Snapper, GRUB, and UEFI configuration without requiring a filesystem redesign.

## Companion Utilities

BootPrep is part of a growing collection of focused utilities. Each project has a single responsibility and can be used independently or together.

* **[snapshot-chroot](https://github.com/mcsgeek/snapshot-chroot)** – Creates a recovery chroot from a Btrfs/Snapper root snapshot, automatically detecting the last successfully booted snapshot.
* **[cleanup-bootstrap-root](https://github.com/mcsgeek/cleanup-bootstrap-root)** – Safely cleans the original bootstrap `@` root while preserving its Btrfs subvolumes.
* **[dpkg-pre-post-snapper](https://github.com/mcsgeek/dpkg-pre-post-snapper)** – Creates descriptive Snapper pre/post snapshots around Debian package transactions.
* **[add_subvolumes](https://github.com/mcsgeek/add_subvolumes)** – Converts selected root and home directories into independent Btrfs subvolumes.
* **[add_updategrub-service](https://github.com/mcsgeek/add_updategrub-service)** – Installs a systemd service that runs update-grub during system shutdown.

## Project Philosophy

I prefer tools that are:

* **Focused** – one clearly defined responsibility.
* **Native** – build on existing Linux components instead of replacing them.
* **Discoverable** – detect the system's actual configuration instead of relying on unnecessary hard-coded assumptions.
* **Safe** – validate the environment before making filesystem or boot-related changes.
* **Composable** – useful independently, but able to work together as part of a larger workflow.

If you're working with **Btrfs, Snapper, GRUB, or snapshot-based Linux system recovery**, start with [BootPrep](https://github.com/mcsgeek/bootprep), explore the companion projects above, and bring your own configurations and test cases to [BootPrep Discussions](https://github.com/mcsgeek/bootprep/discussions).
