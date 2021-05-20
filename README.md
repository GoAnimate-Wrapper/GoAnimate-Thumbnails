# GoAnimate-Thumbnails
This repository is a storage location for stock-theme thumbnails originally hosted on Vyond.  If you'd like to know about how I did it, I got the item IDs by running a quick Powershell script to perform regex-search on [the theme files](https://github.com/GoAnimate-Wrapper/GoAnimate-Wrapper/tree/master/_THEMES).  The original file URLs were obtained with the following PowerShell script:
```ps
Select-String -Path ../ga-w/themes/*.xml -Pattern 'https://s3.amazonaws\.com/fs\.goanimate\.com/files/.{1,90}\.(?:png|jpg)' -AllMatches | % {$_.Matches.Value}
```
