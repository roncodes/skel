# Composer Package Creator & Skeleton
### A Bash script to create skeleton based composer packages

The script will basically ask for some information (destination, vendor, package, vcs username...) clone a skeleton repositoy, replaces everything related to the package with the information the user provides and push it to your VCS (Github, Bitbucket...).

#### Running it directly from Github

```
bash <(curl -s https://raw.githubusercontent.com/antonioribeiro/skeleton/master/createPackage.sh)
```

#### Installing on your system

```
wget http://sitehere.com/install.sh -v -O /usr/install.sh
```

#### Skeletons

During creation of a package the script may ask for a skeleton to install, the currently available are:

* League
* Laravel 5
* Laravel 4
* Your own skeleton

#### Skeleton Base

All skeletons on this repository are currently using as a base [ThePhpLeague/Skeleton](https://github.com/thephpleague/skeleton), all packages are based on League's and every commit should be merged to ours. The differences between League's and this respository are:
  
* Replacement strings (:package_name, :vendor_namem, etc.)
* Framework specific repositories, for instance Laravel Service Providers, included in Laravel versions.
