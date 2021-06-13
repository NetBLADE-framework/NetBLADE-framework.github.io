---
layout: single
title:  "Things to do after installing Fedora 28"
search: true
categories: 
  - Linux
  - Fedora
last_modified_at: 2018-09-27T08:05:34-05:00
header:
  teaser: /assets/images/blog/things-to-do-after-installing-fedora-28.jpeg
---

![Fedora 28](/assets/images/blog/things-to-do-after-installing-fedora-28.jpeg)

Fedora has been my favourite from the day I started using Fedora. As Fedora was sponsored by Red Hat, I had to make sure I gave it a try. I started my linux life using Ubuntu. Switching from Ubuntu to Fedora was not a easy task. I found first few days of using Fedora a bit hard. So, after gaining some experience using Fedora, gave me an idea to write a blog about the initial steps to be performed by a newbie Fedora user or a user who has just installed Fedora. When I was planning to write the blog, came the release of Fedora 28.

These are the steps I followed after installing Fedora 28.

First, we will switch to superuser.

```yaml
$ sudo su
```
There are few rpm packages to download. So,

```yaml
$ cd Downloads 
$ mkdir post-fedora-install
$ cd post-fedora-install
```
Now, lets update the OS. If you are new to Fedora, the fedora's update function will automatically update the repo list and will install the latest packages to the system.

```yaml
$ dnf -y update
```

Lets start the SSH server. SSH will help to connect to your system remotely from another system in the same network.

```yaml
$ systemctl start sshd 
$ systemctl enable sshd
```

Lets install RPM fusion repository into the system. The fusion repository will help to install all free and non free 3rd party applications.

```yaml
$ rpm -ivh https://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-28.noarch.rpm 
$ rpm -ivh https://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-28.noarch.rpm 
$ dnf -y update
```

If you are using GNOME, installing the GNOME tweak tool will help you customize the desktop environment.

```yaml
$ dnf -y install gnome-tweak-tool
```

Lets install some media codecs to view all media files.

```yaml
$ dnf -y install gstreamer-plugins-base gstreamer1-plugins-base gstreamer-plugins-bad gstreamer-plugins-ugly gstreamer1-plugins-ugly gstreamer-plugins-good-extras gstreamer1-plugins-good-extras gstreamer1-plugins-bad-freeworld ffmpeg gstreamer-ffmpeg

```

Lets install VLC.

```yaml
$ dnf -y install vlc
```

Lets install Stacer. Stacer is an application to view system information and monitor all the system resources. As stacer is an open-source application, we must first download it from github.

```yaml
$ wget https://github.com/oguzhaninan/Stacer/releases/download/v1.0.8/stacer-1.0.8_x64.rpm
```

Now lets install the downloaded rpm file.

```yaml
$ dnf -y install stacer-1.0.8_x64.rpm
```

Lets install a torrent client. qbittorrent works just fine for Fedora 28.

```yaml
$ dnf -y install qbittorrent
```

If you like to download videos from youtube. Then worry not, here comes youtube-dl. The youtube-dl is a commandline function to download youtube videos.

```yaml
$ dnf -y install youtube-dl
```

Consider Fedora is your daily driver workstation. You might need to take screenshots or custom screenshots. Shutter snipping tools is the best alternative for Fedora.

```yaml
$ dnf -y install shutter
```

Lets install unzip for uncompressing files.

```yaml
$ dnf -y install unzip
```

Lets install java plugins for web browsers.

```yaml
$ dnf -y install icedtea-web java-openjdk
```

Lets install java JDK.

```yaml
$ yum install -y java-1.8.0-openjdk-devel
```

If you develop programs in C, you will need development tools.

```yaml
$ dnf -y group install 'Development Tools'
```

Everyone has an IDE preference, I like to use Sublime. First we must import the sublime repo.

```yaml
$ rpm -v --import https://download.sublimetext.com/sublimehq-rpm-pub.gpg
```

We then add the repo using config manager.

```yaml
$ dnf config-manager --add-repo https://download.sublimetext.com/rpm/stable/x86_64/sublime-text.repo
```

Now, we are ready to install Sublime IDE.

```yaml
$ dnf -y install sublime-text
```

If you are a gamer, you must have steam. For installing steam, we need to add the steam repo into the system.

```yaml
$ dnf -y config-manager --add-repo=http://negativo17.org/repos/fedora-steam.repo
```

Now, lets install the update the repo list.

```yaml
$ dnf -y update
```

Lets install Steam.

```yaml
$ dnf -y install steam
```

This is it folks. These steps helped me make my Fedora be used as a daily driver.