# Benfords-Law-Forensic-Tool
An automated Excel tool for forensic accountants that utilizes Benford's Law to conduct forensic analysis. Includes First Digit, Second Digit, First-Two Digit, Last-Two Digit, and Duplication tests. Graphically displays results. Designed for audit, forensic accounting, and fraud screening.
---
## Overview
This project is an Excel tool that allows the user to input numerical transaction data (a ramdom sample from a geometric or approximately geometric sequence) into the Data sheet. The tool will generate several tables and visualizations, running five distinct tests to detect abnormal duplications and other anomalies. The tool does not neccesarily prove the existence of fraud, but it does aid in the forensic analysis process by identifying and screening anomalies. Results ought to be interpreted within their proper accounting context.
--
## Tests
1. **First Digit Benford's Law Test**
2. **Second Digit Benford's Law Test**
3. **First-Two Digit Benford's Law Test**
-Generates graph along with Upper-Bound limit, which can be changed by N and Z-Score input options
4. **Last-Two Digit Benford's Law Test**
-Supports whole numbers and cents, generates graph assuming expected values follow a uniform distribution. Allows for various different modes of analysis for small transactions, credit transactions, etc.
5. **Duplication Test**
-Identifies duplicate amounts in descending order

All outputs are automatically generated.
--
## How to Use
1. Download Excel workbook from the 'Tool' folder
2. Open file in Excel and enable macros. **Note that this is not required. Macros are only used to refresh pivot tables**
3. Paste transactional data into Column D of the Data sheet. A-C can be used for ancillary data.
4. Select Last-Two Digit test modes and filter scope (minimum value) of analysis using the drop down options
5. Review tables and graphs. Adjust N value for First-Two Digit Upper Bound if desired. Review calculated MAD values.

--
## Notes
-Not all data sets conform to Benford's Law. Requires random samples from geometric sequences or approximately geometric sequences, such as the base data provided (court purchasing card transactions).

-Upper Bound Limit approaches the expected value (Benford's Law) as N increases. Manual adjustments to N as provided in the tool should be conducted within the context of professional risk assesment. Statistical significance is different than practical significance. 

--
## Sample Data and Attribution 
This project includes sample data from a real case as provided by Mark J. Nigrini on his website. The transactions are card purchases from a court in Pennsylvania and includes 2009-2014 data.
Mark J. Nigrini's research on Benford's Law and his publication, Forensic Analytics: Methods and Techniques for Forensic Accounting Investigations Second Edition were foundational in the creation of this tool.

**Reference:**
Nigrini, M. J. *Forensic Analytics: Methods and Techniques for Forensic Accounting Investigations Second Edition*

All data is used for non-commercial, educational use.
--
## Macros
-This Excel workbook contains VBA macros that are used only to refresh pivot tables. They need not be enabled.

## Disclaimer
-The project is intended for analytical and educational use. It doesn't prove fraud, and should not replace professional judgment. 
