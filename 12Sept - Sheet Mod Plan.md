|-------------|-----------|---------------|
Resources	Analogy	Included Attributes/Remarks
Clusters	Client Org NAME	-
Namespace	dc(/DR?) AND ENVIRONMENT	Hierarchy starts here - Varad sir // from analogies mail
Deployments	Application name	Client Applications - e.g. Vahan, Sarathi
Pods	Client applications of Deployment applications	Sarathi Client Application - eg. SarathiService, NewDL, RenewDL, DBServer
Containers	further details of client applications	e.g. SarathiService runs on Tomcat 9, includes db images // from analogies mail
replicaset	Applications that are load balanced	-
statefulset	clustered applications	will be retrieved from etransport sheet
Nodes	Server Types - Phys or VM or K8 Clusters	-
Images	container images	Platform - Java 8/ Java 11, PHP 7 // from analogies mail
Services	-	DB Cluster IPs, App Cluster IPs or Individual App IPs
ConfigMap	App Configuration	1 config per app
PV	total storage	RWO/RWX - SAN Volume/NAS Volumes
PVC	Individual Application Shared Storage 	RWO/RWX - SAN Volume/NAS Volumes
Ingress	Incoming LBs - HAProxy	-
-------------------------------------------
