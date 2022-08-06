
# Build Host Packages

$ sudo apt-get install gawk wget git-core diffstat unzip texinfo gcc-multilib \
     build-essential chrpath socat cpio python python3 python3-pip python3-pexpect \
     xz-utils debianutils iputils-ping python3-git python3-jinja2 libegl1-mesa libsdl1.2-dev \
     pylint3 xterm

# Setting up the Repo utility

$ mkdir bin (this step may not be needed if the bin folder already exists)

$ curl https://storage.googleapis.com/git-repo-downloads/repo > bin/repo

$ chmod a+x bin/repo

$ export PATH=$(realpath ./bin/):$PATH

$ git config --global user.name "Your Name"

$ git config --global user.email "Your Email"

$ git config --list



$ mkdir est-work

$ cd est-work

$ repo init -u https://github.com/EmbeddedTasks19/est-manifest -b zeus -m rpi3-qt.xml

$ repo sync

 
