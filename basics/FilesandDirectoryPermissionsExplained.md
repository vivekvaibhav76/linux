<h1>Files and Directory Permissions Explained</h1>

<h3>File type</h3>
Lets consider you have a file in your system and you want to know its permission, owner, group, file size, date of creation, etc.
Execute the command ls -l
```sh
ls -l
```
You'll get to know the file type.

Symbol      Type
-           Regular file
d           Directory
l           Symbolic link

<h3>Permission</h3>
To know the permission of the file use ls -l command

```sh
ls -l
```
Output will be like:

-rw-rw-r--  1   <user>   <group>  <filesize>  <Created Date>  <Created Time>  <Name of File>
  
  
  Symbol          Permission
 
  r               Read
  w               Write
  x               Execute
  
<h3>Permissions- File vs Directories</h3>
  
  Permission          File                                        Directory
  Read(r)         Allow files to read                Allow file names in the directory to be read
  
  Write(w)        Allows a files to modified         Allow entries to be modified within the directory
  
  Execute(x)      Allows the excution of a file      Allows access to contents and metadata for entries
  
  
