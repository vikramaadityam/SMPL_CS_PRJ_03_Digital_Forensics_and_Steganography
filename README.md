# Digital Forensics and Steganography: Recovering Hidden Data from a JPG Image

## Overview

This project demonstrates the integration of **Steganography** and **Digital Forensics** by simulating a real-world investigation scenario. A secret message is embedded inside a JPG image using steganography techniques, stored on a virtual disk, deleted, and then recovered using forensic tools. The recovered image is analyzed to extract the hidden message, showcasing the complete lifecycle of data hiding, deletion, forensic recovery, and evidence analysis.

The project provides hands-on experience with industry-recognized forensic tools and highlights how digital investigators can recover hidden information from deleted files.

---

## Project Objective

The primary objective of this project is to:

- Embed hidden text inside a JPG image using steganography.
- Store the image on a simulated storage system.
- Delete the image to simulate data loss or evidence concealment.
- Create a forensic disk image of the storage media.
- Recover the deleted image using forensic analysis tools.
- Extract and verify the hidden text from the recovered image.
- Demonstrate real-world digital forensic investigation techniques.

---

## Project Workflow

```text
Original JPG Image
        │
        ▼
Steganography (SilentEye)
        │
        ▼
Image with Hidden Message
        │
        ▼
Stored on NTFS Disk
        │
        ▼
File Deleted
        │
        ▼
Disk Imaging (FTK Imager)
        │
        ▼
Forensic Analysis (Autopsy)
        │
        ▼
Recover Deleted JPG
        │
        ▼
Decode Hidden Message
        │
        ▼
Successful Recovery of Secret Data
```

---

## Technologies and Tools Used

| Tool | Purpose |
|--------|---------|
| Oracle VirtualBox | Virtual forensic environment |
| Windows Server 2022 | Operating system environment |
| SilentEye | Steganography encoding and decoding |
| FTK Imager | Disk imaging and evidence acquisition |
| Autopsy | Forensic analysis and file recovery |
| NTFS File System | Storage medium for investigation |

---

## Project Implementation

### 1. Environment Setup

- Created a virtual machine using Oracle VirtualBox.
- Added two virtual disks:
  - **2 GB Data Disk**
  - **20 GB Evidence Disk**
- Initialized and formatted both disks using NTFS.

### 2. Steganography Process

- Downloaded a JPG image.
- Used SilentEye to embed a secret text message into the image.
- Saved the encoded image on the Data drive.

### 3. Simulating Data Loss

- Deleted the encoded image.
- Emptied the Recycle Bin to simulate permanent deletion.

### 4. Evidence Acquisition

- Used FTK Imager to create a forensic image of the Data disk.
- Saved the acquired evidence image to the Evidence drive.

### 5. Forensic Investigation

- Created a new forensic case in Autopsy.
- Loaded the FTK image as a data source.
- Analyzed deleted files within the image.
- Identified and recovered the deleted JPG file.

### 6. Hidden Data Recovery

- Opened the recovered image using SilentEye.
- Decoded the hidden content.
- Successfully recovered the embedded message.

---

## Key Features

- Digital evidence acquisition using FTK Imager.
- Recovery of deleted files through forensic analysis.
- Practical implementation of image-based steganography.
- Verification of hidden data integrity after recovery.
- Simulation of a real-world cyber forensic investigation.

---

## Project Outcome

The project successfully demonstrated that:

- Data can be hidden inside image files using steganography.
- Deleted files can often be recovered using forensic tools.
- Hidden information can remain intact even after file deletion.
- Digital forensic methodologies can be used to recover and analyze concealed evidence.
- Proper forensic procedures preserve data integrity during investigations.

---

## Learning Outcomes

Through this project, the following concepts were explored:

- Digital Forensics Fundamentals
- Evidence Acquisition Techniques
- Disk Imaging and Preservation
- File Recovery and Analysis
- Data Hiding Techniques
- Steganography Detection and Extraction
- Cybersecurity Investigation Methodology

---

## Real-World Applications

This project reflects practical scenarios encountered in:

- Cybercrime Investigations
- Law Enforcement Digital Forensics
- Insider Threat Investigations
- Data Exfiltration Analysis
- Incident Response Operations
- Corporate Security Investigations
- Digital Evidence Recovery

---

## Screenshots

### 1. Environment Setup
**Figure 1.7 – Creating the 2 GB Data Disk**
Shows the creation of the NTFS data disk used for storing the steganographic image.

### 2. Steganography Process
**Figure 4.8 – Embedding Secret Text Using SilentEye**
Demonstrates the process of hiding a secret message inside the JPG image.

### 3. Evidence Acquisition
**Figure 4.7 – FTK Imager Evidence Configuration**
Shows the forensic imaging process used to acquire a copy of the disk for analysis.

### 4. Deleted File Recovery
**Figure 5.23 – Deleted JPG Identified in Autopsy**
Illustrates how Autopsy detected the deleted image file during forensic analysis.

### 5. Hidden Message Extraction
**Figure 6.5 – Successfully Recovered Hidden Message**
Shows the final recovery of the secret message from the recovered JPG image.

---

## Skills Demonstrated

- Digital Forensics
- Cybersecurity Investigation
- Evidence Handling
- Disk Imaging
- Incident Response Fundamentals
- File Recovery Techniques
- Steganography Analysis
- Forensic Tool Usage
- Documentation and Reporting

---

## Future Improvements

Potential enhancements for this project include:

- Password-protected steganography implementation.
- Comparative analysis of multiple steganography tools.
- Automated extraction using Python scripts.
- Recovery testing across different file systems.
- Integration with memory forensics techniques.
- Detection of steganographic artifacts using forensic analysis tools.

---

## Conclusion

This project successfully demonstrates the complete lifecycle of hidden data protection and forensic recovery. By combining steganography and digital forensics, the investigation shows how concealed information can be embedded within image files, survive deletion, and later be recovered through proper forensic procedures. The project provides practical experience with industry-standard forensic tools and reinforces the importance of evidence preservation, analysis, and cybersecurity investigation techniques.

---

## Author

**Ashish Yadav**

Cybersecurity Enthusiast | Digital Forensics | SOC Analyst Aspirant

---

## License

This project is intended for educational and research purposes only.
