# rackspace-api-cli
a dirty hack collection of cli scripts developed to work with rackspace api  

Disclaimer:  
This is unofficial, created without Rackspace's official support.  

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
