# rackspace-api-cli
a dirty hack collection of cli scripts developed to work with rackspace api

#rscloudfiles

Features:

 -PUT  -F (content-type) (target file) (destination link)"

  (e.g., ./rscloudfile -PUT -F application/x-gzip /home/XXX.tar.gz  https:\/\/rs.clouddrive.com\/v1\/MossoCloudFS_1212121\/Folder1\/)

 -GET  -F -X (target file) (target link)"

  (e.g., ./rscloudfile -F -X  XXX.tar.gz https:\/\/rs.clouddrive.com\/v1\/MossoCloudFS_1212121\/Folder1\/)

 -SHOWDRIVE"

  (e.g., ./rscloudfile -SHOWDRIVE)

