### Notes and solutions
Important! for the rest of the activities were gonna be using the SSH. SSH allows you to connect to a device or any IOT device across the internet. the host OS will not matter on this activity, however upon logging to SSH, everybody will be using the server OS.

connecting to the SSH server is pretty easy.
```cli
ssh bandit0@bandit.labs.overthewire.org -p 2220
```
this example calls the SSH command followed by the user which were about to login `bandit0` then followed by @ `bandit.labs.overthewire.org` as the host. since the host requires us to connect to the port 2220 we will specify the port number by adding the option `-p` this way it will not connect automatically to port 22.

the solution command for this section is;
```cli
cat readme
```
the output will be the password to the next level
```cli
cat < -
```
`<` negates the special character in order to treat it as a ascii rather than a operator.
```cli
cat "spaces in this filename"
```
or
```cli
cat spaces\ in\ this\ filename
```
this is a string formatting.
```cli
cd inhere/ && cat .hidden
```
we opened the folder `inhere` and read the file `.hidden` and file with a 'dot' in front of the is a hidden file. the only way we could reveal them is by entering this command;
```cli
ls -al
```

```cli
cd inhere/ && find . -type f -exec cat {} \;
```
in this example we used the `find` command to locate every file as `-f` and executed them `-exec` with `cat`
```cli
locations=$(cd inhere/ && find . -size 1033c ! -executable) && cd inhere/ && cat strings $locations
```
this command for bandit6 allows you to look for the location of the badit7.password file a bit easier
```cli
find / -user bandit7 -group bandit6 -size 33c | grep -P "bandit7"
```
the bandit7 will glow red allows you to find it a bit easy. next you have to open the file located in that folder
```cli
cat /var/lib/dpkg/info/bandit7.password
```
this next example allows you to use the grep and its true potential
```cli
grep -P "millionth" data.txt
```
in this example we looked for the pattern `-P` that says "millionth"
```cli
cat data.txt | sort | uniq -u
```
read data.txt file and `sort` with a `uniq` unique result `-u`
```cli
strings data.txt | grep =
```
in the example bellow we open the `data.txt` and decoded it directly using the `base64` function with the `-d` options for decode
```cli
cat data.txt | base64 -d
```

```cli
cat data.txt | tr a-zA-Z n-za-mN-ZA-M
```
opened the data.txt file and translated the string result.