![Banner Image](https://sinisterspatula.github.io/RetroflagGpiGuides/images/GuidesBanner.png)

[Back to Index](https://sinisterspatula.github.io/RetroflagGpiGuides/)


# Stuttering Splash Video guide

Source: [sudomod.com](https://sudomod.com/forum/viewtopic.php?f=44&t=5953&sid=a445fc61f5d69f18b005c1318d303f41&start=10&fbclid=IwAR3gbe9t2zlxNYArphrEwmjOXJnHU55lpKSNYPAUhlmON59dnwsXvtqykis#p61371)

Follow this short guide to fix Splash (boot-up) video stuttering/slowness on the Gpi/Piezero.

* [Connect to your GPi using SSH.](https://www.youtube.com/watch?v=aEJoQZBSlSs)
* Edit the configuration file: `sudo nano /opt/retropie/supplementary/splashscreen/asplashscreen.sh`
  * Edit Line 35 which looks like:
`omxplayer -o both -b --layer 10000 "$line"`

* Change it to:
`omxplayer -b --layer 10000 "$line"`

* And add this line also (underneath the omxplayer line you just changed):
`audio_pwm_mode=2`
   > Mode=2 is recommended for Pi zero, you can also try Mode=0

* [Ctrl+O] (to save) [Enter] and [Ctrl+X] (to exit)


## Support Thread
[Go here for help](https://www.facebook.com/groups/401660300458844/)

[Back to Index](https://sinisterspatula.github.io/RetroflagGpiGuides/)

###### Head back to our [Facebook Group](https://www.facebook.com/groups/401660300458844/)

