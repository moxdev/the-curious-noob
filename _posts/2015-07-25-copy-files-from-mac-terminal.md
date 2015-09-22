---
layout: post
title: "Copy Files From The Mac Terminal"
modified: 2015-07-25 15:21:38 -0400
tags: [terminal, mac, "copy files", "move files", "command line"]
image:
  feature: abstract-5.jpg
  credit: dargadgetz
  creditlink: http://www.dargadgetz.com/ios-7-abstract-wallpaper-pack-for-iphone-5-and-ipod-touch-retina/
comments: true
share: true
---
### Quickly Copy or Move Files and Folders From the Mac Terminal
Today we are going to take a look at a very simple and efficient way to copy or move files and folders from one location to another using just the Terminal commands on a Mac.

#### Copy Command "cp"
The basic concept uses this format:
`cp source destination'

Lets say you want to copy the document "MyFile.rtf" from your Desktop to your Documents folder. You would type the below command in your terminal.
`cp ~/Desktop/MyFile.rtf ~/Documents`

Sometimes you may want to copy an entire directory. To do that you need to use the `-r` flag which tells the OS to copy everything in the directory. The command below will copy the folder "MyFolder" from your Desktop to the "Backup" volume.
`cp -r ~Desktop/MyFolder /Volume/Backup`

#### Move Command "mv"
Now keep in mind that so far we are just copying files and folders, which means the original file/folder remains in its original location. This results in two copies of the same file/folder. In order to actually move a file/folder from one directory to another we need to use the `mv` command.

This will actually move the file from your Desktop to your Documents folder.
`mv ~/Desktop/MyFile.rtf ~/Documents`

We can also use the same command to move a folder from one directory to another. Notice that you do not need to include the `-r` flag with the `mv` command.
`mv ~Desktop/MyFolder /Volume/Backup`

Stay tuned as I will be posting more useful terminal commands that will increase your speed and efficiency by never leaving the terminal window to accomplish your tasks!