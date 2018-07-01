# Invoke-TempDavFS
In Memory Powershell WebDav Server

## DESCRIPTION
 
Creates a memory backed webdav server using powershell that can be mounted as a filesystem.

Note: Mounting the remote filesystem on windows implies local caching of accessed files in the C:\Windows\ServiceProfiles\LocalService\AppData\Local\Temp\TfsStore\Tfs_DAV system directory.
 
## USAGE
'''
Import-Module Invoke-TempDavFS.psm1

Invoke-TempDavFS
'''

## PARAMETERS

port: Port to listen on, defaults to 8080.

sharename: Name of the share to export, defaults to Temp
 
export: Listen on any interface, instead of localhost (requires admin).

auth: Require authentication, defaults to false.
