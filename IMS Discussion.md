# Inventory Management System
## 09 SEPTEMBER, 2023
## 3:00 PM - 3:46 PM

# References
- etcd.XLSX Spreadsheet | [LINK](https://docs.google.com/spreadsheets/d/1_oHivMUs1j4XZFSn3yZTKNkx50YXNYqU/edit#gid=338006155)
- Requirements Document | [LINK](https://docs.google.com/document/d/1kqVSy1tVPH7XL-YVOuwbdmF2fAnJldYFF-MBTGYnDTE/edit)

# Inputs
Anoop Sir's Inputs:
- Explained server information
- Explained two programs - IMS and IMS-Server
- Demonstrated the usage of :
- - `ims UPLOAD etcd.xlsx` for uploading sheet data //(For uploading sheets, `ims upload api.xlsx` too)
- -`ims get key` for listing all keys
- Handling Incomplete Keys can be done //(`ims get 10.249.221.22`
- Handling only values can be done //(`ims GET 32GB`
- Handling key creation can be done //(`ims create -k anoop/xyz/key -v somevalue`
- Handling key deletion can be done //(`ims delete anoop/xyz/key`)
- Handling retrieval of all data can be done //(`ims all done`)
- Output is saved in "output.txt" for CLI searches

Amit Sir's Inputs:
- What if accidentally, all data is deleted with ims delete
- Will be asking Ravi Sir to share Kubernetes outputs in video format 

Varad Sir's Inputs:
- Hierarchy starts from DC DR in the Requirement document - In kubernetes it starts from Namespace
- IP addresses should be in the format "IP address:port" to accommodate multiple APIs running on the same addre
- Should be able to convert data to YAML or JSON format using the "-o" option
- Proposed the option to get output in YAML or JSON format instead of txt
- Discussed limiting the number of ETCD nodes from 5 to 1 for specific roles in the nodes tab
- Per analogy, physical or virtual machines are nodes
- Getting nodes from the "DR" namespace using "ims get nodes" to display relevant host information
- Emphasized the importance of OS over version in the Spreadsheet
- Noted the presence of clustered applications in the main sheet, agreed with Amit Sir to have Ravi Sir share Kubernetes commands and their outputs in a video format
- On monday, will be connecting the analogies with the kubernetes commands according to the Requirements document
