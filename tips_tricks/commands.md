man
===
    $ man nmap

tldr
===
    $ tldr nmap
    $ tldr plocate

plocate
===
    $ plocate myfile.txt

cd
===
Go back to your previous directroy
    $ cd -
Go back home / keyborad shortcut "FN + Shift + ESC
    $ cd ~
Go to the main partition of operationg system
    $ cd /

ip a / ifconfig / hostname
===
Will return your ip address - pen test
    $ ip a
    $ ifconfig
    $ hostname -I

(>/>>)
===
This command (>>) will put the information on the file and append.The (>) command will override the file
    $ touch myfile.txt
    $ echo "this is my text" >> myfile.txt
    $ echo "this is my text" > myfile.txt
    $ nmap -F 10.10.10.10 > scan.txt

tree
===
    $ tree
    $ tree -a
    $ tree -d
    $ tree -l
    $ tree -f
    $ tree -x
    $ tree -L 1
    $ tree -L 2
    $ tree -L 3
    $ tree -R
    $ tree -P

&
===
To open application. Open a new process but can still use terminal
    $ code . &
    $ subl . &

which
===
    $ which code