# Invoke-TmpDavFS
Memory Backed Powershell WebDav Server

### Description
 
Creates a memory backed webdav server using powershell that can be mounted as a filesystem.

Note: Mounting the remote filesystem on windows implies local caching of accessed files in the C:\Windows\ServiceProfiles\LocalService\AppData\Local\Temp\TfsStore\Tfs_DAV system directory.
 
## Usage

```
Import-Module Invoke-TempDavFS.psm1

Invoke-TempDavFS
```

## Parameters

port: Port to listen on, defaults to 8080.

sharename: Name of the share to export, defaults to Temp
 
export: Listen on all interfaces instead of localhost (requires admin).

auth: Require authentication, defaults to false.
