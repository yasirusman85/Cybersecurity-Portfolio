# File permissions in Linux
## Project Description
In this activity, we are managing file permissions in the Linux environment. We'll check, modify, and describe permissions for files and directories in the /home/researcher2/projects directory.
## Check File and Directory Details
### Command:
ls -la /home/researcher2/projects
### Output:
drwx------ 2 researcher2 research_team 4096 Feb 8 15:03 .
drwxr-xr-x 3 researcher2 research_team 4096 Feb 8 15:03 ..
-rw-rw-r-- 1 researcher2 research_team 46 Feb 8 15:03 project_k.txt
-rw------- 1 researcher2 research_team 46 Feb 8 15:03 project_m.txt
-rw-rw-r-- 1 researcher2 research_team 46 Feb 8 15:03 project_r.txt
-rw-rw-r-- 1 researcher2 research_team 46 Feb 8 15:03 project_t.txt
-rw-rw-r-- 1 researcher2 research_team 46 Feb 8 15:03 .project_x.txt
drwxr-x--x 2 researcher2 research_team 4096 Feb 8 15:03 drafts
### Describe the Permissions String
10-Character String:
-rw-rw-r--
### Description:
This 10-character string represents the file permissions. The first character indicates the type of file (regular file, directory, etc.), and the next three sets of three characters each represent permissions for the owner, group, and others. In the example, the file is a regular file with read and write permissions for the owner and group, but only read permissions for others.
## Change File Permissions
### Command:
chmod o-w project_m.txt
### Output:
No output if successful.
## Change File Permissions on a Hidden File
### Command:
chmod go-w .project_x.txt
### Output:
No output if successful.
## Change Directory Permissions
### Command:
chmod 700 drafts
### Output:
No output if successful.
## Summary
In this lab, we checked and modified file and directory permissions in the /home/researcher2/projects directory. We ensured that only the researcher2 user has access to the drafts directory and its contents. Permissions for specific files were updated as needed.

