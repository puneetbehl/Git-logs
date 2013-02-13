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
    ```bash

       2dfd305 Puneet[2013-02-11] Fixed mozRankRequestUrlString problem in MozRankCountRule.

       b5c75ac Puneet[2013-02-11] Fixed mozRank problem.

       531d1e1 Puneet[2013-02-11] Added Lorem ipsum in JobBrowserExistenceRule bootstrap.
    ```
3. Enter command `logs <DAY_OF_CURRENT_MONTH>`. This command will show all the git commits after 10th of current month.

    **NOTE**: *DAY_OF_CURRENT_MONTH* must be of two digits. eg: logs 01.

4. Enter the command `logs <DAY> <DAY>`. This command will show all the git commits after first parameter DAY of the current month and before sencond parameter DAY of the current month.

    **NOTE**: The second parameter day's commits are excluded.

5. Enter the command `logs <DATE>`.  This command will show all the commits after specified date.
    
    **NOTE**: Parameter DATE must in format ```yyyy-mm-dd```. Example: 2012-02-12.

6. Enter the command `logs <DATE> <DATE>`. This command will show all the commits after the first date parameter and before the second date parameter.

## Examples

* ###logs
   ```bash

    2dfd305 Puneet[2013-02-11] Fixed mozRankRequestUrlString problem in MozRankCountRule.

    b5c75ac Puneet[2013-02-11] Fixed mozRank problem.

    531d1e1 Puneet[2013-02-11] Added Lorem ipsum in JobBrowserExistenceRule bootstrap.

    a972fda Puneet[2013-02-11] Code refactored & optimized in LoginExistenceRule & also implement...

    5d38c10 Puneet[2013-02-11] Code refactored & optimized in MozRankCountRule & also implemented...

    2ccb4ed Puneet[2013-02-11] Code refactored & optimized in LoadTimeSizeRule & also implemented t...

    8646c71 Puneet[2013-02-11] Modified scaffold template code.
    
    ```
* ###logs 10
   ```bash

    ec8d7e3 Puneet[2013-02-12] Code generalized in NativeCareerAppLinkExistenceRule and also impl...

    b7ef153 Puneet[2013-02-12] Code refactored & optimized in RedirectLinkExistenceRule and also imp...

    331f3c0 Puneet[2013-02-12] Code refactored and optimized in ThumbFriendlyExistenceRule & also...

    2dfd305 Puneet[2013-02-11] Fixed mozRankRequestUrlString problem in MozRankCountRule.

    b5c75ac Puneet[2013-02-11] Fixed mozRank problem.

    531d1e1 Puneet[2013-02-11] Added Lorem ipsum in JobBrowserExistenceRule bootstrap.

    a972fda Puneet[2013-02-11] Code refactored & optimized in LoginExistenceRule & also implemente...

    5d38c10 Puneet[2013-02-11] Code refactored & optimized in MozRankCountRule & also implemented ...

    2ccb4ed Puneet[2013-02-11] Code refactored & optimized in LoadTimeSizeRule & also implemented...

    8646c71 Puneet[2013-02-11] Modified scaffold template code.

   ```
* ###logs 05 07
    ```bash

    dc1ace7 Puneet[2013-02-06] Code optimized in AnalyticsExistenceRule & also implemented test c...

    7e6c79d Puneet[2013-02-06] Modified mail template for report.

    7b614d5 Puneet[2013-02-06] Added score on the top of site report detail page.

    c16c863 Puneet[2013-02-06] Changed favicon icon to iMomentous icon.

    034a082 Puneet[2013-02-06] Added more keywords in AdvanceSearchExistenceRule.

    1a1a0ba Puneet[2013-02-06] Fixed bugs in ImagesCountRule & also implemented test cases for th...

    305b442 Puneet[2013-02-06] Fixed bugs in VisibleImagesCountRule & also implemented test cases f...

    323e2f5 Puneet[2013-02-06] Fixed bugs in CdnImagesCountRule & also implemented test cases for C...

    b78acec Puneet[2013-02-06] Change the type of reward points & penalty points from BigInetger to...

    19dc09b Puneet[2013-02-06] Code refactored & implemented test cases for AssessmentExistenceRule.

    617bec4 Puneet[2013-02-05] Code refactored in SearchExistenceRule & SocialExistenceRule.
    
    ```
* ####logs 2012-12-31
    ```bash

    b1c849c Puneet[2013-01-01] Migration scripts updated.

    5c3ca8a Puneet[2013-01-01] Leaving date validation modified.

    f60a4a5 Puneet[2013-01-01] Fixed criteria in method 'hasExtraWorkByExpiryDate'

    e41fde0 Puneet[2012-12-31] Fixed compOff notification problem.

    5a2215e Puneet[2012-12-31] Fixed LeaveRecord saving problem.

    4462897 Puneet[2012-12-31] Fixed employee supervisor problem.

    f025f34 Puneet[2012-12-31] Fixed mail problem.

    466a62c Puneet[2012-12-31] Method created in User.groovy to check if user has extra work which...

    7f62180 Puneet[2012-12-31] Method created to update compOff balance.
    
    dfddafc Puneet[2012-12-31] Validation modified.
    
    ```
* ###logs 2012-12-16 2012-12-20
   ```bash

    8726f84 Puneet[2012-12-16] Code refactored in gsps.

    946264b Puneet[2012-12-16] Created template _addMemberForm.gsp.
    
    cfaf06c Puneet[2012-12-18] Date error fiixed in defaultDate tag.

    6c86b58 Puneet[2012-12-18] Hidden field named attendanceExceptionName is added in AttendanceE...

    3ddec23 Puneet[2012-12-18] Error messages code added in message.properties
    
    c1f1e75 Puneet[2012-12-19] Fixed templates used in dashboard.

    3c45154 Puneet[2012-12-19] Modifies methods which find AttendanceException, ExtraWork LeaveRec...

    38304ee Puneet[2012-12-19] Fixed creating new user error in UserService.groovy
    
    ```
