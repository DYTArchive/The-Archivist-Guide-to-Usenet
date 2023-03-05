# Uploading

To upload content to Usenet, you must use a provider that allows upload access. Fortunately, the providers I have listed in the [Downloading](./download.md) section are fit for this role.

The software I recommend is [Nyuu](https://github.com/animetosho/Nyuu). It has [clear performance benefits](https://github.com/animetosho/Nyuu/blob/master/bench/info.md#results) and is used by the anime uploading service called [Anime Tosho](https://animetosho.org/).

You can begin using it by modifying the [sample configuration file](https://github.com/animetosho/Nyuu/blob/master/config-sample.json) with the login data your Usenet provider has given you. There are delimiters in the configuration file that are important to consider: "**Server Options**" and "**Article Options**". The `from` and `comment` are arbitrary and should not contain personal information. They are as public as the files|articles you are uploading. 

The configuration file is read by using Nyuu as such: `nyuu -C config.json`. The options present in this file are the "defaults". Instead of modifying the contents of the file when faced with an edge case, you can specify or override them on runtime using it's various command-line parameters that are found through the help command `nyuu --help`.

Remember to increase the number of connections to the one allowed by your provider (50 or 100 usually) to improve the upload speed significantly.

This is an example use of Nyuu reading from the configuration file, uploading all files from a directory recursively (through all the subdirectories and their children) to the group `alt.binaries.multimedia`, and outputting the articles to an NZB file:

```
nyuu -C config.json -r -g alt.binaries.multimedia -o ./jawed.nzb ./youtube/jawed/ 
```