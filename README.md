# 🏗️ Property Work Order Automation Pipeline  
### A Data-Driven Workflow Automation System for Property Inspection Documentation  

**Tech Stack:** Python · Selenium · BeautifulSoup · Google Drive API · OpenCV · Zipfile · Google Colab  

---

## 🔍 Executive Summary
This project automates and standardizes the **data workflow behind property inspection documentation** for **make-ready** and **turn-over** jobs.  
It was designed to replace a fragmented manual process where contractors sent photos and notes inconsistently, and project managers manually created and named folders for every work order.

Using **Python, Selenium, and Google Drive API**, this workflow automation pipeline:
- **Extracts** property work order data from a management portal.  
- **Transforms** it into a standardized bilingual (English/Spanish) folder schema.  
- **Loads** it to a private Google Drive, where contractors securely upload photos and notes from the field.  
- **Synchronizes** the project manager review cycle by generating follow-up folders for approvals and clarifications.

This system eliminated redundant administrative steps, reduced folder preparation time from **30+ minutes to under 1 minute**, and improved overall inspection documentation accuracy and traceability.

---

## 💼 Business Problem
Before automation, inspection data was unstructured and decentralized:
- Contractors sent photos through text or email, often unlabeled or missing context.  
- Project managers recreated folder hierarchies manually for every property.  
- Tracking progress between “submitted” and “approved” inspections was slow and error-prone.

The result was inconsistent record-keeping and delayed project turnover — issues that created compliance risks and communication breakdowns.

---

## 💡 Solution
The **Property Work Order Automation Pipeline** introduced a structured data flow that mirrored an ETL-style process for operational documentation:

1. **Extract** active work orders and property data directly from the web portal.  
2. **Transform** each entry into a bilingual, standardized folder schema for every inspection category (Electrical, Flooring, Safety, etc.).  
3. **Load** the generated folders to a secure Google Drive, creating isolated upload areas for each contractor.  
4. **Enable real-time collaboration** — contractors upload annotated photos onsite, while project managers review, comment, and request clarification.  
5. **Preserve version history** by generating secondary “approved” folders once the review cycle is complete.  

This approach unified the data flow between field and office, improving both transparency and accountability.

---

## 🧰 Tools and Methods

| Stage | Purpose | Tools / Libraries |
|-------|----------|-------------------|
| Data Extraction | Automate web portal navigation | `selenium`, `webdriver-manager` |
| HTML Parsing | Identify elements and pull data | `BeautifulSoup`, `lxml` |
| Data Structuring | Create bilingual folder schemas | `os`, `zipfile`, `re` |
| Secure Loading | Upload to private Google Drive | `Google Colab`, `gdown`, Drive API |
| Data Validation | Visualize and confirm automation | `OpenCV`, `cv2_imshow` |

---

## ⚙️ Key Features
- **Automated Data Workflow:** Converts raw inspection info into standardized directory structures.  
- **Bilingual Output:** English and Spanish folder names and descriptions for diverse field teams.  
- **Private Cloud Integration:** Upload-only Google Drive URLs ensure controlled access.  
- **Review Synchronization:** Automatically creates follow-up folders for approved or revised submissions.  
- **Process Reusability:** Easily adaptable to other documentation or data-capture pipelines.  

---

## 📊 Results & Business Impact

| Metric | Before | After Automation |
|--------|---------|------------------|
| Folder creation time | 30–45 minutes | < 1 minute |
| Data structure consistency | Low | 100% standardized |
| Photo submission completeness | ~65% | >95% |
| Manager–contractor communication lag | 1–2 days | < 2 hours |

**Impact:**  
Created a traceable, standardized data workflow between contractors and project managers — improving compliance, efficiency, and documentation quality across multiple regions.

---

## 🧠 Skills Demonstrated
- **Python Workflow Automation**  
- **Data Extraction & Transformation**  
- **Structured Data Management (File-Based ETL)**  
- **API Integration & Secure Cloud Collaboration**  
- **Process Design & Version Control**  
- **Cross-Language Data Documentation (EN/ES)**  

---

## 🧾 Example Output (Test Data)

> 🔗 **Sample Folder (View Only):** [View Demo Folder on Google Drive](https://drive.google.com/drive/folders/1017bUw95w6XLiByYmvn6piw3h9-4xoIE?usp=sharing)

This example folder was generated using sanitized test data to demonstrate how the automation organizes property inspection documentation.  
It includes:
- Bilingual (English/Spanish) folder names  
- Scopewalk categories with description text files  
- Standardized naming conventions for traceability  

All project data has been fully anonymized for privacy.

---

## 🧭 Next Steps
- Implement **Drive API v3 automation** for direct uploads and permission control.  
- Build a **Power BI dashboard** to visualize inspection metrics and approval timelines.  
- Add **email notification triggers** for project manager review events.  

---

## ⚖️ Ethical and Privacy Notes
This project was originally developed as an **internal workflow automation** for property inspection management.  
All examples and data are **mocked and non-identifiable**.  
The original system (Pathlight / Scopesey) later merged under **Tricon Residential**.  
This repository exists solely for **educational and portfolio demonstration** purposes.

---

👤 Created by Anthony Edeza  
📧 [anthonyedeza.data@gmail.com]

---

### 💬 Recruiter Note
If you’re evaluating this portfolio:
- This project demonstrates **data workflow automation** that bridges operations and analytics.  
- It highlights strong skills in **Python scripting, structured data design, and automation logic**.  
- It reflects **business-aware problem solving**, showing how data structure and automation directly improve operations.

---

### 🏁 Summary
> This project connects **data automation** with **real-world operational workflows**, transforming unstructured inspection data into standardized, shareable, and reviewable formats.  
> It demonstrates the foundation of a scalable data pipeline — built to solve human workflow problems through clean, automated design.
