# sshfs-dav: sshfs using tunneled NFS or WebDAV

`sshfs-dav` mounts files using SSH tunneled NFS or WebDAV

## Usage

```
sshfs [user@]host:[dir] mountpoint [-f] [-p nfs|webdav] [-o OPTIONS]"
```
Current limitations:
- For webdav, write operations always lead to reset of mtime (mount_webdav limitation)
- Default prototol is nfs, does not have the mtime limition, but requires rclone >= v1.65 on server.
