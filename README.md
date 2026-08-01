<img src="./screenshots/logo.png" width="300">

# Forma GNU/Linux
### By soup1023

Forma GNU/Linux is a Debian-based Linux distribution built around the concept of **"structural beauty."**
Rather than simply being easy to use, Forma is designed to give users as much freedom as possible to **manage and customize** their own systems while keeping those tasks as simple as possible.

---

# 🎯 Features

### 📦 Keep What You Need, Leave What You Don't
Debian includes a large number of kernel modules (drivers) to support a wide variety of hardware.
Forma GNU/Linux plans to provide a mechanism that allows unused drivers to be archived into `tar.xz` files, helping reduce disk usage while allowing them to be restored at any time when needed.
You may wonder why Forma does not simply compress every kernel module into `*.ko.xz` from the beginning. While compressed modules save storage space, they also require CPU time for decompression during loading. On lower-performance hardware, this can increase boot time.
Forma aims to strike a balance between storage efficiency and performance, leaving the final choice to the user.

---

### 🌐 Designed with Offline Use in Mind
Forma GNU/Linux is designed to perform basic installation and everyday use without requiring an Internet connection.
Also, thanks to the developer's questionable sense of humor, Tetris is somehow included.

---

### 💾 Custom Installer

Forma GNU/Linux includes its own TUI (Text User Interface) installer called **Forma Installer**.
While it is not as feature-rich as modern GUI installers, it is designed to provide a straightforward installation experience using only the keyboard. Disk selection, user configuration, and other common installation tasks are presented in a simple and understandable way.
Forma Installer is currently written in **Python**. Although languages such as C or Go may offer better runtime performance, Python was chosen to prioritize development speed, maintainability, and ease of adding new features.

---

### 🧰 Custom Management Commands
Forma GNU/Linux provides a dedicated command called **`forma`** for system management.
The goal of the `forma` command is to provide a unified interface for managing drivers, packages, kernel modules, system settings, and other Forma-specific features.
A TUI-based management tool called **`forma-tui`** is also planned. It is intended to provide an intuitive keyboard-driven interface, making system management accessible to both beginners and experienced users.

---

### 💿 Multiple Editions
Forma GNU/Linux offers several editions for different use cases.

| Edition | Description |
| :--- | :--- |
| **Standard Edition** | The recommended edition for most desktop and laptop users. It provides a balanced selection of drivers while keeping the system lightweight. |
| **Desktop Edition** | Includes a graphical desktop environment for everyday use. Currently under development. |
| **Full Edition** | Includes a broader collection of drivers and additional components for maximum hardware compatibility, including servers and specialized systems. |
| **Minimal Edition** | A lightweight edition containing only the essentials. Designed for users who prefer building their own environment from the ground up. |
| **Garbage Edition** | A joke edition created purely because the developer thought it would be funny. Not recommended if you're looking for a practical system. |

### ✅ System Requirements

The system requirements for Forma GNU/Linux differ depending on whether the system boots in **BIOS** or **UEFI** mode.

### BIOS

| Edition              | Minimum CPU | Recommended CPU | Minimum RAM | Recommended RAM | Minimum Storage | Recommended Storage |
| -------------------- | ----------- | --------------- | ----------- | --------------- | --------------- | ------------------- |
| **Standard Edition** | 1 Core      | 2 Cores+        | 70 MB+      | 128 MB+         | 1 GB+           | 5 GB+               |
| **Desktop Edition**  | 2 Cores+    | 4 Cores+        | 512 MB+     | 1 GB+           | 10 GB+          | 20 GB+              |
| **Full Edition**     | 1 Core      | 2 Cores+        | 128 MB+     | 256 MB+         | 1 GB+           | 5 GB+               |
| **Minimal Edition**  | 1 Core      | 2 Cores+        | 70 MB+      | 128 MB+         | 1 GB+           | 5 GB+               |
| **Garbage Edition**  | 1 Core+     | 1 Core+         | 10 MB+      | 10 MB+          | 1 GB+           | 5 GB+               |

### UEFI

| Edition              | Minimum CPU | Recommended CPU | Minimum RAM | Recommended RAM | Minimum Storage | Recommended Storage |
| -------------------- | ----------- | --------------- | ----------- | --------------- | --------------- | ------------------- |
| **Standard Edition** | 1 Core      | 2 Cores+        | 256 MB+     | 512 MB+         | 1 GB+           | 5 GB+               |
| **Desktop Edition**  | 2 Cores+    | 4 Cores+        | 512 MB+     | 1 GB+           | 10 GB+          | 20 GB+              |
| **Full Edition**     | 1 Core      | 2 Cores+        | 256 MB+     | 512 MB+         | 1 GB+           | 5 GB+               |
| **Minimal Edition**  | 2 Cores     | 2 Cores+        | 256 MB+     | 512 MB+         | 1 GB+           | 5 GB+               |
| **Garbage Edition**  | N/A         | N/A             | N/A         | N/A             | N/A             | N/A                 |

> [!NOTE]
> The reason why the current UEFI build requires more memory than the BIOS build is still unknown and under investigation.
>
> In practice, this limitation is unlikely to affect most users, as systems running UEFI typically have significantly more than 256 MB of RAM available.

---

# 🚧 Features in Development
The following components are currently under development:

- `forma` command
- `forma-tui`
- Package management utilities
- Hardware management tools

---

# 🎯 Project Goals
Forma GNU/Linux is **not** intended to be an all-in-one Linux distribution.
Instead, its goal is to let users choose what they need, leave out what they don't, and gain at least a basic understanding of how Linux works while building an environment that suits their own needs.
Whether you are a beginner or an advanced user, Forma aims to provide a Linux distribution that can grow alongside your knowledge and be customized freely for your own workflow.

---

# 🛠️ Build
Please refer to the `docs/` directory for build instructions.
