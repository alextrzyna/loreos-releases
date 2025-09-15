# LoreOS Releases

Welcome to the official release repository for **LoreOS**, an AI-powered island survival RPG game built with Godot 4.4.1.

## 📥 Latest Release

The latest stable release can always be found in the [releases/latest](releases/latest) directory.

## 🎮 Available Platforms

LoreOS is available for the following platforms:

- **Linux** (x86_64)
- **Windows** (x86_64)
- **macOS** (Universal - Intel & Apple Silicon)
- **Web** (HTML5)

## 📦 Download Instructions

### Quick Download Links

Navigate to the [releases](releases/) directory and choose your version, or use the latest version:

- 🐧 **Linux**: `LoreOS-linux.tar.gz`
- 🪟 **Windows**: `LoreOS-windows.zip`
- 🍎 **macOS**: `LoreOS-macos.dmg`
- 🌐 **Web**: `LoreOS-web.zip`

## 🚀 Installation Instructions

### Linux

1. Download `LoreOS-linux.tar.gz` from the releases directory
2. Extract the archive:
   ```bash
   tar -xzvf LoreOS-linux.tar.gz
   ```
3. Make the binary executable:
   ```bash
   chmod +x LoreOS.x86_64
   ```
4. Run the game:
   ```bash
   ./LoreOS.x86_64
   ```

### Windows

1. Download `LoreOS-windows.zip` from the releases directory
2. Right-click the ZIP file and select "Extract All..."
3. Navigate to the extracted folder
4. Double-click `LoreOS.exe` to run the game

**Note**: Windows may show a security warning. Click "More info" and then "Run anyway" to proceed.

### macOS

1. Download `LoreOS-macos.dmg` from the releases directory
2. Double-click the DMG file to mount it
3. Drag the LoreOS app to your Applications folder
4. Double-click LoreOS to run the game

**✅ Signed and Notarized**: Starting with v0.3.4-alpha, the macOS app is properly signed with an Apple Developer ID and notarized by Apple. You should not see any security warnings when opening the app.

**Note for Apple Silicon Macs**: The app is a Universal build and will run natively on both Intel and Apple Silicon Macs.

### Web Version

1. Download `LoreOS-web.zip` from the releases directory
2. Extract the ZIP file
3. Host the files on a web server (local or remote)

   **For local testing:**
   ```bash
   # Using Python 3
   cd extracted-folder
   python3 -m http.server 8000
   ```
   Then open `http://localhost:8000` in your browser

4. For production deployment, upload the files to your web server and ensure proper MIME types are configured for `.wasm` and `.pck` files

**Browser Requirements:**
- Chrome 91+, Firefox 89+, Safari 15+, or Edge 91+
- WebGL 2.0 support required
- SharedArrayBuffer support recommended for better performance

## 🔧 Troubleshooting

### Common Issues

#### macOS: "Cannot be opened because it is from an unidentified developer"
- This should not occur with v0.3.4-alpha and later (app is signed and notarized)
- For older versions, you may need to right-click the app and select "Open"
- Or go to System Settings → Privacy & Security and click "Open Anyway"

#### Linux: "Permission denied" when running
- Ensure you've made the file executable with `chmod +x`
- Check that you're in the correct directory

#### Windows: "Windows protected your PC"
- This is Windows Defender SmartScreen
- Click "More info" then "Run anyway"
- Or add an exception in Windows Defender

#### Web: Black screen or loading issues
- Ensure your browser supports WebGL 2.0
- Try clearing your browser cache
- Check browser console for error messages
- Some browsers require HTTPS for certain features

## 🎮 Game Controls

### Camera Controls
- **WASD/Arrow Keys**: Move camera
- **Mouse Wheel**: Zoom in/out
- **Right Click + Drag**: Rotate camera view
- **Space**: Reset camera to default position

### Debug Controls
- **Ctrl+Shift+L**: Toggle LLM integration on/off
- **F3**: Toggle debug UI visibility

## 📊 System Requirements

### Minimum Requirements
- **OS**: Windows 10, macOS 10.12, Ubuntu 20.04, or newer
- **Processor**: Dual-core 2.4 GHz
- **Memory**: 4 GB RAM
- **Graphics**: OpenGL 3.3 / OpenGL ES 3.0 compatible
- **Storage**: 500 MB available space

### Recommended Requirements
- **OS**: Latest version of Windows, macOS, or Linux
- **Processor**: Quad-core 3.0 GHz
- **Memory**: 8 GB RAM
- **Graphics**: Dedicated GPU with 2GB VRAM
- **Storage**: 1 GB available space

## 📝 Version History

Check the [releases](releases/) directory for version-specific folders. Each version includes:
- Platform-specific builds
- `version.json` with build metadata
- SHA256 checksums for verification

## 🔐 Verifying Downloads

Each release includes SHA256 checksums. To verify your download:

```bash
# Linux/macOS
sha256sum -c SHA256SUMS.txt

# Windows (PowerShell)
Get-FileHash LoreOS-windows.zip -Algorithm SHA256
```

## 🐛 Bug Reports & Feedback

Found a bug or have feedback? Please report issues at:
https://github.com/alextrzyna/aisland/issues

## 📜 License

LoreOS is distributed under the MIT License. See the main repository for details.

## 🤝 Contributing

Interested in contributing? Check out the main development repository:
https://github.com/alextrzyna/aisland

---

**Note**: This repository contains only release builds. For source code and development, please visit the main repository.
