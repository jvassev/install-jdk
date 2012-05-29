Steps to install Oracle JDK on Ubuntu:
===========

Download the tar.gz from here http://www.oracle.com/technetwork/java/javase/downloads/index.html

Download the script

    wget https://raw.github.com/jvassev/install-jdk/master/install-jdk
    

Run the script as root:

    $ sudo bash install-jdk ~/Downloads/jdk-7u4-linux-x64.tar.gz
    

The script prompts you for what to do next:

    prefix:/usr/lib/jvm
    prio:168
    JVM: /usr/lib/jvm/jdk1.7.0_04/
    alias: jdk1.7.0_04
    
    +++ Currently available javas:
    java-6-sun 63 /usr/lib/jvm/java-6-sun
    java-7-oracle 100 /usr/lib/jvm/java-7-oracle
    jdk1.7.0_04 168 /usr/lib/jvm/jdk1.7.0_04
    
    +++ Select the newly installed java using:
    sudo update-java-alternatives -s jdk1.7.0_04

So let's run
    
    sudo update-java-alternatives -s jdk1.7.0_04


Verify the new version is installed:

    $ java version "1.7.0_04"
    Java(TM) SE Runtime Environment (build 1.7.0_04-b20)
    Java HotSpot(TM) 64-Bit Server VM (build 23.0-b21, mixed mode)
    
