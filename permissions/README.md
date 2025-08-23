# Holberton School Shell Scripts - Permissions

This repository contains a series of shell scripts that manage file and directory permissions, ownerships, and user settings.

## Scripts Overview

### 0. My name is Betty (`0-iam_betty`)
Switches the current user to the user `betty`.  
- Must use exactly 8 characters for the command (+1 for newline).  
- Assumes `betty` exists.

### 1. Who am I (`1-who_am_i`)
Prints the effective username of the current user.

### 2. Groups (`2-groups`)
Prints all groups the current user belongs to.

### 3. New owner (`3-new_owner`)
Changes the owner of the file `hello` to the user `betty`.  
- Requires `sudo` if not the file owner.

### 4. Empty! (`4-empty`)
Creates an empty file called `hello` in the working directory.

### 5. Execute (`5-execute`)
Adds execute permission to the **owner** of the file `hello`.

### 6. Multiple permissions (`6-multiple_permissions`)
Adds:  
- Execute permission to **owner** and **group**.  
- Read permission to **others**.  
For the file `hello`.

### 7. Everybody! (`7-everybody`)
Adds execute permission to **owner**, **group**, and **others** for the file `hello`.  
- Comma usage is not allowed.

### 8. James Bond (`8-James_Bond`)
Sets the permissions of the file `hello` as:  
- Owner: no permissions  
- Group: no permissions  
- Others: all permissions  

### 9. John Doe (`9-John_Doe`)
Sets the mode of the file `hello` to: `-rwxr-x-wx`.  
- Comma usage is not allowed.

### 10. Look in the mirror (`10-mirror_permissions`)
Sets the mode of the file `hello` the same as the file `olleh`.  
- Works for any permission mode.

### 11. Directories (`11-directories_permissions`)
Adds execute permission to **all subdirectories** of the current directory for owner, group, and others.  
- Regular files remain unchanged.

### 12. More directories (`12-directory_permissions`)
Creates a directory called `my_dir` with permissions `751`.

### 13. Change group (`13-change_group`)
Changes the **group owner** of the file `hello` to `school`.  

### 14. Owner and group (`14-change_owner_and_group`)
Changes the **owner** to `vincent` and the **group owner** to `staff` for all files and directories in the working directory.

### 15. Symbolic links (`15-symbolic_link_permissions`)
Changes the **owner** and **group** of `_hello` (symbolic link) to `vincent` and `staff`.

### 16. If only (`16-if_only`)
Changes the owner of `hello` to `vincent` **only if** the current owner is `guillaume`.
