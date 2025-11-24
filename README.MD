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
# Step 1: Add .env here > ./server/.env
FIREFLY_ID="Your id here"
FIREFLY_API_KEY="Your key here"
FIREFLY_ORG="Your org here"
```

## Install Server
```
# Step 2
cd server
npm install
```

## Start Server
```
# Step 3
node server.js
```

# Install Extension
Copy the entire illustrator-firefly-extension folder to:
Mac: /Library/Application Support/Adobe/CEP/extensions/
Windows: C:\Program Files\Common Files\Adobe\CEP\extensions\

## Enable CEP Debugging
Mac:
```
defaults write com.adobe.CSXS.11 PlayerDebugMode 1
```

Windows:

Run regedit as administrator
Navigate to: HKEY_CURRENT_USER\Software\Adobe\CSXS.11
Create DWORD: PlayerDebugMode = 1



