## look shell info
        1.cat /etc/shells
            look linux installed shell
        2.echo $SHELL
## write
            echo "$USER"
            echo "today is \c";date
            echo "number of login:\c";who|wc -l
            echo "Calandar"
            cal
## diff with "" ,'',``
        1."" can know $
        2.'' just output as the same
        3.`` exec command

## diff with >, >>, <
        1.> overwrite to a file
        2.>> append to a file
        3.< read from a file
## if
        #!/bin/sh
        if [ $1 -gt 0 ];then
        echo "$1 > 0"
        elif [ $1 -eq 0 ];then
        echo "$1 = 0"
        else
        echo "$1 < 0"
        fi

        -gt >
        -lt <
        -le <=
        -gs >=
        -eq =
        -ne !=
        
        # file empty?
        -s file
        # file not a directory,exist and is a noraml file
        -f file
        # is a directory
        -d file
        # file can read
        -r file
        # file can write
        -w file
        # file can execute
        -x file
        
        ! expression
        expressiona -a expressionb
        expressiona -o expressionb
        
## loop
        for i in 1 2 3 4 5
        do
        echo welcome $i time
        done