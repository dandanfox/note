# basic
    1. .git directory
    2. staging Area
    3. Working Directory

![relationship](https://git-scm.com/book/en/v2/images/areas.png)

## git rm
    just like
        1.rm file
        2.git add file

## git add revert
    1.modify or add revert
        git reset file

    2.git rm revert
        git checkout HEAD file

## git rm --cached 
to ignore some had commit but now you want to ignore,something you not add in .gitignore file

        git rm --cached file

        #the file from staging Area to delete and became untrace state

## git log
        # show last one log,-p show ditail , -1 limit count
        1.git log -p -1

        # show just this file's change log
        1.1 git log -p file

        # show counting for log(3 file modify,100 line code new add,40 line deleted)
        2.git log --stat

        #show oneline ,maybe useful
        3.git log --pretty=oneline

        #since limit time
        4.git log --since=2.weeks
          git log --since=7.months

        #show brach graph,Head point,braches
        5.git log --decorate --oneline --graph --all 
        git config --global alias.lga 'log --decorate --oneline --graph --all'


## git log limit
        1.time --after,--before
        2.--commiter="sha1 checksum"
        3.--author='author name'
        4. -(n) limt num
        5.--grep 'commit message'
        6 -S 'adding or removing code matching the string'

## git commit undo
        git commit --amend

## git checkout undo
        # modify a file ,before use git add,if you want to revert the file
        git checkout file
        
        

