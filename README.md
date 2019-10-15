# IEEE-2030_5-Client
Portland State University Generic SEP 2.0 Client for DERAS

## Resources

* Github: https://github.com/emesene/emesene/wiki/GitHowTo#what-should-i-do-if-im-in-a-bad-situation
* CPP: https://en.cppreference.com/w/
* Style Guide: https://google.github.io/styleguide/cppguide.html
* Design Patterns: https://refactoring.guru/design-patterns


## Dependencies
All dependencies should be located in your "/home/src" directory. If there are updates to one of the dependencies ensure it is modifed in this location.

### Linux
``` console
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install tmux git build-essential gcc g++ openssl
cd /home
mkdir src dev logs
```

### Default Network
For DCS that will be connecting to PSU's network you will need to setup a default network connection using the registered device network.

https://www.pdx.edu/oit/internet-device-registration

Once you have registred the device, modify the "wpa_supplicant.conf" file to elevate the priority of the registered device network to ensure it is the first network connected to. 

``` console
sudo nano /etc/wpa_supplicant/wpa_supplicant.conf
```

### Boost
Download and extract the boost libraries into the "/home/src" directory.

https://www.boost.org/users/history/version_1_71_0.html

### IEEE 2030.5
Download and extract the available IEEE 2030.5 downloads that provide example xml models.

https://standards.ieee.org/standard/2030_5-2018.html
