# Al Madhi Carpentry — ERP

A single-file, offline-first Progressive Web App running the full purchase and sales operations of a wooden pallet manufacturing and trading business in Sharjah, UAE.

## Overview

Al Madhi ERP handles both sides of the business in one codebase, switching between a Purchase mode (navy/gold theme) and a Sales mode (teal/aqua theme) via a single toggle — same UI and logic, different data pointer and theme. It's built specifically for wood/pallet trading, not adapted from generic accounting software: KG/bag-based weight pricing, auto-filled last prices by supplier, a shared cheque register across both modules, bilingual (English/Urdu) documents, and FIFO-based receivables aging.

## Features

- Dashboard with unified Purchase + Sales overview
- Invoice creation and full invoice/record history
- Payments with invoice-wise allocation
- Customer/supplier statements and search
- Shared cheque register (pending/cleared tracking)
- Expenses module with salary tracking
- Delivery notes and quotations
- Global search, PIN + biometric app lock
- Party and user management
- Export/backup (Excel via SheetJS) and bilingual invoice/document printing

## Tech Stack

- **Core:** Pure HTML5, CSS3, vanilla JavaScript — no framework, no build step (~17,000 lines, single file)
- **Backend:** Firebase Realtime Database (cloud-first, ES module SDK)
- **Export:** jsPDF, jsPDF-AutoTable, SheetJS (xlsx)
- **Offline:** Local write queue with dual-signal connection detection, replayed on reconnect

## Screenshots

*Coming soon.*

## Documentation

Full technical and feature documentation (dual-mode architecture, Firebase sync, every module, form validation, keyboard shortcuts, known bug fixes): [`docs/DOCUMENTATION.md`](docs/DOCUMENTATION.md)
