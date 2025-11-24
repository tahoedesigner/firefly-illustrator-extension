# Illustrator Firefly Extension


## Architecture
```
illustrator-firefly-extension/
├── proxy-server/
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

## Install
```
npm install
```

## Start
```
npm start
```
## Env Example 
```
FIREFLY_ID="Your id here"
FIREFLY_API_KEY="Your key here"
FIREFLY_ORG="Your org here"
```

