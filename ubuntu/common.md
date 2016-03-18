
## Install Common Tools
``sudo apt-get update && sudo apt-get install -qy vim tree history htop openjdk-7-jdk ``

---
## Install oh-my-zsh
zsh command line looks more obvious


``sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"``  

`` sudo apt-get install zsh  `` 

`` sudo chsh -s `which zsh` username ``

reboot or relogin 

---
## Update Java

`` curl -L -k -H "Cookie: oraclelicense=accept-securebackup-cookie" -o ojvm.tar.gz http://download.oracle.com/otn-pub/java/jdk/8u71-b15/server-jre-8u71-linux-x64.tar.gz `` 

`` sudo mkdir -p /usr/lib/java ``

`` sudo tar -xzf ojvm.tar.gz -C /usr/lib/java/ ``
     
`` echo JAVA_HOME=/usr/lib/java/jdk1.8.0_71 >> ~/.zshrc ``

`` echo PATH=$PATH:$JAVA_HOME/bin >> ~/.zshrc ``

`` sudo update-alternatives install /usr/bin/java java /usr/lib/java/jdk1.8.0_71/bin/java 1 ``

`` sudo update-alternatives --config java ``

select java want update



