# Chill TV
## Live TV. Free. No ads.
![A photo of the ChillTV loading screen](https://i.ibb.co/7Yd8XmV/loading.jpg)
Want to watch your favorite channels for free but don't want to deal with annoying advertisements? Maybe Chill TV is right for you! (For legal reasons, by using Chill TV you agree to [this license agreement](https://github.com/chillsocial/ChillTV/blob/main/LICENSE.md).

This README will be broken down into three categories, how to set it up and how to use it.

## Set Up
### XAMPP (Private - Supports Windows, Linux and MacOS X)
This documentation assumes you are using XAMPP on a Windows computer and you have admin permissions. If your computer is managed, contact your organization to give you admin privlidges.

1. [Download the ZIP version of the service pack](https://github.com/chillsocial/ChillTV/raw/main/chillTVServicePack.zip).
2. If you don't have XAMPP, [download it](https://www.apachefriends.org/download.html). If possible, use the latest version.
3. Run `Windows Key + R` and type `C:\xampp\htdocs` in the box. Press the enter key and make sure all files in this folder are deleted.
4. In a new File Explorer window, find the ZIP, rightclick it and click `Extract All`. When it asks what folder you want to extract it to, type `C:\xampp\htdocs` in that box. Press enter.
5. Open XAMPP and make sure the `Apache` service is enabled. All other services should be disabled.
6. Open your browser. In your browser, go to `http://localhost`. If this doesn't work, try `http://localhost:80`.
7. Enjoy your private Chill TV server! :D
### Web Server (Public - Supports Any Modern Browser)
This documentation assumes you are using a Nginx webserver with PHP on a Pterodactyl-based hosting provider. Contact your hosting provider if you need spesific directions in regards to extracting files.

1. Download the service pack (Chill TV supports [zip](https://github.com/chillsocial/ChillTV/raw/main/chillTVServicePack.zip) and [tar.gz](https://github.com/chillsocial/ChillTV/raw/main/chillTVServicePack.tar.gz))
2. In Pterodactyl, select your Nginx server then click the file manager. Open the `webroot` folder and make sure its empty. If you want to run Chill TV in a folder (i.e. running Chill TV at `example.com/chill-tv/index.php` instead of `example.com`), create a folder, open it and make sure its empty.
3. Upload the `zip` or `tar.gz` to the folder (Pterodactyl supports both).
4. Once uploaded, right-click it and click `Unarchive` from the menu that appeared.
5. Ensure your server is running and a domain is either pointed to the server or you used a reverse proxy.
6. Share your server's URL to get more users! :D

## How To Use
### First Time Use and Changing CDN
You'll first be asked to select or enter a CDN. TV channels will be fetched from this CDN. You have three options...
- Enter your two-letter CountryID to get channels from [IPTV-Restream](https://github.com/iptv-restream/iptv-channels)
- Select a CDN from a list I made (there's 8 options, feel free to try out whatever one you like :D)
- If you have an M3U list, you can load it as a CDN

You can return to this screen by clicking `Change CDN?` on the main menu.
### Menu and Streaming
On the main menu, you will see a selection of logos. Select a logo to watch that channel. The stream will open in a new tab (no, its not a redirect to a third-party site, you'll still be on Chill TV!). Once done watching, close this tab to return to Chill TV.
