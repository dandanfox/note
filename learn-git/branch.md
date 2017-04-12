## branch rename
    1. git br -m oldname newname
## create branch from before commit
    1.look up what commit you want to create,find commitid
        git log lga 
    2.create a branch
    git ck -b branchname commitid
        git ck -b fix commitid

## merge fix to master
    git ck master && git merge fix && git st
    
## fix Confilexs
        <<<<<<< HEAD:index.html
        <div id="footer">contact : email.support@github.com</div>
        =======
        <div id="footer">
         please contact us at support@github.com
        </div>
        >>>>>>> iss53:index.html
        
        do someting like this ,you can see two branch modify a file in the smae position cause the confilexs        
        1.mdoify the confilexs file
        2.git ci -a ,problem is solve;
        
## add new remote branch
        #maybe should config 
        1.git config --global push.default matching
        or git config --global push.default simple
        
        #you can push localbranch to remote with a new name,or don't set servername,then default servername is the same as your localname        
        2.git push gitoschina localbranchname[:serverbranchname]

## git merge remote branch
        remote branch is also a normal branch ,do the same as a lcoal branch,with nothing difference
        
## track branch (not import,because easy to cause error)
        # use checkout create a track branch
        git ck -b localbranchname serverbarchname
        
        # change local branch's track branch
        # lcoalbrancname used if you want set another lcoalbranch track,but no need to ck to that branch
        git br -u serverbrachname [localbranchname]
        
        # show branches track info
        # you can see ahead 2 or behind 6,but almost help nothing
        git br -vv
        
## delete remote branch
        # delete a remote branch,don't add remotename        
        git push github --delete serverfix

<red style="color:red;">error</red>

<info style="text-decoration:line-through">git push github --delete githbu/serverfix</info>

## merge diff rebase
        it's too difficult to say
        rebase is not nessary to use

