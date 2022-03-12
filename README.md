# sshfs-dav: sshfs using WebDAV

`sshfs-dav` mounts files using SSH tunneled WebDAV

## Usage

```
sshfs [user@]host:[dir] mountpoint [-f] [-o OPTIONS]"
```
Current limitations:
- Write operations always lead to reset of mtime (mount_webdav limitation)
