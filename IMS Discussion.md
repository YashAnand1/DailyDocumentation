# Inventory Management System
## 09 SEPTEMBER, 2023
## 3:00 PM - 3:36 PM

# References
- etcd.XLSX Spreadsheet | [LINK](https://docs.google.com/spreadsheets/d/1_oHivMUs1j4XZFSn3yZTKNkx50YXNYqU/edit#gid=338006155)
- Requirements Document | [LINK](https://docs.google.com/document/d/1kqVSy1tVPH7XL-YVOuwbdmF2fAnJldYFF-MBTGYnDTE/edit)

# Inputs
Anoop Sir:
- Explained server information
- Explained two programs - IMS and IMS-Server
- Demonstrated the usage of :
  - `ims UPLOAD etcd.xlsx` for uploading sheet data //(For uploading sheets, `ims upload api.xlsx` too)
  - `ims get key` for listing all keys
  -  `ims get 10.249.221.22` or `ims get <IP>` for finding data of incomplete Keys
  -  `ims GET 32GB` or `ims get <value>` for finding server information from values
  -  `ims create -k anoop/xyz/key -v somevalue` for creating key-value pair
  -  `ims delete anoop/xyz/key` for deleting keys-value pair
  -  `ims all` for retrieval of all data
- Output is saved in "output.txt" for CLI searches

Amit Sir:
- What if accidentally, all data is deleted with ims delete
- Will be asking Ravi Sir to share Kubernetes outputs in video format
- Said that he had found E-Transport related data for helping the data of the sheet

Varad Sir:
- Hierarchy starts from DC DR in the Requirement document - In kubernetes it starts from Namespace
- IP addresses should be in the format "IP address:port" to accommodate multiple APIs running on the same address
- Suggested converting data to YAML or JSON format using the "-o" option
- Add option to get output in YAML or JSON format instead of .txt
- Change number of ETCD nodes from 5 to 1 for specific roles in the nodes tab
- Per analogy, physical or virtual machines are nodes
- Should be able to get nodes from `DR` using `ims get nodes` to display relevant host information
- Replace version with OS in the Spreadsheet
- Asked about clustered applications in the main sheet - agreed with Amit Sir to have Ravi Sir share Kubernetes commands and outputs
- On monday, will be connecting the analogies with the kubernetes commands according to the Requirements document
