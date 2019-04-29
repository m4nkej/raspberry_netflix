# raspberry_netflix
```
sudo -i
apt-get remove chromium-browser
dpkg -r chromium-browser
rm -Rf /etc/chromium-browser
rm -Rf ~/.config/chromium
exit
rm -Rf ~/.config/chromium
cd ~/Downloads
wget https://github.com/kusti8/chromium-build/releases/download/netflix-1.0.0/chromium-browser_56.0.2924.84-0ubuntu0.14.04.1.1011.deb
sudo dpkg -i ./chromium-browser_56.0.2924.84-0ubuntu0.14.04.1.1011.deb
wget https://github.com/nateg5/Android/releases/download/NateCast/drm.zip
unzip drm.zip
sudo cp libwidevinecdm.so /usr/lib/chromium-browser/libwidevinecdm.so
sudo cp libpepflashplayer.so /usr/lib/chromium-browser/libpepflashplayer.so
sudo chmod 755 /usr/lib/chromium-browser/libwidevine*
sudo chmod 755 /usr/lib/chromium-browser/libpepflashplayer.so
```
