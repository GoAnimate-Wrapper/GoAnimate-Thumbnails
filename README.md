# GoAnimate-Thumbnails
This repository is a storage location for stock-character thumbnails.  If you're curious, I got the item IDs by running a quick Powershell script to perform regex-search on [the theme files](https://github.com/GoAnimate-Wrapper/GoAnimate-Wrapper/tree/master/themes).  The original file URLs were obtained with the following PowerShell script:
```ps
Select-String -Path ../ga-w/themes/*.xml -Pattern 'https://s3.amazonaws.com/fs.{1,30}.com/files/thumbnails/ccthumb.{1,70}\.png' -AllMatches | % {$_.Matches.Value}
```
