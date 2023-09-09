# Inventory Management System
## 09 SEPTEMBER, 2023
## 3:00 PM - 3:46 PM

# References
- etcd.XLSX Spreadsheet | [LINK](https://docs.google.com/spreadsheets/d/1_oHivMUs1j4XZFSn3yZTKNkx50YXNYqU/edit#gid=338006155)
- Requirements Document | [LINK](https://docs.google.com/document/d/1kqVSy1tVPH7XL-YVOuwbdmF2fAnJldYFF-MBTGYnDTE/edit)

# Minutes   
- Discussed Excel: Explained server information
- Address Format: Emphasized that IP addresses should be in the format "IP address:port" to accommodate multiple APIs running on the same addre
- Tree Format: Considered implementing a tree format for data presentation
- Program Parts: Mentioned two program parts - IMS and IMS Server
- File Upload: Demonstrated the usage of "ims UPLOAD etcd.xlsx" for uploading sheet data
- Key Retrieval: Explained that "ims get keys" lists all keys
- API Upload: Noted that uploading "upload api.xlsx" also uploads APIs
- Handling Incomplete Keys: Mentioned the correct retrieval of output even with incomplete keys
- Value-Based Retrieval: Highlighted that values can be retrieved by specifying just the value, e.g., "ims GET 32GB
- Key Creation: Described the key creation process with "ims create -k anoop/xyz/key -v value
- Key Deletion: Explained that "ims delete anoop/xyz/key" deletes keys
- Data Retrieval: Mentioned that "ims all done" retrieves all data
- Output Location: Indicated that output is saved in "output.txt" for CLI searches
- Concern Raised: Amit sir raised a concern about accidentally deleting all data with "ims delete

Varad Sir's Inputs:
- Hierarchy starts from DC DR in the Requirement document - In kubernetes it starts from Namespace
- Should be able to convert data to YAML or JSON format using the "-o" option
- Proposed the option to get output in YAML or JSON format //(kubectl get allows such output as well)
- Discussed limiting the number of ETCD nodes from 5 to 1 for specific roles in the nodes tab
- Per analogy, physical or virtual machines are nodes
- Getting nodes from the "DR" namespace using "ims get nodes" to display relevant host information
- Emphasized the importance of OS over version in the Spreadsheet
- Noted the presence of clustered applications in the main sheet, agreed with Amit Sir to for creating
- Mentioned that Kubernetes commands and their outputs will be provided in video format
