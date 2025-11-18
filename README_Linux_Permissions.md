# Linux File Permissions Portfolio


File permissions in Linux

Project description
As a security professional, my job is to ensure that users on the research team have the correct authorization to access files and directories in the projects directory. Some of the permissions did not match the proper authorization levels, so I inspected the current permissions and updated them.

Check file and directory details
Command used:
ls -la

Output:
total 32
drwxr-xr-x 3 researcher2 research_team 4096 Dec 2 15:27 .
drwxr-xr-x 3 researcher2 research_team 4096 Dec 2 15:27 ..
-rw------- 1 researcher2 research_team 46 Dec 2 15:27 .project_x.txt
drwxr-x--- 2 researcher2 research_team 4096 Dec 2 15:27 drafts
-rw-rw-r-- 1 researcher2 research_team 46 Dec 2 15:27 project_k.txt
-rw-r----- 1 researcher2 research_team 46 Dec 2 15:27 project_m.txt
-rw-rw-r-- 1 researcher2 research_team 46 Dec 2 15:27 project_r.txt
-rw-rw-r-- 1 researcher2 research_team 46 Dec 2 15:27 project_t.txt

Describe the permissions string
Example: -rw-rw-r--
- regular file
rw- user can read/write
rw- group can read/write
r-- others can read only

Change file permissions
chmod o-w project_k.txt

Change hidden file permissions
chmod u-w .project_x.txt
chmod g+r .project_x.txt

Change directory permissions
chmod g-x drafts

Summary
I used Linux commands to examine and securely update file permissions in the projects directory.
