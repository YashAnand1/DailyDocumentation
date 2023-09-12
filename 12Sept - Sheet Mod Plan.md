# Spreadsheet Modification Plan
   
[etcd.XLSX](https://docs.google.com/spreadsheets/d/1_oHivMUs1j4XZFSn3yZTKNkx50YXNYqU/edit#gid=1916382268) will be modified based on the analogies provided below, while referring to the [e-T sheet](https://docs.google.com/spreadsheets/d/1eusMRNqXoCwfI_HlH9ILodZLxxTTpZX-4B2uOusbJ9A/edit#gid=0).

<div align="center">
  
| Resources      | Analogy                                        | Includes | Remarks                   |
|----------------|------------------------------------------------|-|--------------------------------------------|
| Clusters       | Client Org NAME -                             | |                  -                          |
| Namespace      | dc(/DR?) AND ENVIRONMENT | Hierarchy starts here - Varad sir     |
| Deployments    | Application name                               | Tomcat IP| Client Applications - e.g. Vahan, Sarathi  |
| Pods           | Client applications of Deployment applications | | Sarathi Client Application - e.g. SarathiService, NewDL, RenewDL, DBServer |
| Containers     | Further details of client applications         | | e.g. SarathiService runs on Tomcat 9, includes db images |
| replicaset     | Applications that are load balanced            |  |                   -                        |
| statefulset    | Clustered applications                          | | Will be retrieved from etransport sheet     |
| Nodes          | Server Types - Phys or VM or K8 Clusters       | |                     -                      |
| Images         | Container images                                | | Platform - Java 8/ Java 11, PHP 7 |
| Services       | -                                              | | DB Cluster IPs, App Cluster IPs or Individual App IPs |
| ConfigMap      | App Configuration                               | | 1 config per app                             |
| PV             | Total storage                                  | | -            |
| PVC            | Individual Application Shared Storage          | | RWO/RWX - SAN Volume/NAS Volumes            |
| Ingress        | Incoming LBs - HAProxy                         |  |                    -                       |

</div>
