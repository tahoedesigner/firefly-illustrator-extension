# Illustrator Firefly Extension


## Architecture
```
illustrator-firefly-extension/
├── server/
│   ├── server.js
│   ├── package.json
│   ├── .env
│   └── .gitignore
└── extension/
    ├── CSXS/
    │   └── manifest.xml
    ├── client/
    │   ├── index.html
    │   └── CSInterface.js (download separately)
    └── host/
        └── index.jsx
```

# Install and start the proxy-server
## Add .env 
```
FIREFLY_ID="Your id here"
FIREFLY_API_KEY="Your key here"
FIREFLY_ORG="Your org here"
```

## Install Server
```
cd server
npm install
```

## Start Server
```
node server.js
```

# Install Extension

## Prerequisites
- Adobe Illustrator CC 2020 or later
- CEP 11 or later

## Mac/Linux

1. Open Terminal
2. Navigate to the extension folder
3. Run the setup script:
   ```bash
   chmod +x setup.sh
   ./setup.sh
   ```

## Windows

1. Right-click `setup.bat`
2. Select "Run as Administrator"

### Manual Installation

Copy the entire illustrator-firefly-extension folder to:

#### Mac: /Library/Application Support/Adobe/CEP/extensions/ 
#### Windows: C:\Program Files\Common Files\Adobe\CEP\extensions\

## Enable CEP Debugging
#### Mac:
```
defaults write com.adobe.CSXS.11 PlayerDebugMode 1
```

#### Windows:

- Run regedit as administrator
- Navigate to: HKEY_CURRENT_USER\Software\Adobe\CSXS.11
- Create DWORD: PlayerDebugMode = 1



