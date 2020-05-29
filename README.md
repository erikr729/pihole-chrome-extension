# Switch-for-PiHole ![t](https://github.com/badsgahhl/pihole-chrome-extension/blob/master/icon/icon-48.png?raw=true)

This is a small extension to revive the project of Yoder Spencer.
https://github.com/Spencer-Yoder/Remote-Switch-for-Pi-Hole-Chrome	

I reused some of his code and icons to build this extension, but a lot of parts got rebuild.
This extension is available in the chrome webstore and mozilla addon store.

![alt text](https://cdn.glaser.casa/s/B7bDBr8oVP_807c35a29a748ca0d4cbda4ced9c65613a0037de6bbba3059e.png)


### Features:
- Disable your pihole easily with one click
- Individual url to your pihole
- Dark Mode depending on your OS Settings
- Compact UI
- Settable default disable time
- White-/Blacklist your current tabs url with one click (PiHole v5.0+)

### How to use:

- Install the extension
- Right click the "Raspberry" Icon in the top navigation fo your browser and click 'Settings'
- Enter your host address (including http:// or https://)
- Go to your Pihole settings. Click 'Api/Web interface' and then on 'Show Api token' at the bottom of your screen.
- Copy the token to the settings. Press save.
- Congratulations you successfully installed and configured the extension.


### Troubleshooting

#### Status / Slider are not working
Please check that you used the correct host address. Use the address where you can see your dashboard page (statistics board).
For example if your pihole is located at http://192.168.178.2 but you can see your dashboard/admin page at http://192.168.178.2/admin then don't forget to add /admin to the address.

#### Error after clicking the Slider (was "on" before)

This indicates that your API key is probably wrong. In the version >2.0.6 the options will show you if your key is wrong.
Check that you copied the key correctly and that there are no whitespaces, etc. in it.

#### PiHole doesn't block ads after turning it on

Disabling your pihole works seamlessly. Turning it on, or turning on automatically after the timeout will need some seconds.
During the start ads will show up, and the popup won't show any status until the pihole is back online. Be patient.

#### Black- / Whitelisting domains
With the extension version v2.1 you are able to black and whitelist the current tabs url. This feature requires PiHole v5.
<br>Meaning of colors:
 - Orange: The domain wasn't added to any list
 - Green: The domain was successfully added to the list
 
**Known Bug:** Domains which you have manually added to one of the both lists cannot be added/changed via the extension.
This will be fixed in the next version of PiHole.

**What does that mean:** For example you added a domain to your blacklist (example.com), then you visit this domain in your browser.
You want to whitelist this domain with the extension now. If you click onto the whitelist button it will respond with orange and
the domain cannot be added to the whitelist (cannot be moved from the black to the whitelist). This will work in a future update of PiHole.

 

**This is not an official Pi-Hole application.**
<br>
Please use the issue templates in this repository for bugs. The main PiHole project is not responsible for any malfunction that is caused by the use of the extension!
