## git move next /prev
        1.clone a github repo
        2.create a localbranch 'dev' in first commit
        
        3.use <git merge commitid> to move next
            git merge 46d861a
            
        4.use <git reset commitid> to move prev
            git reset a765d751
        
        5.after use git reset,some file maybe new add,or modify
        
            1.new add use git clean use clean them
    
            git clean -dfx (d:directory,f:force,x:not just .ignore file)
            
            2.modify use git checkout filename to reset them            
            git checkout README.md
