# logs
========

####Smart way to display git logs.


## Install

Just put the **logs** file in the classpath.

In case of Ubuntu :

1. Open the terminal.
2. Open the file .bashrc in Home directory using your favorite text editor. (e.g. gedit, vim, vi)
3. Appened the below line to the end of the file.

    ```
      if [ -f ~/scripts/logs ]; then
        . <path_to_file>/logs
      fi
    ```

## Usage

Once you are done with the installation part. Just open new terminal and follow steps:

1. Move to git respository using "cd" command.
2. Enter command "logs". The output will be something like as shown below:
    ```shell
       2dfd305 Puneet[2013-02-11] Fixed mozRankRequestUrlString problem in MozRankCountRule.

       b5c75ac Puneet[2013-02-11] Fixed mozRank problem.

       531d1e1 Puneet[2013-02-11] Added Lorem ipsum in JobBrowserExistenceRule bootstrap.
    ```
3. Enter command `logs <DAY_OF_CURRENT_MONTH>`. This command will show all the git commits before 10th of current month.

   **NOTE**: *DAY_OF_CURRENT_MONTH* must be of two digits. eg: logs 01.
4. Enter the command `logs <DAY> <DAY>`. This command will show all the git commits after first parameter DAY of the current month and before sencond parameter DAY of the current month.
5. Enter the command `logs <DATE>`.  This command will show all the commits before specified date.
  
   **NOTE**: Parameter DATE must in format ```yyyy-mm-dd```. Example: 2012-02-12
6. Enter the command `logs <DATE> <DATE>`. This command will show all the commits after the first date parameter and before the second date parameter.
