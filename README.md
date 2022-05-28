# Disk-searcher
A multithreaded code to find files
To begin a search please run a command in the upcoming format:
java DiskSearcher <# milestoneQueueFlag> <file-prefix> <root directory>
  <destination directory> <# of searchers> <# of copiers> 
keys:
                                                                                                                                                 
  <boolean of milestoneQueueFlag> ---> Indicates whether the milestonesQueue and written to or not (in that case, it should be set to null). 
  If not, the  program executes without any writings and the queue is set to null (the constructor of the all threads receives null in 
  it’s parameter place).
  If the flag is “true”, then the milestonesQueue will store the documentation of what happened during the program and will print it.

  <file-prefix> ---> Indicates what prefix of files names the program will find.
  
  <root directory> ---> Indicates the path of the directory the program will begin the search (it will search recursively in all the diectories with in).
 
  <destination directory> ---> Indicates the path of the directory the program will copy all the files that she found in to.
  
  <# of searchers> ---> Indicates the number of seraching threads that will run simultaniously trying to find matching files.

  <# of copiers> ---> Indicates the number of copying threads that will run simultaniously trying to copy the matching files.
