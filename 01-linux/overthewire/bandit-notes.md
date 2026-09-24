Level 0 → 1: cat readme in home directory
6y2kwnwK6grgvwvpvLaa2T1cpFEKOhNR
Level 1 → 2: cat ./- in bandit1 directory
PK8fYLZg2hnHSz83plBL1iEPKdD3QToB
Level 2 → 3: cat ./--spaces in this filename-- in bandit2 directory
7ZZ2LFrykP2zEyvBl4m3clcL7tGYJPME
Level 3 →43 :cd inher tcat ...Hiding-From-You  in bandi31 director
xzTXq1rDJQVVAzdv5cHq1TQytTWufAMq
Level 4 → 5:cd inhere cat ./-file07
6C7h9GD8M6ai5nr7wo1RonrzFjj9yIrG
Level 5 → 6 cd inhere find -size 1033c
pXa26xhMWaC2SvDotA4r9EgZkulOeSBW
Level 6 →  7:find / -user "bandit7" -group "bandit6" -size 33c  cat /var/lib/dpkg/info/bandit7.password
Bmnnvf82KzQlfxgAI2d1zYbr1u9pr3E3
Level 7 →  : grep "millionth" data.txt
VR1ljMayciFxbnUokuQmJFw6QC9VKtub 
Level 8 →  9 sort data.txt | uniq -c
EjmOSvuAu7sGAHqHVcBDPirRe9T03kxl
Level 9 →  10 strings data.txt
B0s2khmbT9u0geKuOoVGW3JZKhndE3BG
Level 10 →  11 cat data.txt | base64 --decode
pYfOY6HwUsDj5rL9UvyhU7MCmv8vN5Ro
Level 11 →  12 cat data.txt | tr 'a-zA-Z' 'n-za-mN-ZA-M'   or    cat data.txt | tr 'a-z' 'n-za-m' | tr 'A-Z' 'N-ZA-M'
GROozWPO8QyN0mGrjUkID0WCYkZiQxrN
Level 12 →  13 bunch of decompressing and extracting 
qQYQiHOBPR8zR61qxYqX45quvihF2uzk
Level 13 →  14:had to scp key to local machine first, chmod 600, and connect via public hostname:2220 from local, not by chaining from inside bandit13 (localhost login blocked)
aaWecNkG4FhxJQxz07uiwzVP6bJiYS65
Level 14 →  15 nc bandit14@localhost 30000
pbLYuZtTg4MgaqfJx8jbA9gKKGqM68A7
Level 15 → 16:openssl s_client -connect localhost:30001
kS0Hf0u5HiXFwKMKFqXvPdOTNGGa0X8V
Level 16 → 17 ssh -i lvl17k.private bandit17@bandit.labs.overthewire.org -p 2220
Level 17 → 18:diff passwords.old passwords.new
OQxXZjELndr90zuhOTDYBEomI0SZITXI
Level 18 → 19 ssh bandit18@bandit.labs.overthewire.org -p 2220 "cat readme"
KpsOfPkcP7i1FlIExk2QEjyt6dw8dxZI
Level 19 → 20 /home/bandit19/bandit20-do cat /etc/bandit_pass/bandit20
4pIjcunZ0fK2vmp3IwfG8Vf7VhxD6pOA
Level 20 → 21nc -lvp 12345   in another terminal, ssh into 20 again and /home/bandit20/suconnect port , back to first terminal and input password for 20
bW9kBv5WC3P4yoDyf12LSdGuNz5ka6hY
Level 21 → 22:cd etc/cron.d  cat cronjob_bandit22  cat /usr/bin/cronjob_bandit22.sh   cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
RYVux2rHEm9tiXHmLFzuR7Vhx6AZQMEz
Level 22 → 23 cat /tmp/8ca319486bfbbc3663ea0fbe81326349 which you the has from echo I am user bandit23 | md5sum | cut -d ' ' -f 1
gKXDTAXnIz3OBxiPjRZ2uqutUlPZrBsw
Level 23 → 24:make a script in the foo directory that puts the password to level 24 in a txt file in /tmp.
hVQMk3lJNsmQ7VF3ubyrNNBom7BOgVXv
Level 24 → 25 In /tmp directory, make a txt file of all the combinations for the pin, make a script file and make sure it has the execute permissions.
SoHfqMOEqIX2IYKVciZxvgpR9a2Djx4P
Level 25 →26:ssh using the key then v → :set shell=/bin/bash → :shell
jHdv2ELQhT22BkprMNDjybZDAkw1zeBJ
Level 26 →27:./bandit27-do cat /etc/bandit_pass/bandit27
STJLJBRRphMxKB392CT4iOr5CbzPU9ER
Level 27 →28 git clone ssh://bandit27-git@bandit.labs.overthewire.org:2220/home/bandit27-git/repo 
y8Yd2ssKcpHpud7UvOSOxwamRMzIGIeQ
Level 28 →29:git show
Em7eGtqaMySwNFjCpwzzHhLhospOcdt0
Level 29 →30:git log --oneline --graph --all      git show  key was in a different branch
jq9Dfg2rXsfYsWMgFuKlXhphjdH7USgX
Level 30 →31 git show secret
82NkymblpGBYmIXG6ZQ8YldBYstHpfUf
Level 31 →32: create and push key.txt file. 
pWuj5jBQ6IgV0NXwiH6g1pXRF8S1YvbT
Level 32 →33:$0 then cat the password for level 33
u4P2CyPOwPGLe94RdD9Uo2FxFwvnFswM
Level 33 ->34: There isnt anything for this level yet :) <3

COMMANDS AND CONCEPTS
find - bash command used to find a files and directories
grep - bash command used to filter through a file for certain text. it returns the lines that has a keyword/phrase you ask for
xargs - bash command that takes the output of one command and passes it as arguments to another command.
nc - way to communicate from one host/ip/port to another host/ip/port without encryption
openssl - same as nc but with encryption used on the communication medium
ssh -i - opening a secure way to connect to a remote server using a private key. thats what the -i is for.
cron - automated tasks on a computer that get triggered at a predefined time
permissions- 4=read 2=right 1=execute. a file has three kinds of users that can engage with it, owner, group, and everyone else. when you run ls -l on a file you get something like -rwxr-xr--. owner=rwx
group=r-x everyone else= r--
