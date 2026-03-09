# Back2Phase2

B2P2: Back2Phase2 Launcher
B2P2 is a specialized version-management utility for Project: Playtime, developed entirely in Python. It allows users to download, manage, and switch between Phase 2 (Incineration) and Phase 3 (Destroy-a-Toy) using high-speed direct downloads.

Key Features
Python-Powered Logic: Built with Python for efficient file handling and system-level automation.

Direct Install: Downloads the Phase 2 archive directly to your system, bypassing complex setup processes.

Visual Progress Bar: Real-time tracking of download progress and completion percentages within the terminal.

Zero-Latency Switching: Uses folder-renaming logic to swap game versions in under a second.

Smart State Detection: Automatically identifies the active version via is_phase2.txt or is_phase3.txt markers.

Automated Backups: Safely renames your existing game folder before applying the swap to prevent data loss.

Requirements
Windows 10 or 11.

Administrator Privileges: Required for modifying the Program Files (x86) directory and hooking keyboard inputs.

Stable Internet Connection: Required for the initial download of Phase 2 assets.

Project: Playtime (Steam): The game must already be installed in your Steam library.

Installation
For Users (EXE)
Download B2P2.exe from the official source.

Place the EXE in its own folder (e.g., C:\B2P2).

Right-click and select Run as Administrator.

Select "Install Phase 2 Files" to begin the download.

For Developers (Python Source)
To run the script from source, ensure you have Python 3.x installed and the following libraries:

Bash
pip install requests keyboard colorama
Run the script:

Bash
python main.py
Instructions
Navigation: Use the UP and DOWN arrows to move the highlight.

Selection: Press ENTER to confirm.

The Swap Process:

Switch to Phase 2: Renames "Poppy Playtime - Multiplayer" to "..._Phase 3" and activates your downloaded Phase 2 folder.

Switch to Phase 3: Reverts the folders back to the standard Steam version.

Auto-Launch: Once the swap is complete, B2P2 will automatically trigger Steam to launch the game.

Troubleshooting
Permission Denied: You must run the program as Administrator. Windows protects the Steam folder from unauthorized changes.

Download Stuck: Ensure you have enough disk space (at least 15GB free for the compressed archive and the extracted folder).

Game Won't Start: If Steam reports missing files, use B2P2 to switch back to Phase 3 and "Verify Integrity of Game Files" within Steam, then attempt the swap again.

Credits
Lead Developer: NotCotik

Language: Python 3.x

Interface: B2P2 Stylized CLI
