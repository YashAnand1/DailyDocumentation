# Inventory Management System
## 09 SEPTEMBER, 2023
## 3:00 PM - 3:46 PM

# References
- etcd.XLSX Spreadsheet | [LINK](https://docs.google.com/spreadsheets/d/1_oHivMUs1j4XZFSn3yZTKNkx50YXNYqU/edit#gid=338006155)
- Requirements Document | [LINK](https://docs.google.com/document/d/1kqVSy1tVPH7XL-YVOuwbdmF2fAnJldYFF-MBTGYnDTE/edit)

# Minutes   
- Discussed Excel: Explained server information.  
- Address Format: Emphasized that IP addresses should be in the format "IP address:port" to accommodate multiple APIs running on the same address.  
- Tree Format: Considered implementing a tree format for data presentation.
- Program Parts: Mentioned two program parts - IMS and IMS Server.
- File Upload: Demonstrated the usage of "ims UPLOAD etcd.xlsx" for uploading sheet data.
- Key Retrieval: Explained that "ims get keys" lists all keys.
- API Upload: Noted that uploading "upload api.xlsx" also uploads APIs.
- Handling Incomplete Keys: Mentioned the correct retrieval of output even with incomplete keys.
- Value-Based Retrieval: Highlighted that values can be retrieved by specifying just the value, e.g., "ims GET 32GB."
- Key Creation: Described the key creation process with "ims create -k anoop/xyz/key -v value."
- Key Deletion: Explained that "ims delete anoop/xyz/key" deletes keys.
- Data Retrieval: Mentioned that "ims all done" retrieves all data.
- Output Location: Indicated that output is saved in "output.txt" for CLI searches.
- Concern Raised: Amit sir raised a concern about accidentally deleting all data with "ims delete."

Additional Points:
- Discussed hierarchy starting from DC DR and adding analogies.
- Mentioned the ability to run commands using "kubectl get namespace" on any node.
- Considered converting data to YAML or JSON format using the "-o" option.
- Suggested allowing data uploads from JSON.
- Proposed the option to get output in YAML or JSON format.
- Discussed limiting the number of ETCD nodes to 5-6 for specific roles.
- Introduced the analogy that physical or virtual machines are considered nodes.
- Discussed retrieving nodes from the "DR" namespace using "ims get nodes" and displaying relevant host information.
- Emphasized the importance of OS over version in node information.
- Noted the presence of clustered applications in the main sheet.
- Mentioned that Kubernetes commands and their outputs will be provided in video format.
