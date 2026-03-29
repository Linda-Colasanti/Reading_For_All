# Reading For All™ — Lesson System Guide

This repository contains the automated "Smart Swap" lesson engine. Each lesson is powered by a single Master Template (`lesson-paid.html`) and controlled by individual JSON data files.

## **The Master Template**
* **lesson-paid.html**: NEVER edit this file. It contains the logic that swaps out the letters, titles, videos, and PDFs based on the URL.

## **Your Folder Structure**
To keep URLs clean (e.g., `.../lessons/1-2-short-i`), every lesson has its own folder inside the `lessons/` directory.

- **lessons/**
  - **1-1-short-a/**
    - `index.html` (The Redirect)
    - `1-1-short-a.json` (The Data)
  - **1-2-short-i/**
    - `index.html`
    - `1-2-short-i.json`

---

## **SOP: How to Publish a New Lesson (e.g., Short O)**

### **Step 1: Assets (Cloudflare)**
Upload your 4 PDFs to the `/rf4i/` folder in Cloudflare. 
**Naming Convention:** `ShortO-WordList.pdf`, `ShortO-CVCSentences.pdf`, `ShortO-ParentGuide.pdf`, `ShortO-MadLib.pdf`.

### **Step 2: Create the Folder (GitHub)**
Inside the `lessons/` directory, create a new folder: `1-3-short-o`.

### **Step 3: Add the Redirect (GitHub)**
Inside that new folder, create a file named `index.html` and paste this code:
`<script>window.location.replace('/lesson-paid.html?lesson=1-3-short-o');</script>`

### **Step 4: Add the Data (GitHub)**
Inside that same folder, create `1-3-short-o.json`. Copy the code from a previous lesson and update the following:
* `"title"`: "Short O"
* `"heroDisplay"`: "O"
* `"youtube"`: (New YouTube Embed Link)
* `"pdfs"`: (Update the 4 PDF URLs to match Step 1)

* ## Brand Colors (for reference)

- Navy: `#0d1b3e`
- Gold: `#f5c842`
- Rainbow: Red → Orange → Yellow → Green → Blue → Indigo → Violet

---

*Reading For All™ · LindaColasanti.com*
