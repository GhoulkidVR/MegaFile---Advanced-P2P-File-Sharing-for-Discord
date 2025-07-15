# MegaFile - Advanced P2P File Sharing for Discord

[![License](https://img.shields.io/badge/License-GPL--3.0--or--later-blue.svg)](LICENSE)
[![Vencord](https://img.shields.io/badge/Vencord-Plugin-5865F2.svg)](https://github.com/Vendicated/Vencord)

MegaFile is an advanced distributed file sharing system for Discord that enables seamless transfer of files up to 100GB+ through a peer-to-peer network. This Vencord plugin bypasses Discord's file size limitations while maintaining security, reliability, and performance.

## Key Features

- **Distributed P2P Architecture**: Leverages the collective resources of all users for file hosting
- **Massive File Support**: Transfer files up to 100GB+ with no central server limitations
- **Military-Grade Security**: End-to-end encryption and cryptographic integrity verification
- **Intelligent Chunking**: Configurable chunk size (default 50MB) with automatic reassembly
- **Network Redundancy**: Multiple copies of each chunk ensure file availability
- **Real-Time Monitoring**: View network statistics and hosting status
- **Seamless Integration**: Native Discord UI integration with minimal footprint

## Installation

### Prerequisites
- [Vencord](https://github.com/Vendicated/Vencord) developer build installed
- Node.js and pnpm installed on your system

### Installation Methods

#### Method 1: Git Clone (Recommended)
```bash
# Navigate to your Vencord userplugins directory
cd /path/to/vencord/src/userplugins

# Clone the repository
git clone https://github.com/[your-username]/MegaFile.git

# Build the plugin
pnpm build
```

#### Method 2: Manual Installation
1. Download the latest release from the [Releases page](https://github.com/[your-username]/MegaFile/releases)
2. Extract the ZIP file into your `vencord/src/userplugins` directory
3. Run `pnpm build` in your Vencord directory

## Usage

Once installed and built:
1. Open Discord with Vencord
2. Access the plugin settings via Vencord's settings panel to configure:
   - Storage allocation
   - Network preferences
   - Security options
3. Upload files through:
   - The new "Upload MegaFile" context menu option
   - Drag-and-drop file sharing
   - The `/megaupload` command

## Technical Details

### Network Architecture
MegaFile utilizes a hybrid P2P architecture combining:
- Distributed Hash Table (DHT) for peer discovery
- WebRTC for direct peer connections
- Relay servers for NAT traversal
- Cryptographic chunk verification

### Security Model
- AES-256 encryption for all file chunks
- SHA-256 integrity verification
- Zero-knowledge architecture (no central server sees your files)
- Configurable redundancy levels

## Troubleshooting

If you encounter any issues:
1. Verify you're using the latest Vencord developer build
2. Check your firewall allows P2P connections (UDP ports 50000-60000 recommended)
3. Ensure sufficient disk space is allocated in settings
4. For additional help, open an Issue or contact [your support channel]

## Contributing

We welcome contributions! Please:
1. Fork the repository
2. Create a feature branch
3. Submit a Pull Request

See our [Contribution Guidelines](CONTRIBUTING.md) for details.

## License

This project is licensed under the GPL-3.0-or-later License - see the [LICENSE](LICENSE) file for details.

---

## README.md Notes

1. **Name**: "MegaFile" conveys the large file capability while being professional
2. **Badges**: Added license and Vencord compatibility badges
3. **Structure**: Organized with clear sections and subsections
4. **Technical Depth**: Added architecture and security details for advanced users
5. **Visual Hierarchy**: Used proper Markdown formatting for readability
6. **Call to Action**: Clear installation and contribution instructions
