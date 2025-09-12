# dualimagestxt2receipt
the unique receipt maker


# i2r Receipt Gallery - Dual Image Support

## Project Overview

i2r Receipt Gallery is a powerful web-based tool for generating professional receipt-style outputs with dual image support. This application allows users to upload two images, customize processing parameters, add text content, and generate printable receipts. The generated receipts are saved in a gallery for easy management and export.



## Key Features

### Dual Image Processing
- Upload and process two independent images
- Per-image parameter controls:
  - Dither matrix size (2×2 to 16×16)
  - Brightness and contrast adjustment
  - Color inversion toggle
  - Dithering enable/disable

### Flexible Layout Options
- Image 1 → Text → Image 2
- Image 1 → Image 2 → Text

### Text Customization
- Multi-line text input with separator support (`---` for dashed lines, `===` for solid lines)
- Font selection (including Chinese fonts)
- Text alignment (left, center, right)
- Font size and line height adjustment
- Perforation line option
- White-space preservation toggle

### Gallery Management
- Automatic saving of generated receipts
- Pagination system (10 receipts per page)
- Individual receipt download
- Bulk download all receipts
- Receipt deletion (single or entire gallery)

### Real-time Preview
- Instant visual feedback as parameters change
- Accurate representation of final output

## Usage Guide

### Basic Workflow
1. **Upload images** using drag-and-drop or file selection
2. **Adjust parameters** for each image independently
3. **Enter text content** in the text area
4. **Select layout** (Image1-Text-Image2 or Image1-Image2-Text)
5. **Generate receipt** with the Generate button
6. **Manage outputs** in the gallery panel

### Keyboard Shortcuts
- `Ctrl + Enter`: Generate receipt
- `Ctrl + R`: Reset all settings
- `Alt + ←`: Previous gallery page
- `Alt + →`: Next gallery page

### Image Processing Tips
- Use 4×4 dither matrix for balanced detail
- Adjust brightness/contrast to optimize for thermal printers
- Enable color inversion for dark-background images
- Toggle dithering for different artistic effects

## Technical Implementation

### Core Technologies
- **HTML5/CSS3**: Responsive layout with CSS Grid and Flexbox
- **JavaScript (ES6)**: Object-oriented implementation
- **html2canvas**: Client-side rendering library

### Architecture
- **DualImageReceiptGenerator Class**: Central controller
- **Modular Components**:
  - Image processing pipeline
  - Preview rendering system
  - Gallery management
  - UI event handlers

### Image Processing
- Ordered dithering algorithm
- Matrix-based thresholding (2×2 to 16×16)
- Grayscale conversion with luminance preservation
- Brightness/contrast adjustments
- Real-time canvas manipulation

## Setup Instructions

1. Save the provided HTML code as `index.html`
2. Open the file in any modern web browser (Chrome, Firefox, Edge)
3. No additional installation required

> **Note**: Internet connection is required to load the html2canvas library from CDN

## Browser Compatibility
- Google Chrome (latest)
- Mozilla Firefox (latest)
- Microsoft Edge (latest)
- Safari (latest)

## License
 MIT License.

---

**Tip**: For optimal printing results, use thermal paper settings in your printer configuration and ensure bleed settings are properly adjusted.
