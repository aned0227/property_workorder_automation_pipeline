# 🏗️ Property Work-Order Automation Pipeline

Automates a property-management workflow — from field inspection (“Scopewalk”) folder generation to post-review line-item extraction — using **Python**, **Selenium**, and **BeautifulSoup**.

This project demonstrates how real-world property operations can be streamlined through automation, standardized folder creation, and bilingual documentation generation.

---

## 💡 Why This Was Built

This automation was developed to improve collaboration between **contractors** and **project managers** who often had varying levels of technical experience.

Many field contractors struggled with complex reporting tools and file-sharing platforms, so a practical solution was created:

- Automatically generate standardized inspection folders for each property.
- Upload these folders to a **private Google Drive**, configured so that **only users with the unique URL could access the folder**.
- Contractors could **upload photos and notate them directly within the shared folder**, without needing admin privileges or full-drive access.

Each Google Drive folder link was sent to the assigned contractor and included:
- The **property address**
- The **lockbox code**
- The **property type** (either *Make-Ready* or *Turn-Over*)

This ensured that contractors received **only the information relevant to their assigned job site** while maintaining controlled access and data privacy.

After the **project manager** reviewed the contractor’s submissions:
- A second set of folders was automatically generated for **approved or clarified items**, ensuring a clean separation between:
  1. The **original contractor submissions** (field findings).
  2. The **approved and verified work items** (project-manager confirmations).

This workflow allowed the team to:
- Maintain full transparency and traceability between field and management.
- Ensure that only approved scope items were billed.
- Preserve both the original and approved documentation for quality assurance and accountability.

---

## 🚀 Project Overview

This repository contains a two-stage automation pipeline designed for a legacy property-management system (now deprecated).  
It replicates a common internal process used by property-management teams to organize field inspections and extract approved work-order data for reporting and payment verification.

| Stage | Notebook | Description |
|--------|-----------|-------------|
| **1️⃣ Folder Creation & Setup** | `01_generate_inspection_folders.ipynb` | Automates generation of bilingual inspection folders (“Scopewalks”) for contractors, including subfolder templates for photos, findings, and scope categories. |
| **2️⃣ Review & Extraction** | `02_extract_reviewed_lineitems.ipynb` | Parses and organizes post-review work-order data after project-manager approval, producing clean, structured outputs for downstream reporting. |

---

## 🧠 Key Features

- **Automated Portal Interaction:** Uses Selenium to simulate browser activity, log in, and capture work-order data.  
- **Dynamic Folder Generation:** Creates bilingual (English/Spanish) inspection folder structures with standardized sub-sections.  
- **Controlled Access:** Uploads folders to a private Google Drive, granting upload-only permissions to contractors via unique URLs.  
- **Scoped Line-Item Extraction:** Gathers, cleans, and formats approved project-manager line items for export.  
- **Image & Description Handling:** Generates per-section descriptive text files and demo images for contractors.  
- **ZIP Archive Output:** Bundles folders into ready-to-share ZIP files for property and vendor coordination.  
- **Legacy Compatibility:** Originally designed for a now-deprecated internal system; logic preserved for educational and technical demonstration.

---

## ⚙️ Tools & Libraries

- `Python 3.x`
- `Selenium`
- `BeautifulSoup4`
- `Requests`
- `OpenCV`
- `Zipfile`, `OS`, `Shutil`
- `Google Colab` (runtime environment)

---

## 🖥️ Demonstration

Below are sample (simulated) screenshots and folder outputs generated during execution.  
*(No live or proprietary systems are accessed.)*

📁 property_workorder_automation_pipeline/ ├── 01_generate_inspection_folders.ipynb ├── 02_extract_reviewed_lineitems.ipynb ├── demo_screenshots/ │   ├── portal_login_demo.png │   ├── workorder_dashboard_demo.png │   └── bilingual_folder_output.png └── outputs/ └── property_1234_TO.zip

> 🖼️ *Screenshot Example:*  
> ![Demo Output](demo_screenshots/bilingual_folder_output.png)  
> *Sample folder structure generated during the inspection automation phase.*

---

## 🧩 Ethical Notice

This project automates a **legacy property-management workflow** once used in a private environment that no longer exists.  
All included screenshots and code are for **technical demonstration and educational purposes only.**  
No live data, credentials, or proprietary information are accessed, stored, or distributed.

---

## 📂 Repository Structure

. ├── 01_generate_inspection_folders.ipynb   # Creates bilingual inspection folders ├── 02_extract_reviewed_lineitems.ipynb    # Extracts and structures approved line items ├── demo_screenshots/                      # Example screenshots for demonstration ├── outputs/                               # Generated ZIP archives ├── LICENSE                                # MIT License └── README.md                              # Project documentation

---

## 🧱 Setup & Usage

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/property_workorder_automation_pipeline.git
   cd property_workorder_automation_pipeline

2. Install Dependencies

pip install selenium beautifulsoup4 requests opencv-python


3. Run on Google Colab

Upload both notebooks.

Provide environment credentials (if needed) via .env variables.

Execute each section sequentially to generate or extract folders.



4. Outputs

ZIP folders containing inspection structures and review summaries appear in the /outputs directory.





---

📘 License

This project is licensed under the MIT License — see the LICENSE file for details.


---

✨ Author

[Anthony E.]
Data & Automation Specialist
💼 https://www.linkedin.com/in/anthony-edeza
📧 aned0227@gmail.com


---

> “Automating real-world workflows into structured, analyzable data pipelines — one property at a time.”
