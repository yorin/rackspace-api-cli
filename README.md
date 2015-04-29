rackspace-api-cli
===================
__A collection of cli scripts developed to work with rackspace api__  

_Disclaimer: This is unofficial, created without Rackspace's official support._  

_Note: Insert your Rackspace USERNAME & APIKEY to .cache/rs.conf_  
  
#rscloudfiles

Features:
- Add file or directory to Rackspace cloud files
- Extract file to Rackspace cloud files
- Show all Rackspace link and region
- Show generated token for whatever reason
- Show files/directory
- Error prompts if username and api not detected
- Added file cache to cache token and initial directory  
  data fetched from Rackspace  
 
Example Commands

  -PUT  -X (content-type) -F (target file) -L (destination link)

  (e.g., ./rscloudfile -PUT -X application/x-gzip -F XXX.tar.gz  -L https:\/\/rs.clouddrive.com\/v1\/MossoCloudFS_1212121\/Folder1\/)

  -GET  -F (target file) -L (target link)

  (e.g., ./rscloudfile -GET -F XXX.tar.gz -L https:\/\/rs.clouddrive.com\/v1\/MossoCloudFS_1212121\/Folder1\/)

  -SHOWDRIVE

  (e.g., ./rscloudfile -SHOWDRIVE)

  -SHOWTOKEN

  (e.g., ./rscloudfile -SHOWTOKEN)

  -SHOW -L (rackspace api link)

  (e.g., ./rscloudfile -SHOW -L https:\/\/rs.clouddrive.com\/v1\/MossoCloudFS_1212121)  
  (e.g., ./rscloudfile -SHOW -L https:\/\/rs.clouddrive.com\/v1\/MossoCloudFS_1212121\/Folder1)

#rsdns

Features:
- Search DNS created
- Create DNS
- Delete DNS
- SHOW DNS ID
 
Example Commands
  
  -SHOWTOKEN  
  
  (e.g., ./rsdns -SHOWTOKEN)  
  
  -LISTDOMAINS"  
  
  (e.g., ./rsdns -LISTDOMAINS)  
  
  -DOMAINID (domain id)"  
  
  (e.g., ./rsdns -DOMAINID 3456127)  
  
  -DELETE (domain id)"

  (e.g., ./rsdns -DELETE 3456127)  
  
  -CREATEDOM  -n (domain.com) -t (ttl value)"  

  (e.g., ./rsdns -CREATEDOM -n domain.com -t 84600)  
  
  -CREATEREG  -ty (A,CNAME) -n (domain or subdomain name) -ip (ip address) -t (ttl value) -did (domain id)"  
  
  (e.g., ./rsdns -CREATEREG -ty A -n domain.com -ip 127.0.0.1 -t 84600 -did 3456127)  
  
