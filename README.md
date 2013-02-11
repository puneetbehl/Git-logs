# logs
========

Smart way to display git logs.


## Install

Just put the logs file in the classpath.

In case of Ubuntu :

1. Open the terminal.
2. Open the file .bashrc in Home directory using your favorite text editor. (e.g. gedit, vim, vi)
3. Appened the below line to the end of the file.
  
  if [ -f ~/scripts/logs ]; then
    . <path_to_file>/logs
  fi

## Usage

Once you are done with the installation part. Just open new terminal and follow steps:

1. Move to git respository using "cd" command.
2. Enter command "logs". The output will be something like as shown below:

   2dfd305 Puneet[2013-02-11] Fixed mozRankRequestUrlString problem in MozRankCountRule.

   b5c75ac Puneet[2013-02-11] Fixed mozRank problem.

   531d1e1 Puneet[2013-02-11] Added Lorem ipsum in JobBrowserExistenceRule bootstrap.
3. Enter command "logs <DAY_OF_CURRENT_MONTH>"
