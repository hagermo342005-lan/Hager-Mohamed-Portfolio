# Activity 2: Digital Forensics Practical Analysis

**Digital Forensics | Metadata Analysis | Evidence Examination**

## Overview

This activity presents two practical digital forensic experiments using **ExifTool** and **Autopsy** to examine video and image files, extract metadata, and document technical findings.

## Practical Experiments

### 01. Video File Analysis

**Evidence:** `13413499_2732_1440_25fps.mp4`

**Tools:** ExifTool 13.59, Autopsy 4.23.1

**Main Procedures:**
- Extracted video metadata using ExifTool.
- Examined file format, resolution, encoding, and timestamps.
- Added the video to an Autopsy forensic case.
- Reviewed the video in the Image/Video Gallery.

**Key Findings:**

| Property | Result |
|---|---|
| File Format | MP4 |
| File Size | Approximately 27 MB |
| Resolution | 2732 × 1440 |
| Video Compressor | avc1 / libx264 |
| Color Metadata | BT.709 |
| Rotation | 0° |
| Duration Fields | Reported as 0 seconds |
| Autopsy Results | Video displayed in Image/Video Gallery |
| Hash Set Hits | 0 reported |

**Observation:** Some duration and internal date fields returned zero values and require independent validation. The metadata alone cannot establish the video's authenticity or recording history.

**Full Report:** [View Video File Analysis Report](Video-File-Analysis.pdf)

---

### 02. Picture File Analysis – Computer-Created Files

**Evidence:** `Bust_of_Germanicus_front_-_Getty_Museum_(2021.66).jpg`

**Tools:** ExifTool 13.59, Autopsy 4.23.1

**Main Procedures:**
- Reviewed common types of computer-created files.
- Extracted JPEG metadata using ExifTool.
- Examined the selected project folder using Autopsy.
- Reviewed image properties, timestamps, and embedded XMP metadata.
- Compared findings reported by both tools.

**Key Findings:**

| Property | Result |
|---|---|
| File Format | JPEG |
| File Size | Approximately 9.8 MB |
| Resolution | 9749 × 12141 |
| Image Size | Approximately 118.4 Megapixels |
| Color Profile | sRGB2014 |
| JPEG Encoding | Baseline DCT |
| Autopsy MD5 | `5b77de9a519f6a465e6f5452701b8d3f` |
| Hash Set Hits | 0 reported |

**Important Observations:**
- Both tools reported matching image dimensions.
- Modification timestamps were consistent.
- Creation timestamps differed by approximately one second.
- ExifTool identified embedded XMP metadata associated with The J. Paul Getty Museum.
- Autopsy displayed the image and its technical attributes.

**Full Report:** [View Picture File Analysis Report](Picture-File-Analysis.pdf)

---

## Tools & Technologies

| Tool | Purpose |
|---|---|
| ExifTool | Metadata extraction and examination |
| Autopsy | Digital forensic case management and file examination |
| MD5 | File hash identification |
| XMP | Embedded descriptive metadata |

## Overall Results

The experiments demonstrated how different forensic tools can provide complementary information about digital files.

**Main Outcomes:**

1. Successfully extracted and documented available metadata from an MP4 video and a JPEG image.
2. Examined both evidence files within Autopsy forensic cases.
3. Identified file properties, dimensions, timestamps, encoding information, and embedded metadata.
4. Compared findings between ExifTool and Autopsy.
5. Identified metadata inconsistencies and limitations requiring further verification.

**Key Finding:** Digital metadata provides valuable investigative information, but individual metadata fields must be interpreted carefully and supported by independent evidence before drawing forensic conclusions.

## Limitations

- The examination focused on selected files and project folders, not a complete forensic image of an entire computer.
- Metadata and timestamps do not independently prove file authenticity or authorship.
- The video duration fields require independent playback and decoding validation.
- The Autopsy MD5 value has not yet been independently compared.
- Zero hash-set hits do not establish that a file is safe or authentic.

## Skills Developed

- Digital Forensic Examination
- Video and Image Metadata Analysis
- ExifTool and Autopsy
- File Properties and Timestamp Analysis
- XMP Metadata Examination
- Evidence Documentation and Interpretation

## References

- [ExifTool Official Documentation](https://exiftool.org/)
- [Autopsy Digital Forensics Platform](https://www.autopsy.com/)
- [NIST](https://www.nist.gov/)

## Academic Information

- **University:** Egyptian Russian University (ERU)
- **Faculty:** Faculty of Artificial Intelligence
- **Department:** Cyber Security
- **Course:** Digital Forensics
- **Instructor:** Dr. Ali Allam
- **Academic Year:** 2026
- **Team Members:** Hager Mohamed Elkhamy, Yasmine Tarek Mohamed

---

**Activity 2 | Practical Digital Forensics | Evidence Analysis**
