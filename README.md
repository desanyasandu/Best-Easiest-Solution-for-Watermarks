# 🧹 Gamma Watermark Remover

A fully client-side web application that removes **"Made with Gamma"** watermarks from PPTX and PDF files — instantly, privately, and without any server uploads.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Client-Side](https://img.shields.io/badge/processing-100%25%20client--side-green)
![PPTX](https://img.shields.io/badge/format-PPTX-orange)
![PDF](https://img.shields.io/badge/format-PDF-red)

---

## 🌐 Live Demo

Simply open the `index.html` file in any modern browser — no installation or server required.

---

## ✨ Key Features

| Feature | Description |
|---|---|
| 🔒 **100% Client-Side** | No files are uploaded to any server. All processing happens locally in your browser. |
| 📊 **PPTX Support** | Full watermark removal from PowerPoint presentations |
| 📄 **PDF Support** | Annotation, text, and metadata cleanup for PDF files |
| 🖱️ **Drag & Drop** | Intuitive file upload with visual feedback |
| 📋 **Detailed Activity Log** | See exactly what was changed in your file |
| ⚙️ **Configurable Options** | Toggle individual removal steps on/off |
| 📱 **Responsive Design** | Works seamlessly on desktop and mobile devices |

---

## 🔧 How It Works

### 📊 PPTX Processing (5-Step Pipeline)

PPTX files are ZIP archives containing XML files. The app uses **JSZip** to unpack, modify, and repack them.
