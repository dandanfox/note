## find -exec
    # -exec end with ;but must use \;keep jianrong
    # {} means the result of find
    find /etc/ -name sources.list -exec ls -alh {} \;