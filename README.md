# SubStudy

Minimalist web tool for processing subtitle files with clean, modern interface.

## Features

- **Subtitle Processing**: Clean and format SRT/TXT subtitle files
- **PDF Export**: Generate multi-column PDFs with customizable settings
- **Text Download**: Export processed content as TXT files
- **Copy to Clipboard**: Quick copy functionality
- **Responsive Design**: Works on desktop and mobile devices

## Setup

1. Clone or download the project
2. Open terminal in project directory
3. Start local server:
   ```bash
   python -m http.server 8000
   ```
4. Open browser and navigate to `http://localhost:8000`

## Usage

1. **Upload File**: Drag and drop or click to upload SRT/TXT files
2. **Review Output**: Processed content appears in the text area
3. **Configure PDF**: Adjust columns, font size, and title in settings
4. **Export**: Use Copy, Download TXT, or Print PDF buttons

## PDF Settings

- **Columns**: 1-4 columns layout
- **Font Size**: 6pt-10pt options
- **Title**: Optional PDF title
- **Timestamps**: Show/hide timestamps in PDF

## Technical Stack

- **Frontend**: Vanilla JavaScript (ES6 modules)
- **Styling**: Pure CSS with Inter font
- **PDF Generation**: jsPDF + html2canvas
- **Icons**: Lucide icons
- **Architecture**: Modular component system

## File Structure

```
src/
├── components/          # UI components
│   ├── App.js           # Main application
│   └── common/          # Shared components
├── services/            # Business logic
│   ├── ConfigManager.js # Settings management
│   ├── PDFExporter.js   # PDF generation
│   └── ToolRegistry.js  # Tool registration
├── tools/               # Feature modules
│   └── SubtitleProcessor.js
├── styles/              # CSS styles
└── utils/               # Utility functions
```

## Browser Support

- Chrome/Edge 88+
- Firefox 85+
- Safari 14+
- Mobile browsers with ES6 module support

## License

MIT License - see package.json for details