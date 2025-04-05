# SneakPeek

An experimental web tracking project that explores advanced fingerprinting and identification techniques.

## Features

- Creates persistent identifiers using advanced browser fingerprinting.
- Demonstrates how data can survive typical privacy protection methods.
- Works across normal browsing modes and survives cache/cookie clearing (not incognito).
- Emulates realistic web environments with multiple servers.

## How it Works

The system uses a set of coordinated components to identify users uniquely:

1. **Fingerprint Collection**: Gathers unique characteristics of the browser and system.
2. **Identifier Generation**: Produces a consistent UID based on the fingerprint.
3. **Data Persistence**: Writes the UID to multiple browser storage locations.
4. **Server Communication**: Web servers receive and store fingerprint data.

## Components

- `main.js`: Core server logic.
- `express-web`: Web interface with tracking scripts.
- `client.js`: JavaScript fingerprint collector injected into the client.
- Multiple webservers mimic domain diversity for realism.

## Requirements

- Node.js (v12+ recommended)
- Modern web browser (for testing)

## Getting Started

```bash
git clone https://github.com/Nagacharan898/SneakPeek.git
cd SneakPeek
npm install
node --experimental-json-modules main.js
