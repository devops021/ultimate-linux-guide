# Understanding the Folder Structure

### Explanation of System Directories

### **Symbolic Links (Less Significant)**
| Directory | Description |
|-----------|-------------|
| `/sbin -> /usr/sbin` | System binaries for administrative commands (linked to `/usr/sbin`). |
| `/bin -> /usr/bin` | Essential user binaries (linked to `/usr/bin`). |
| `/lib -> /usr/lib` | Shared libraries and kernel modules (linked to `/usr/lib`). |

### **Important System Directories**
| Directory | Description |
|-----------|-------------|
| `/boot` | Stores files needed for booting the system (not relevant in containers). |
| `/usr` | Contains most user-installed applications and libraries. |
| `/var` | Stores logs, caches, and temporary files that change frequently. |
| `/etc` | Stores system configuration files. |

### **User & Application-Specific Directories**
| Directory | Description |
|-----------|-------------|
| `/home` | Default location for user home directories. |
| `/opt` | Used for installing optional third-party software. |
| `/srv` | Holds data for services like web servers (rarely used in containers). |
| `/root` | Home directory for the root user. |

### **Temporary & Volatile Directories**
| Directory | Description |
|-----------|-------------|
| `/tmp` | Temporary files (cleared on reboot). |
| `/run` | Holds runtime data for processes. |
| `/proc` | Virtual filesystem for process and system information. |
| `/sys` | Virtual filesystem for hardware and kernel information. |
| `/dev` | Contains device files (e.g., `/dev/null`, `/dev/sda`). |

### **Mount Points**
| Directory | Description |
|-----------|-------------|
| `/mnt` | Temporary mount point for external filesystems. |
| `/media` | Mount point for removable media (USB, CDs). |
| `/data` | Likely your **mounted volume** from Windows (`C:/ubuntu-data`). |

### How ls is reconised as command
<div>when it type ls that command will be searched in one on directory configured in PATH </div>
<div>echo $PATH </div>
<div>/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin </div>

### Short descriptions of typical /usr subdirectories on Linux/Unix:

Folder	Role
/usr/bin	Normal user programs and scripts (third‑party and distro packages); should be on every user’s PATH.
/usr/games	Game binaries and related program files (historical convention; not always present).
/usr/include	Header files for C/C++ development (*.h), used when compiling against system libraries.
/usr/lib	Shared libraries, language runtimes, and other architecture‑dependent support files for programs in /usr.
/usr/libexec	Helpers not meant to be run directly by users—only invoked by other programs (daemons, GUI apps, etc.).
/usr/local	Locally installed software (often from source or manual installs); mirrors the layout (bin, lib, …) and overrides nothing in /usr unless you put it earlier on PATH.
/usr/sbin	Programs mainly for system administration (not usually on a normal user’s default PATH).
/usr/share	Architecture‑independent data: docs, man pages, icons, themes, locale files, default configs—no native code here.
/usr/src	Source code the distro keeps handy (e.g. kernel headers or source trees); often empty or minimal on minimal installs.
