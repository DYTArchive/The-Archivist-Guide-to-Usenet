# Introduction

Welcome to **The Archivist Guide to Usenet**.

## Your Journey Into The Unknown

This guide will show you the process of creating an account on a provider, setting up software to download and upload, and using your new-found knowledge to archive your much-loved content.

## A Little About Usenet

Usenet is an underrated medium for archival. It has many potential uses within our community. It's unconventional, but once acquainted with it, it can serve its use surprisingly well, and it can even become a viable option for those that cannot afford the analogous physical or cloud storage. The main audience is pirates, and now the minority will be librarians!

11$ a month can get you 100 simultaneous connections with unlimited bandwidth. There are cheaper yearly plans that are only 3$ that offer 50 connections, but that will do just fine for most people. To really make use of all of those 100 connections you would need a 10Gbps internet connection.

I also have to mention that there are no storage quotas. You just upload, and they store, maybe. You don't have your own little private space and a limited amount. Everything you upload is immediately public and synced across multiple datacenters with their own rules, speeds, hardware, and country-specific laws. It's not a good idea to (accidentally) upload your private files on Usenet, so be careful. And have fun trying to get it removed. Great for being censorship-resistant, bad for mishaps. Content is stored on the servers anywhere between 1 and over 5000 days. Although the typical amount of days is between 2000 and 5000. There are still many files uploaded 14 years ago you can download today.

Technically, you have unlimited storage. Realistically, if you keep uploading TB of junk you'll get your account banned by the provider you use, and if your abuse is significant, it will make providers increase their subscription prices and restrict upload access, so don't ruin it for the rest of us.

## Technicalities

Usenet is the OG forum. Just like how content is served over HTTP, news (user-made, plain text posts that are similar to email) are served over NNTP, a fairly simple, robust, and extremely old protocol. These posts are submitted to groups such as `alt.binaries.multimedia`, `alt.binaries.documentaries`, `alt.linux` and many others. The standard format is `x`, `x.y`, `x.y.z`. The creations of new groups is up to the Higher Order of Usenet Wizards (they're actually called The Big-8 Management). You submit a request and they'll decide. But the creation of new groups is not something we need or want.

There isn't just one Usenet, but there is "one" agreed-upon Usenet synchronized over multiple datacenters. All of these Usenet providers have to store data like posts and groups on hardware, usually in datacenters. They have all agreed a long time ago to talk to each other and synchronize data between each other. It's purely a mutual agreement that can be broken due to DMCA violations, illegal content, or anything like that. But most of the time, if some content is not available on one provider, it will be available on some other or multiple others.

Someone went ahead and thought of adding binaries to Usenet. The only limitation is that articles posted on the network have a fixed size. The big idea was to just split the files across multiple articles, in plain text. It's not that inefficient and works fairly well. You then assemble those pieces into files. The way you give instructions on how to assemble those articles together is typically by adding them to a file called an NZB, an XML file that has links to the articles. Whatever Usenet downloader you use reads that file, downloads the articles, and then merges them into actual files.