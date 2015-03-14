# rackspace-api-cli
a dirty hack collection of cli scripts developed to work with rackspace api

#rscloudfiles

Features:
- Add file or directory to Rackspace cloud files
- Extract file to Rackspace cloud files
- Show all Rackspace link and region
- Show generated token for whatever reason
 
Example Commands

  -PUT  -F (content-type) (target file) (destination link)

  (e.g., ./rscloudfile -PUT -F application/x-gzip /home/XXX.tar.gz  https:\/\/rs.clouddrive.com\/v1\/MossoCloudFS_1212121\/Folder1\/)

  -GET  -F -X (target file) (target link)

  (e.g., ./rscloudfile -F -X  XXX.tar.gz https:\/\/rs.clouddrive.com\/v1\/MossoCloudFS_1212121\/Folder1\/)

  -SHOWDRIVE

  (e.g., ./rscloudfile -SHOWDRIVE)

  -SHOWTOKEN

  (e.g., ./rscloudfile -SHOWTOKEN)
