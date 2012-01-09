!SLIDE commandline smaller
# Installing on Ubuntu #

## jenkins-ci.org has binaries available for Ubuntu ##

    $ wget -q -O - http://pkg.jenkins-ci.org/debian/jenkins-ci.org.key | sudo apt-key add -
Adds jenkins-ci.org's apt key to your system's trusted keys

    $ sudo sh -c 'echo deb http://pkg.jenkins-ci.org/debian binary/ > \
    /etc/apt/sources.list.d/jenkins.list'
Adds jenkins-ci.org's repository to your apt's sources list

    $ sudo apt-get update
    $ sudo apt-get install jenkins
Installs Jenkins, creating a jenkins user, and adds a init script at
`/etc/init.d/jenkins`

!SLIDE
# Plugins #

There are plugins for both git and GitHub. We'll use both in this
presentation
