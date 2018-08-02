# ref-insanity-check

## Just run it and enjoy.

#### Table of Contents
1. [Description](#description)
2. [Setup](#setup)
    * [Setup requirements](#setup-requirements)
    * [Usage](#usage)
3. [Future plans for the Project Development](#future)
4. [Annotations](#annotations)
5. [Credits](#credits)

## Description

this script is the dream of the lead developer in r*t project.
you need to run it few minutes after the deployment (not release, for duck stake).

## Setup

### Setup requirements

you need to have brainsi, ssh-kinda-tool and no zombies around.

### Usage

start hacking with:
```
toor
vm1337 # 
vm1337 # yum install screen sshpass
vm1337 # git clone https://github.com/nicon89/ref-insanity-check
vm1337 # cd instanity-check
vm1337 # curl wiki/sites/ref#prod | awk {'print $1'} >> hosts/dev-hosts-list
vm1337 # 
# configure services you want to check in conf/*-service-list
# configure $USER ($2) password in conf/.passwd (default already set)
vm1337 # ./insanity-service-check dev-hosts-list root
vm1337 # [...stuff on a screen going on...]
vm1337 # d
vm1337 # logout
vm1337 $ logout
d
```

### Future plans for the Project Development

r*t lead developer had a dream about havivng:
* reports
  * html
  * jenkins (colors, fails, final report)
* app checks
  * check for deployed, deploying, failed *appexec files (the wet)
  * check disk space on the portal servers (then ask a user if he/she wants to run rm -Rfv /* on server depending on current disk space usage. Options: y/n: 'y' will work for 'no', 'n', will work for 'yes')

### Annotations

```
i've wanted to thank very much my mentor, my sensei, mr. eN Jay aka main vip.
i also wanted to thank my dear friend, an assistant and the bj project lead, mr pee jay.
i've wanted also to thank you for the music, for giving it to me.
```

### Credits
#theducks

copyright 2018 nicon89 aka The Writer.
any changes are rised by jira requrest, or git issues and need to follow git workflow prcess
each change/fix needs to have separated branch and be merged after review.
* create new branch
* code & qa
* raise merge request and assign to nicon89 or nicon89.
