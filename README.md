
# Wotsin — Android Food Barcode Scanner

**A native Android application combining barcode scanning, OCR and an offline food product database.**

Wotsin helps users identify ingredients and food additives of interest in packaged food products. Users can configure which substances they want to be alerted about.

The application is independently developed and published on Google Play.

**[Google Play](https://play.google.com/store/apps/details?id=com.stacktracesoftware.wotsin)** | **[Technical Case Study](https://stacktracesoftware.com/portfolio/wotsin.html)**

## Overview

Wotsin supports two complementary methods of examining packaged food:

1. **Barcode scanning** — looks up product information in a locally stored database.
2. **Optical Character Recognition (OCR)** — reads ingredient information directly from product packaging.

Users can select which ingredients and additives are relevant to them, reducing unnecessary alerts.

The application is designed to operate without requiring an internet connection for its core scanning and database functions.

## Technologies

| Component | Technology |
|-----------|------------|
| Application | Native Android |
| Language | Kotlin |
| Product database | SQLite |
| Image processing | OpenCV |
| Text recognition | OCR |
| Barcode scanning | Android barcode scanning integration |
| Data preparation | Java, Python, MongoDB |

## Technical Highlights

### 1. Offline Product Database

The application's local SQLite database contains approximately 500,000 product records.

The database was produced from a substantially larger source dataset using a processing pipeline involving MongoDB, Java and SQLite.

The resulting database is approximately 350 MB, with indexes and a reduced dataset designed for mobile use.

### 2. Barcode and OCR Integration

Barcode scanning provides rapid access to product information when a product is present in the database.

OCR provides an alternative method for examining ingredient information directly from packaging.

This combination improves coverage when barcode lookup alone is insufficient.

### 3. OCR Image Preprocessing

A significant development challenge involved improving the quality of images submitted for text recognition.

Image preprocessing using OpenCV helped improve OCR performance when working with real-world product packaging.

The OCR capture interface is optimised to reduce camera shake and greatly improve the accuracy of the scanned text.

### 4. Configurable Alerts

Wotsin maintains a configurable list of substances that users may wish to investigate.

Users can enable or disable individual alerts, view explanatory information and access further research through their preferred browser or search engine.

### 5. Offline Operation

The local database and on-device processing approach allow core functionality to remain available without a network connection.

## Additional Features

- Product search and scanning history
- Light and dark themes
- Context-sensitive help
- Configurable ingredient and additive alerts
- Offline product lookup

## Engineering Responsibilities

This project involved the complete application development lifecycle, including:

- Requirements and feature design
- Android application development
- Database preparation and optimisation
- Barcode and OCR integration
- Image processing and usability improvements
- Testing and debugging
- Google Play publication and maintenance

## Availability

Wotsin is available on Google Play.

**[View Wotsin on Google Play](https://play.google.com/store/apps/details?id=com.stacktracesoftware.wotsin)**

For screenshots, additional technical background and project details, see the **[Wotsin case study](https://stacktracesoftware.com/portfolio/wotsin.html)**.

## Source Code

This repository is a technical showcase.

The commercial application's source code, product database and associated proprietary assets are not included.

## Contact

**Stack Trace Software**

Website: https://stacktracesoftware.com/

Email: hello@stacktracesoftware.com
