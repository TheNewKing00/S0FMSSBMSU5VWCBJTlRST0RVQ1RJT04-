# Digital Forensics Tools, PW Cracking And Wordlist

### **Linux Apps**

Using applications and programs in Linux is Fairly Easy. Think of them as you are filling up a UI form with some check boxes and toggle options. Kali-Linux Also has a packages manager from the cli. this allows you to download apps directly from its source with insanely fast and easy installation process.

**Using an application or Tool in Linux**
Here is an example.
Say you have a form that Looks like this.

- - -

#### Register

**FIrst Name**

```

```

**Last Name**

```

```

**Email**

```

```

**Password**

```

```

`SUBMIT`                                                             `CLEAR`

- - -

On Linux cli it should look a lot like this
<br>
```
register -Firstname "My First name" -Lastname "My Lastname" -Email "My email" -password "my Password"
```

**resgister** being the name of the application and its sub sequent feilds.
There might be some toggle options such as <i>**remember info**</i>can be selected on the ui. how ever in the command line, by default it will be set to none or false. to turn it on you just have to add the option like say for example `-R`option on the end of the line.

You can find out any options and feilds by typing `man` before any of the application, software or  tools. additionally you can display a very short info about the appication, software or tools by adding `-h` or `--help`  after the it.

Like for example:

```
register -h
```

or

```
register --help
```
<br>
##### **Installing Applications or tools**

Installing comes easy. In kali, has a package manager on its own called `apt`.
for example I wanted to install a tool called `cyberchef`
first I will try to search the tool by typing.

```
apt search cyberchef
```

if you found the tool you need you can proceed the installation by

```
apt install cyberchef -y
```

in this case the `-y`option allows the installation process to go automatically without any prompts.

#### Forensics

Forensics or digital forensics in general deals in findinding important data invisible to the surface level UI. for this you need to dig deeper into the system's internal data such as exif or medata data, log memory, registry and bin files.

there are a handful of tools you can use for this. heres a list of forensics tools.

| **Tool Name** | **Description** |
| --------- | :---------- |
| Aircrack-Ng | Crack 802.11 WEP and WPA-PSK keys |
| Audacity | Analyze sound files (mp3, m4a, whatever) |
| Creddump | Dump windows credentials |
| Exif Tool | Read, write and edit file metadata |
| Extundelete | Used for recovering lost data from mountable images |
| Fsck.ext4 | Used to fix corrupt filesystems |

More info about this topic here:[https://int0x33.medium.com/day-18-essential-ctf-tools-1f9af1552214](https://int0x33.medium.com/day-18-essential-ctf-tools-1f9af1552214)

> Note : You can read more about the tool on its documentation. use chatGPT or Google for aditional help  or usecases for the tool.

### Password Cracking Tools

password craking tools are on fo the most popular softwares in the market. able to scale WIFI's 'Unmaintained' websites, poor passwords on laptops, mobile devices or even IOT devices, such as network switch, routers and many more.

One tool I've been familliar with is. [BurpSuite](https://github.com/apsdehal/awesome-ctf/tree/master) this seemingly harmless tool can intercept http request and modify its data. bombard websites with bruteforce attacks from a password list. and it can reveal unlinked url on a website included ones that are intentionally hidden from the casual user. this tool comes pre installed in kali.

> Note : that this tool however unlike tools on this category is more easy to use on its UI

here are some password craking tools

| **Tool Name** | **Description** |
| :-------- | :---------- |
| Hashcat | Password Cracker |
| John The Jumbo | Community enhanced version of John the Ripper |
| John The Ripper | Password Cracker |
| Nozzlr | Nozzlr is a bruteforce framework, trully modular and script-friendly. |
| Ophcrack | Windows password cracker based on rainbow tables. |
| Patator | Patator is a multi-purpose brute-forcer, with a modular design. |