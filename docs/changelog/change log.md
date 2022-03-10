Sudobox Change Log - v0.1.0 - 10.03.2022

Bug Fixes

- **Both the ''sb" and ''sudobox" commands will now be recognised.**
- ****Domain install question now specifies as top-level domain (TLD).****

Improvements

- **The installation script has been updated with error catching.** 

- **CLI installation questions have been updated and have removed unnecessary questions** -
  
  Asking the user if they want to add a domain (removed).
  
  Asking the user for a CloudFlare API Token (removed).

- **Added the ability to skip domain lookup check.** This acted as a blocker. Traefik is now configured to generate the SSL certs over DNS validation using a .txt.

- **No longer requires user to enter Cloudflare Token.**  This will now use your global API key instead.

Features

- **Traefik is now protected with basic authentication if Authelia isn't installed.**
- **Apps by default won't map the host port to the container.**
- **The SudoBox API and admin dashboard have also been updated to accommodate these new changes.**

Known Issues

- MongoDB ( sb-database ) won't start up if CPU doesn't support AVX. This mostly effects older systems and VM's which aren't  passing through the host CPU. We are looking into the possibility of downgrading to MongoDB 4.XX

Special Thanks

We would like to say a special thanks to all those users that helped with testing. Especially those that came into member voice chat, we hope to have more of those in the future.
