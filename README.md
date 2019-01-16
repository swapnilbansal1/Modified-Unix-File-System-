# Modified Unix File System 

**Modified Version of V6 Unix File System


Project Statement :
The modified Unix Version 6 file system that we designed in project 2-part 1 is to be extended to implement the following additional commands:

(a) cpin externalfile v6-file
Creat a new file called v6-file in the v6 file system and fill the contents of the newly created file with the contents of the externalfile.

(b) cpout v6-file externalfile
If the v6-file exists, create externalfile and make the externalfile's contents equal to v6-file.

(c) mkdir v6-dir
If v6-dir does not exist, create the directory and set its first two entries . and ..

(d) rm v6-file
If v6-file exists, delete the file, free the i-node, remove the file name from the (parent) directory that has this file and add all data blocks of this file to the free list.

(e) q
Save all changes and quit.


1. fsaccess.c : **main code
2. Readme.md : **readme file
3. Results.pdf : **sample results and commands output report
4. sf.txt: **smallfile for testing
5. lf.txt: **large file for testing

file name: fsaccess.c

**Compiler Used:
CC  Compiler

**Platform used: 
UNIX and C
 
**Compiling and running code.



*Steps (on csgrads1.utdallas.edu linux server):
1. The source code file was added to server using WINSCP software.
2. Next type "vi fsaccess.c" to see your Source code. 
3. Type "i" to make any changes to the source code
4. Type ":wq" to save the changes made inside the code.
5. You can compile the source code by typing the command "cc fsaccess.c"
6. Use the command "./a.out" to run your source code.


**Commands using in program output:

1. initfs :: initialization of file system 
             >>initfs <file system name> <number of blocks> <number of inodes>

2. cpin   :: creates new mv6 file and fill the contents of 
 	    >>cpin <external file> <mv6-file> 
 
3. cpout  :: creates external file and copies content of mv6 file into external file 
 	    >>cpout <mv6-file> <external file>
 
4. mkdir  :: making directory in current directory
 	    >>mkdir v6-dir
5. rm     :: removing directory  from current directory
            >>rm v6-dir
6. q      :: save all changes and quiet
	    >>q
