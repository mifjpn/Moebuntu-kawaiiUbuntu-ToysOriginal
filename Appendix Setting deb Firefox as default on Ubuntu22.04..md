# AppendixSetting deb Firefox as default on Ubuntu22.04

## 1.Uninstall snap firefox

    $ snap remove --purge firefox
    $ sudo apt remove --autoremove firefox

## 2.Add firefox ppa

    $ sudo add-apt-repository ppa:mozillateam/ppa

## 3.Write while creating a file (details later)

    $ sudo gedit /etc/apt/preferences.d/99mozillateamppa

 *content

    Package: firefox*
    Pin: release o=LP-PPA-mozillateam
    Pin-Priority: 1001
    Package: firefox*
    Pin: release o=Ubuntu
    Pin-Priority: -1

## 4.Check Candidates

    $ apt-cache policy firefox

## 5.install firefox

    $ sudo apt install firefox
