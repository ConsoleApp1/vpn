# ConsoleApplication1 - VPN information and guides

Repository with information about VPN and guides for setting up a personal VPN service.

![Preview of VPN][docs._assets.preview_image]

The docs is published under the GNU v3.0 License, the license is available [here][root.license].

The tutorials use the [Shadowsocks][external.shadowsocks] protocol and the [Outline][external.outline] server, [manager][external.outline.manager], and [client][external.outline.client].

## Suported systems:

The latest version of web clients is available for:

* Outline Server: GNU/Linux platform's modern operating systems and their various distributions like:
  * Linux Ubuntu;
  * Linux Debian;
  * Kali Linux;
  * Elementary OS;
  * Linux Mint;
  * MX Linux;
  * Feodora;
* Outline Manager: 
  * Windows;
  * Linux;
  * MacOS;
* Outline Client: 
  * Windows;
  * Linux;
  * MacOS;
  * Android;
  * iOS;
  * Chrome Browser (extension).

## The Complete Guide to Creating a Personal VPN Service.

## Renting a VPS (Virtual Private Server) using [pq.hosting][external.hosting.pq.hpsting] as an example.
1. Go to [pq.hosting][external.hosting.pq.hosting] and sign-up the site: 
   ![Preview of pq.hosting home page][docs._assets.external-pq-hosting-1] 
2. Fill the registration form and and click "Register": ![Preview of pq.hosting register page][docs._assets.external-pq-hosting-2]
3. Wait for registration to complete: ![Preview of pq.hosting registration waiting page][docs._assets.external-pq-hosting-3]
4. During the registration process, your Email will receive a confirmation letter: ![Preview of registration confirmation email message][docs._assets.external-pq-hosting-4-5]
5. You can immediately go to your personal account using the link from the letter;
6. Go to the private virtual servers page: ![Preview of pq.hosting page][docs._assets.external-pq-hosting-6]
7. Click on the "Order" button: ![Preview of bill.pq.hosting page orders button][docs._assets.external-pq-hosting-7]
8. Choose your preferred VPS location country (recommended country located in geographic proximity): ![Preview of bill.pq.hosting tariff plans page][docs._assets.external-pq-hosting-8-9]
9. Choose your preferred VPS configuration (cheapest recommended) and click "Order" button;
10. Select operating system (Ubuntu-20.04 is recommended): ![Preview of bill.pq.hosting service parameters page][docs._assets.external-pq-hosting-10-11]
11. Click the "Add to cart" button;
12. Click the "Pay" button: ![Preview of bill.pq.hosting cart page][docs._assets.external-pq-hosting-12]
13. Choose any convenient payment method. "YooMoney" for example (Available if you are from Russia. Also accepts russian roubles): ![Preview of bill.pq.hosting payment method selection page][docs._assets.external-pq-hosting-13]
14. Choose a payer or create new one: ![Preview of bill.pq.hosting payer selection page][docs._assets.external-pq-hosting-14-15]
15. Click on the "Next" button;
16. Check the payer's main information and change them if necessary: ![Preview of bill.pq.hosting payer information page][docs._assets.external-pq-hosting-16-18]
17. Check the payer's actual address and change them if necessary;
18. Click on the "Next" button;
19. Click on the "Pay" button: ![Preview of bill.pq.hosting payment confirmation page][docs._assets.external-pq-hosting-19]
20. Select the final payment method, if you have chosen to pay via YooMoney: ![Preview of yoomoney.ru payment final method selection page][docs._assets.external-pq-hosting-20-21]
21. Make a payment;
22. After payment, return to the hosting VPS list page. If the button does not work, you can do it manually: ![Preview of yoomoney.ru completed payment page][docs._assets.external-pq-hosting-22]
23. In the VPS list page, you will see the VPS with the "Activation in progress" status. Payment can be processed up to 15 minutes. Until this moment, status of the VPS will be "ordered" and this is normal. Activation can also take up to 15 minutes: ![Preview of bill.pq.hosting vps list page: vps activation in progress][docs._assets.external-pq-hosting-23]
24. When the VPS is activated, its status will be changed to "Active". If the status hasn't changed in 15 minutes, try refreshing the page: ![Preview of bill.pq.hosting vps list page: vps active][docs._assets.external-pq-hosting-24]
25. Select VPS: ![Preview of bill.pq.hosting vps list page: instructions][docs._assets.external-pq-hosting-25-26]
26. Click on the "Instructions" button;
27. On the page that opens, you will find the IP address, login (root) and password from your VPS: ![Preview of bill.pq.hosting vps instructions page][docs._assets.external-pq-hosting-27]
28. In the VPS list page select VPS again: ![Preview of bill.pq.hosting vps list page: to panel][docs._assets.external-pq-hosting-28-29]
29. Click on the "To Panel" button to open a VPS control panel;
30. Click on the "Computer Icon" (VNC) button to open a virtual terminal: ![Preview of bill.pq.hosting vps control panel page][docs._assets.external-pq-hosting-30]
31. Enter your VPS username (root by default) and password: ![Preview of bill.pq.hosting virtual terminal page: user credentials][docs._assets.external-pq-hosting-31]
32. Ensure you have successfully connected: ![Preview of bill.pq.hosting virtual terminal page: sucsessful login confirmation][docs._assets.external-pq-hosting-32]
33. You can work through a virtual terminal, but the clipboard (Ctrl+C, Ctrl+V) does not work in it.
34. For greater convenience and a working Clipboard, we recommend installing [Putty][external.putty].


## Installing [Putty][external.putty] and connecting to a remote server.
1. Go to [www.putty.org][external.putty] and follow the link "here": ![Preview of putty.org main page][docs._assets.external-putty-1]
2. Download the app installer for your OS. MSI x64 Installer is recommended for Windows: ![Preview of putty.org download page][docs._assets.external-putty-2]
3. Run the app installer. For a successful installation, you just need to click the "Next" button: 
   
   ![Preview of putty installer][docs._assets.external-putty-3]
4. After installation, run the Putty app. Enter in the field "Host Name (or IP address)" the IP address of your server: 
   
   ![Preview of putty app: save & load connection settings][docs._assets.external-putty-4-6]
5. Enter the name of the connection configuration in the field under "Saved Sessions" to use this configuration in the future;
6. Click on the "Save" button to save connection configuration;
7. Click on the "Load" button to load connection configuration: 
   
   ![Preview of putty app: open putty terminal][docs._assets.external-putty-7-8];
8. Click on the "Open" button to open terminal;
9. Click on the "Accept" button to add the host key to Putty:
    
    ![Preview of putty terminal: user credentials][docs._assets.external-putty-9];
10. Enter your VPS username (root by default) and password: 
    
    ![Preview of putty terminal: sucsessful login confirmation][docs._assets.external-putty-10-11]
11. Ensure you have successfully connected;
12. Now you can work through Putty terminal!

## Installing an Outline VPN Service on your server.
### Docker installation.
   1. Synchronize the package index files from their sources:
      ```shell
      sudo apt update
      ```
   2. Install the newest versions of all packages currently installed on the system from the sources:
      ```shell
      sudo apt upgrade
      ```
   3. Install package that allows the use of repositories accessed via the HTTP Secure protocol:
      ```shell
      sudo apt install apt-transport-https ca-certificates curl software-properties-common
      ```
   4. Add the GPG key for the Docker repository to the system:
      ```shell
      curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
      ```
   5. Add the Docker repository to the system:
      ```shell
      sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"
      ```
   6. Synchronize the package index files from their sources:
      ```shell
      sudo apt update
      ```
   7. Install Docker:
      ```shell
      sudo apt install docker-ce
      ```
### Outline Manager & VPN Service Installation.
   1. Go to [getoutline.org][external.outline];
   2. Click on the "GET OUTLINE" button: ![Preview of getoutline.org page][docs._assets.external-outline-manager-2]
   3. Click on the "GET OUTLINE MANAGER" button: ![Preview of getoutline.org get-started page: manager][docs._assets.external-outline-manager-3]
   4. Choose OS: ![Preview of getoutline.org get-started page: step 1][docs._assets.external-outline-manager-4-5]
   5. Click on the "DOWNLOAD THE OUTLINE MANAGER" button to download Outline Manager;
   6. After downloading, run Outline Manager. In the agreement, click OK;
   7. Click on the "Set up OUTLINE anywhere" panel: ![Preview of Outline Manager interface: mode selection][docs._assets.external-outline-manager-7]
   8. Copy the following command to clipboard: 
      ```shell
      sudo bash -c "$(wget -qO- https://raw.githubusercontent.com/Jigsaw-Code/outline-server/master/src/server_manager/install_scripts/install_server.sh)"
      ```
      ![Preview of Outline Manager interface: command][docs._assets.external-outline-manager-8]
   9.  Log in to the server and enter the copied command: ![Preview of Outline Manager interface: linux command][docs._assets.external-outline-manager-9]
   10. Copy the output green line to the clipboard: ![Preview of linux terminal][docs._assets.external-outline-manager-10]
   11. Paste the copied line into field 2 ![Preview of Outline Manager interface: command output][docs._assets.external-outline-manager-11-12]
   12. Click on the "DONE" button;
   13. Skip the tips;
   14. Click on the "Settings" button: ![Preview of Outline Manager interface: server control panel][docs._assets.external-outline-manager-14]
   15. Change the server name if you wish: ![Preview of Outline Manager interface: server settings panel][docs._assets.external-outline-manager-15]
   16. Return to VPN Server Connections Panel.
### Outline Client Installation.
   1. Go to [getoutline.org/get-started][external.outline.get-started];
   2. Click on the "GET OUTLINE CLIENT" button: ![Preview of getoutline.org get-started page: client][docs._assets.external-outline-client-2]
   3. Choose OS: ![Preview of getoutline.org get-started page: step 3][docs._assets.external-outline-client-3-4]
   4. Click on the "GET OUTLINE CLIENT" button to download Outline Client;
   5. After downloading, run Outline Client.
### Granting access to VPN.
   1. Open Outline Manager's Connections Panel of your VPN server;
   2. Click on the "Add new key" button: ![Preview of Outline Manager: add new key button][docs._assets.external-outline-keys-2]
   3. Enter a name for the key (preferably a name that will identify the device, user, or group of users): ![Preview of Outline Manager: new key][docs._assets.external-outline-keys-3-4]
   4. Click on the button with "Share icon";
   5. In the "Share access" window that opens, scroll down to "1. Copy your access key" and copy the access key: ![Preview of Outline Manager: access key][docs._assets.external-outline-keys-5-6]
   6. Click on the "DONE" button;
   7. Open Outline Client app;
   8. Click on the "Add server" button:

      ![Preview of Outline Client: add server][docs._assets.external-outline-keys-8]
   9.  Paste the previously copied access key into the input field: 

      ![Preview of Outline Client: paste access key][docs._assets.external-outline-keys-9-10]
   10. Click on the "ADD SERVER" button;
   11. Click on the "ROUND" or "CONNECT" button: 

      ![Preview of Outline Client: cennect to server][docs._assets.external-outline-keys-11]
   12. Ensure you have successfully connected: 

      ![Preview of Outline Client: successful connect confirmation][docs._assets.external-outline-keys-12]

   13. If you have several connections to different servers or with different keys, you can rename them in the settings ("three dots" button);
   14. Now you own a private VPS service!
### Outline Mobile Client Installation on Android via Play Store.
   1. Go to Google Play Store app, find the Outline app and install it: 
      
      ![Preview of Google Play Store][docs._assets.external-outline-client-mobile-1]
   2. Open the Outline app and click on the "Add Server" button: 
      
      ![Preview of Outline Client Mobile: add server][docs._assets.external-outline-client-mobile-2]
   3. Paste the previously copied access key into the input field and click on the "ADD SERVER" button:
      
      ![Preview of Outline Client Mobile: Access key][docs._assets.external-outline-client-mobile-3]
   4. Click on the "CONNECT" button: 
      
      ![Preview of Outline Client Mobile: connect to server][docs._assets.external-outline-client-mobile-4]
   5. In the pop-up window, click OK: 
      
      ![Preview of Outline Client Mobile: pop-up window][docs._assets.external-outline-client-mobile-5]
   6. Ensure you have successfully connected: 
      
      ![Preview of Outline Client Mobile: successful connect confirmation][docs._assets.external-outline-client-mobile-6]
### Fixing problems.
   - If in Windows 10 the Outline client does not connect to the server, then you need to disable Hyper V. To do this, open PowerShell as an administrator and enter:
     ```shell
     Disable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V-Hypervisor
     ```




<!-- LINKS -->


<!-- consoleapplication1 -->

[consoleapplication1]: https://consoleapplication1.com


<!-- root -->

[root.license]: LICENSE


<!-- docs -->

[docs.readme]: docs/README.md
[docs.ubuntu-build]: docs/roadmap/README.md
[docs.tasks]: docs/tasks/README.md



<!-- assets -->

[docs._assets.preview_image]: docs/_assets/preview_image.gif
[docs._assets.external-pq-hosting-1]: docs/_assets/external-pq-hosting-1.png
[docs._assets.external-pq-hosting-2]: docs/_assets/external-pq-hosting-2.png
[docs._assets.external-pq-hosting-3]: docs/_assets/external-pq-hosting-3.png
[docs._assets.external-pq-hosting-4-5]: docs/_assets/external-pq-hosting-4-5.png
[docs._assets.external-pq-hosting-6]: docs/_assets/external-pq-hosting-6.png
[docs._assets.external-pq-hosting-7]: docs/_assets/external-pq-hosting-7.png
[docs._assets.external-pq-hosting-8-9]: docs/_assets/external-pq-hosting-8-9.png
[docs._assets.external-pq-hosting-10-11]: docs/_assets/external-pq-hosting-10-11.png
[docs._assets.external-pq-hosting-12]: docs/_assets/external-pq-hosting-12.png
[docs._assets.external-pq-hosting-13]: docs/_assets/external-pq-hosting-13.png
[docs._assets.external-pq-hosting-14-15]: docs/_assets/external-pq-hosting-14-15.png
[docs._assets.external-pq-hosting-16-18]: docs/_assets/external-pq-hosting-16-18.png
[docs._assets.external-pq-hosting-19]: docs/_assets/external-pq-hosting-19.png
[docs._assets.external-pq-hosting-20-21]: docs/_assets/external-pq-hosting-20-21.png
[docs._assets.external-pq-hosting-22]: docs/_assets/external-pq-hosting-22.png
[docs._assets.external-pq-hosting-23]: docs/_assets/external-pq-hosting-23.png
[docs._assets.external-pq-hosting-24]: docs/_assets/external-pq-hosting-24.png
[docs._assets.external-pq-hosting-25-26]: docs/_assets/external-pq-hosting-25-26.png
[docs._assets.external-pq-hosting-27]: docs/_assets/external-pq-hosting-27.png
[docs._assets.external-pq-hosting-28-29]: docs/_assets/external-pq-hosting-28-29.png
[docs._assets.external-pq-hosting-30]: docs/_assets/external-pq-hosting-30.png
[docs._assets.external-pq-hosting-31]: docs/_assets/external-pq-hosting-31.png
[docs._assets.external-pq-hosting-32]: docs/_assets/external-pq-hosting-32.png

[docs._assets.external-putty-1]: docs/_assets/external-putty-1.png
[docs._assets.external-putty-2]: docs/_assets/external-putty-2.png
[docs._assets.external-putty-3]: docs/_assets/external-putty-3.png
[docs._assets.external-putty-4-6]: docs/_assets/external-putty-4-6.png
[docs._assets.external-putty-7-8]: docs/_assets/external-putty-7-8.png
[docs._assets.external-putty-9]: docs/_assets/external-putty-9.png
[docs._assets.external-putty-10-11]: docs/_assets/external-putty-10-11.png

[docs._assets.external-outline-manager-2]: docs/_assets/external-outline-manager-2.png
[docs._assets.external-outline-manager-3]: docs/_assets/external-outline-manager-3.png
[docs._assets.external-outline-manager-4-5]: docs/_assets/external-outline-manager-4-5.png
[docs._assets.external-outline-manager-7]: docs/_assets/external-outline-manager-7.png
[docs._assets.external-outline-manager-8]: docs/_assets/external-outline-manager-8.png
[docs._assets.external-outline-manager-9]: docs/_assets/external-outline-manager-9.png
[docs._assets.external-outline-manager-10]: docs/_assets/external-outline-manager-10.png
[docs._assets.external-outline-manager-11-12]: docs/_assets/external-outline-manager-11-12.png
[docs._assets.external-outline-manager-14]: docs/_assets/external-outline-manager-14.png
[docs._assets.external-outline-manager-15]: docs/_assets/external-outline-manager-15.png
[docs._assets.external-outline-manager-16]: docs/_assets/external-outline-manager-16.png
[docs._assets.external-outline-manager-17-18]: docs/_assets/external-outline-manager-17-18.png

[docs._assets.external-outline-client-2]: docs/_assets/external-outline-client-2.png
[docs._assets.external-outline-client-3-4]: docs/_assets/external-outline-client-3-4.png

[docs._assets.external-outline-keys-2]: docs/_assets/external-outline-keys-2.png
[docs._assets.external-outline-keys-3-4]: docs/_assets/external-outline-keys-3-4.png
[docs._assets.external-outline-keys-5-6]: docs/_assets/external-outline-keys-5-6.png
[docs._assets.external-outline-keys-8]: docs/_assets/external-outline-keys-8.png
[docs._assets.external-outline-keys-9-10]: docs/_assets/external-outline-keys-9-10.png
[docs._assets.external-outline-keys-11]: docs/_assets/external-outline-keys-11.png
[docs._assets.external-outline-keys-12]: docs/_assets/external-outline-keys-12.png

[docs._assets.external-outline-client-mobile-1]: docs/_assets/external-outline-client-mobile-1.jpg
[docs._assets.external-outline-client-mobile-2]: docs/_assets/external-outline-client-mobile-2.jpg
[docs._assets.external-outline-client-mobile-3]: docs/_assets/external-outline-client-mobile-3.jpg
[docs._assets.external-outline-client-mobile-4]: docs/_assets/external-outline-client-mobile-4.jpg
[docs._assets.external-outline-client-mobile-5]: docs/_assets/external-outline-client-mobile-5.jpg
[docs._assets.external-outline-client-mobile-6]: docs/_assets/external-outline-client-mobile-6.jpg

<!-- external -->

[external.shadowsocks]: https://shadowsocks.org/en/index.html
[external.outline]: https://getoutline.org/
[external.outline.get-started]: https://getoutline.org/get-started/
[external.outline.manager]: https://getoutline.org/get-started/#step-1
[external.outline.client]: https://getoutline.org/get-started/#step-3
[external.hosting.pq.hosting]: https://pq.hosting/en/
[external.putty]: https://www.putty.org/