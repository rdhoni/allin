# allin


## Live Editor Home Termux

step first install termux-service 
````
 $ pkg install busybox termux-services
````
second step to running FTP
````
 $ source $PREFIX/etc/profile.d/start-services.sh
 $ sv-enable ftpd
 $ sv up ftpd
````
now open [Acode apk](https://play.google.com/store/apps/details?id=com.foxdebug.acodefree)
````
 /// add new FTP
 name            : Termux
 username        : 
 password        :
 host            : 127.0.0.1
 scurity type    : ftp
 connection mode : active
 port            : 8021

````
if after running ftp connect close, you repeat this step ` $ sv up ftpd `

## brings up a lot of buttons

for the up, down, right, left arrows. and others
````
echo "extra-keys = [ \ ['ESC','|','/','HOME','UP','END','PGUP','DEL'], \ ['TAB','CTRL','ALT','LEFT','DOWN','RIGHT','PGDN','BKSP'] \ ]" > /data/data/com.termux/files/home/.termux/termux.properties
````

## Oh-My-Zsh Theme

````
 $ sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
````

## Powerlevel10k Theme

````
 /// fist step 
 $ pkg install nano
 
 $ git clone --depth=1 https://gitee.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k
 
 $ nano ~/.zshrc

 /// change zsh theme name with

 ZSH_THEME="powerlevel10k/powerlevel10k"

````

## Install Composer

````
 /// install php
 $ pkg install php

 /// install composer
 $ curl -sS https://getcomposer.org/installer | php -- --install-dir=/data/data/com.termux/files/usr/bin --filename=composer
 
 /// check versi composer
 $ composer -V

````



