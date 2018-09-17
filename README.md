# Reference Insanity Check

### Just run it and enjoy.

#### Table of Contents
1. [Description](#description)
2. [Setup](#setup)
    * [Setup requirements](#setup-requirements)
    * [Usage](#usage)
3. [Future plans for the Project Development](#future)
4. [Bugtrack](#buqtrack)
5. [Annotations](#annotations)
6. [Copyrights](#theducks)

### Description

this script was a wet dream of the lead developer in some random project.
you need to run it few minutes after the deployment (not release, for duck sake).

### Setup

##### Setup requirements

you need to have brainz and ssh-kinda-tool and no zombies around.

##### Usage

start hacking with:
```
upa.8vm1337# 
vm1337 # 
vm1337 # 
vm1337 # 
vm1337 # yum install screen sshpass
vm1337 # git clone git@github.com:nicon89/ref-insanity-check.git
vm1337 # cd ref-insanity-check
vm1337 # curl wiki/hosts | awk {'print $1'} >> hosts/devjboss (if you know what I mean)
# if your servers don't include name in hostname you can use this:
# xyz1337 PNWEB
# xyz420 PN2BOAPP
# xyz2137 PN2GAME
# and so on...
vm1337 # 
# configure services you want to check in conf/*-service-list
# configure $USER ($2) password in conf/.passwd (default already set)
# configure disabled-services.example and move to disabled-services
vm1337 # ./insanity-check qajboss root service
[...stuff on screen going on...]
# configure containers in conf/*-container-list
vm1337 # ./insanity-check devjboss root marker
[...stuff on a screen going on...]
# you can also use sudo mode, but there are some issues with this when run from jenkins*
vm1337 # ./insanity-check prodjboss nicon service sudo
vm1337 # d
vm1337 # logout
vm1337 $ logout
d
```

#### Jenkins
###### you can also do some jenkins jiu jitsu with Jenkins DSL Groovy, if you need help with this just let me know.

### Future plans for the Project Development

##### random project lead developer had a wet dream about havivng:
* reports
  * html
  * ~~jenkins (colors, fails, final report)~~
* jboss checks
  * ~~check for deployed, deploying, failed ear files (the wet)~~
  * check list of markers to see if they are deployed

#### Buqtrack
 * 000001 - sudo issue in jenkins, I don't really have time to fix this one, you're more than welcome to fix it by yourself if you care, kthxbye. PS. Proposed fix: /etc/sudoers controled by Puppet/Ansible/Whatever.


##### Annotations

```
i've wanted to thank very much my mentor, my sensei, mr. nj
huge thanks to my dear pain-in-the-ass friend and an assistant, the b guy, mr pee.
i've wanted to thanks for the music, for giving it to me.
this manual was done with a help of [editor.md](https://pandao.github.io/editor.md/en.html)
```

##### Copyrights

###### copyright 2018 nicon@bash.org.pl
###### each change/fix needs to have separated branch and (may) be merged after review.
* create new branch
* code & qa
* rise merge request and assign to the owner.
