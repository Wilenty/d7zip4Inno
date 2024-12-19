# Delphi 7-zip for InnoSetup

[![Latest Version](https://img.shields.io/github/release/Wilenty/d7zip4Inno.svg)](https://github.com/Wilenty/d7zip4Inno/releases/latest)
[![Total Downloads](https://img.shields.io/github/downloads/Wilenty/d7zip4Inno/total.svg)](https://github.com/Wilenty/d7zip4Inno/releases)
[![Latest Release Downloads](https://img.shields.io/github/downloads/Wilenty/d7zip4Inno/latest/total.svg)](https://github.com/Wilenty/d7zip4Inno/releases/latest)

Basic rule of using this plugin in your project is simple - you have to provide link to this repository in your project about section or in the project documentation shared to the final consumer.

I decided to update and share here my fourth years old project, because... I tried to use extracting 7-zip archives in the latest (beta/dev) of InnoSetup and I was not able to extract any of them.

**Limitations of this plugin: it will not work with old ANSI versions of InnoSetup and cannot extract 7-zip archives when the dictionary has been set to over 1G/1024M.**

I tried to extract various 7-zip archives downloaded from the Internet and archives created locally using the new 7-zip extraction method in the latest version (beta/dev) of InnoSetup, and I was unable to extract anything. You have to create 7-zip archives with special command-line options to be able to extract them using 7-zip's internal extraction function in the InnoSetup. So it is completely useless.

This plugin supports all archives that 7-zip plugin supports, even the password protected. I had compiled few 7-zip plugins with limited archive support which allowed to reduce their size. So you can choose which one of them you will to use.

**Note: Extracting some old 7-zip archives with ExtractCallBack hangs the entire InnoSetup in some cases. I have tried using various ExtractCallBack options, but none of them helped in this case. So, repackage the old 7-zip archives to the new version or not using ExtractCallBack should help.**

### Credits:

https://github.com/ip7z/7zip

https://github.com/geoffsmith82/d7zip
