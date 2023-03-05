# Downloading

The most commonly used and actively maintained "Binary Newsreader" (downloader) is [SABnzbd](https://sabnzbd.org/). Highly extensible and performant, it runs on a WebUI that you can access over the internet or on your local network.

SABnzbd already has its own guides on how to install and set it up. Here's the one for [Windows](https://sabnzbd.org/wiki/installation/install-windows) and the one for [Linux](https://sabnzbd.org/wiki/installation/install-unix).

If you're running Linux as your desktop and want to run SABnzbd on your user account and have it start with your system, you should execute the following command:

```
sudo systemctl enable --now sabnzbd@your username, this is a placeholder, replace it with your actual username
```

Once you've added the servers (providers) to SABnzbd, you can test out your speed by reading an NZB file. You can get one from [NZBKing](https://nzbking.com/). You will be surprised at the speeds you can achieve. The NZB file is plain text XML, and you should examine its format to gain a better understand of how it works.