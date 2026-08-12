# Hi, I'm Scott

I build small, focused Linux utilities for Debian, Ubuntu, and their derivatives, with an emphasis on **Btrfs, Snapper, GRUB, and system recovery**.

My current work focuses on improving the native Btrfs and Snapper experience without replacing the tools and workflows already provided by the distribution.

## BootPrep

**[BootPrep](https://github.com/mcsgeek/bootprep)** is my flagship project.

BootPrep is a lightweight boot preparation layer for Debian, Ubuntu, and their derivatives using Btrfs and Snapper.

It is designed to work alongside native tools such as **Btrfs, Snapper, GRUB, and grub-btrfs**, handling the additional boot preparation needed after snapshot operations.

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

If you're working with **Debian, Btrfs, Snapper, GRUB, or snapshot-based system recovery**, take a look at [BootPrep](https://github.com/mcsgeek/bootprep) and the companion projects above.
