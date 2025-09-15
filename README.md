# ACV to FFMPEG Converter

A web-based tool to convert Adobe Photoshop .acv (curve) files to FFMPEG filter parameters. Works entirely in the browser - no server or installation required!

## 🎯 Features

- 📊 Decode Photoshop .acv curve files
- 🎬 Generate FFMPEG `curves` filter parameters
- 📈 Visual curve preview with canvas rendering
- 🖱️ Drag & drop file support
- 📋 One-click copy commands
- 🔍 Debug mode for file analysis
- 💻 Works offline - no server needed
- 📱 Mobile responsive design

## 🚀 Quick Start

### Use Online
Visit: https://trebla.github.io/acv-to-ffmpeg-converter/

### Use Locally
1. Download `index.html`
2. Open in any modern web browser
3. Load your .acv file

## 📖 How to Use

1. **Load an ACV file** - Click or drag & drop a .acv file from Photoshop
2. **View the results** - The tool will display:
   - FFMPEG filter parameters
   - Ready-to-use FFMPEG commands
   - Visual curve representation
   - Detailed curve point data
3. **Copy the command** - Click the copy button to use in your terminal

## 💡 Example Output
```bash
ffmpeg -i input.mp4 -vf "curves=master='0/0 0.25/0.3 0.5/0.5 0.75/0.7 1/1'" output.mp4
```

# Example ACV Files

This folder contains sample Adobe Curve (.acv) files for testing the converter.

## 🎨 Example Results

Color correction underwater webcam


<div align="center">
  <table>
    <tr>
      <td align="center"><b>Before</b></td>
      <td align="center"><b>After</b></td>
    </tr>
    <tr>
      <td><img src="examples/before.jpg" width="400" alt="Before"></td>
      <td><img src="examples/after.jpg" width="400" alt="After"></td>
    </tr>
  </table>
</div>


## How to Create Your Own ACV Files

1. Open any image in Photoshop
2. Go to Image → Adjustments → Curves (Ctrl/Cmd + M)
3. Adjust the curves to your liking
4. Click the menu icon (≡) in the Curves panel
5. Select "Save Curves Preset..."
6. Save as .acv file


## 🛠️ Technical Details

* Pure HTML/JavaScript/CSS - no dependencies
* Supports Photoshop ACV format versions 1 and 4
* Handles multiple curve channels (Master, R, G, B, Alpha)
* Binary file parsing in browser using DataView API

## 📄 License
MIT License - feel free to use in your projects!

## 🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first.

## 🙏 Acknowledgments
Built to bridge the gap between Photoshop color grading and FFMPEG video processing.

Build with Claude.ai
