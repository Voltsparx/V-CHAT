█▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀█  
█  ██╗   ██╗         ██████╗██╗  ██╗ █████╗ ████████╗  █  
█  ╚██╗ ██╔╝        ██╔════╝██║  ██║██╔══██╗╚══██╔══╝  █  
█   ╚████╔╝ █████╗  ██║     ███████║███████║   ██║     █  
█    ╚██╔╝  ╚════╝  ██║     ██╔══██║██╔══██║   ██║     █  
█     ██║           ╚██████╗██║  ██║██║  ██║   ██║     █  
█     ╚═╝            ╚═════╝╚═╝  ╚═╝╚═╝  ╚═╝   ╚═╝     █  
█▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄█         
║► BY: Voltsparx                         VERSION: 3.2 ◄║  
║► GITHUB: github.com/your-repo                       ◄║  
▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀

V-CHAT TERMINAL CHAT v3.2
=============================

Developed by: Voltsparx
Email: voltsparx@gmail.com

INSTALLATION
------------

Required Packages:
- Python 3.6+
- netifaces (for network detection)
- colorama (for colored terminal output)
- sound playback tools

OS-Specific Installation:

1. Linux (Debian/Ubuntu/Kali):
   sudo apt update
   sudo apt install python3 python3-pip
   pip3 install netifaces colorama
   sudo apt install libasound2-dev  # For sound support

2. macOS:
   # Install Homebrew if you don't have it:
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   brew install python
   pip3 install netifaces colorama
   # Sound support comes pre-installed

3. Windows:
   # Download Python from python.org (3.6+)
   # During installation, check "Add Python to PATH"
   pip install netifaces colorama
   # Sound support comes pre-installed

QUICK START
-----------

1. First-time setup:
   mkdir -p assets/sounds
   # Add your sound files (optional):
   # - assets/sounds/notify.mp3
   # - assets/sounds/mention.wav

2. Start the server:
   python v_chat.py --server --username Admin

3. Connect clients:
   python v_chat.py --host [SERVER_IP] --username Client1

NETWORK TYPES
-------------
When starting the server, choose:
1. Internet - Public IP (requires port forwarding)
2. WiFi - Local wireless network IP
3. Ethernet - Local wired network IP

COMMAND REFERENCE
-----------------

Basic Commands:
/exit-terminal-chat - Disconnect gracefully
/msg [user] [message] - Private message
@username - Mention a user (plays sound)

Notification Control:
/notify-me on every message True - All messages
/notify-me on every message False - Only mentions

TROUBLESHOOTING
---------------

Common Issues:

1. Connection Failed:
   - Verify server is running
   - Check firewall settings
   - Ensure correct IP/port

2. No Sound:
   - Check sound files in assets/sounds/
   - Verify OS sound permissions

3. Network Detection Issues:
   - Ensure netifaces is installed
   - Try manual --host parameter

For Windows Users:
- If pip isn't recognized, use:
  py -m pip install netifaces colorama

For macOS Users:
- If Python isn't found after brew install:
  echo 'export PATH="/usr/local/opt/python/libexec/bin:$PATH"' >> ~/.zshrc
  source ~/.zshrc

SUPPORT
-------
Report issues to: voltsparx@gmail.com
