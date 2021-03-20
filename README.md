# macbuntu
my experience with ubuntu unity 20.10 on a 2012 macbook pro - extra stuff i installed for optimal usage.


so installing, i used the Ubuntu Unity Project (https://ubuntuunity.org) for my OS. I hate gnome with a passion, like everything uses it. 
it all went fairly smoothly with no issue. I'm dual booting using rEFInd and have experienced very little issues with my install.

First thing I did upon install was update/upgrade
> sudo apt-get update
> sudo apt-get upgrade

after updating/upgrading, in order to satisfy the needs of rEFInd, i uninstalled grub and put a hold on it so it wouldn't come with further updates/upgrades.
> sudo apt remove grub2
> sudo apt-mark hold grub2*

now for fan and optimizations...

i credit (https://ohthehugemanatee.org/blog/2016/10/15/perfect-linux-mint-macbook-pro-9-2/) for some ideas.

fan support is as easy as installing
> sudo apt-get install mbpfan

next is powertop
> sudo apt install powertop

once installed simply run
> sudo powertop --html=powertop.html

then you go to your usr directory and open it and go to the tweaks page. from there you can see what needs to change for optimal usage
to apply you need to go into su. I couldn't get sudo to work, and su refused so I used sudo -i and got in w/o password just fine
