[#]: subject: "5 Useful Linux Command Line Tools that Everyone Should Use"
[#]: via: "https://www.debugpoint.com/2022/06/useful-linux-command/"
[#]: author: "Arindam https://www.debugpoint.com/author/admin1/"
[#]: collector: "lkxed"
[#]: translator: " "
[#]: reviewer: " "
[#]: publisher: " "
[#]: url: " "

5 Useful Linux Command Line Tools that Everyone Should Use
======
In this article, I will explain five useful Linux command(s) that will change your life forever.

### 5 Useful Linux Command(s)

#### 1. rmlint

Have you ever wondered how you can easily find duplicate, empty folders and empty files? Well, for that, there is a nifty utility called **rmlint**.

The [rmlint][1] scans your file system and tells you how much space is taken by duplicate files, folders, broken symlinks, empty files and more.

Moreover, it gives you an autogenerated shell script to remove all those files with just a single command. In addition, it also outputs a nice-looking report for your to analyze.

I think it’s a must-have terminal utility for your Ubuntu, Fedora and other Linux systems. Here are two images of rmlint in action.

![rmlint output – Figure 1][2]

![rmlint output – Figure 2][3]

Let’s take a look at how you can install rmlint. Installation is easy as it’s available in the major distro’s repo. Here are the commands

For Ubuntu, Linux Mint and similar distros:

```
sudo apt install rmlint
```

For Fedora, RHEL and similar distros:

```
sudo dnf install rmlint
```

After installation, run `rmlint` from the terminal. And it will give you a summary of the status of your system.

```
rmlint
```

Not only that, but you can also scan by file size, modification dates and so on—all the examples you can find in the [beginner’s guide][4].

#### 2. ntfy

The second useful command in this list is ntfy. It is a nifty utility that helps you send notifications to your desktop. The ntfy works via system DBUS and libnotify in all the popular Linux desktops (KDE Plasma, GNOME) and provides a system-like notification.

Now, you may ask – why do you need to send a custom notification?

Well, think about a use case where you are writing some script to achieve some purpose (e.g. taking backups), and you need the script to send a notification after it finishes. In this example, you can run ntfy via shell script to notify that the backup is complete.

The syntax of ntfy is simple.

```
ntfy send "Your task is complete"
```

![ntfy output][5]

Installing ntfy requires Python3. In Ubuntu Linux, you can install it using the below set of commands.

```
sudo apt install python3-pippip install ntfy
```

By default, it installs the binary at ~/.local/bin, where you can get the executable to run.

You can further customize it with its wide range of options available in the [documentation][6].

#### 3. btop

There are some excellent terminal-based system monitors available. And I think btop is the best. Firstly, it’s available pre-compiled executable, so you do not need to install it. All you need to do is download and run.

Secondly, one single interface gives you the entire system snapshot, containing the following features.

* Battery level and available time
* Disks usage by partition and IO
* Process list with executables, path, threads, memory and lazy CPU
* Deep dive into a single process to investigate
* Network interface utilization details

In addition, you can also configure it with various themes from its settings. I think it’s a perfect utility for terminal lovers to monitor your system.

![btop][7]

To get this application, visit the [GitHub page here][8] and download the zip file for Linux distros. You need to run the executable after extracting the zip file.

#### 4. ncdu

The fourth command in this list is super helpful ncdu (NCurses Disk Usage). The ncdu is a disk usage analyzer with an NCurses interface which scans your system and gives you an excellent representation of the disk space status in the terminal.

Then, you can use this report and manually remove the files which are not needed.

Furthermore, ncdu is a perfect tool to analyze your remote servers where you do not have access to a graphical user interface. It’s simple, fast and can run in any POSIX-like environment.

In addition, you can also browse the directories via keyboard in the terminal, and you can sort by size, date, etc.

That’s not all. Ncdu is available for almost all Linux distributions. Here are the commands to install in Ubuntu and Fedora-related distributions.

```
sudo apt install ncdu
```

```
sudo dnf install ncdu
```

![ncdu][9]

For more details, visit the [homepage][10].

#### 5. rclone

The rclone is the best command-line program to sync and manage files from your local system to the cloud storage such as Google driver, AWS etc. It’s a feature-rich program which currently supports 40+ cloud storage products.

Moreover, if you configure rclone effectively, you may not need rsync or login to the cloud provider’s web interface to manage your files. All of the operations can be easily done via the terminal.

Not only that, but rclone is also capable of handling the integrity of data such as:

* Verify checksum
* Preserve timestamps
* Options to transfer over limited bandwidth

In addition, to make it safer, it provides a “–dry-run” switch to verify which files or folders get replaced during the sync operation to the cloud.

You can install rclone using the commands below in your favourite distros.

After you install, head over to [this page][11]. For each cloud storage provider, there is a one-time configuration needed. Choose your cloud provider and select the config link. Then follow the easy instructions to set up.

For more details and documentation, visit the [official website][12].

### Closing Notes

We discussed some useful command-line tools in this article. These tools are perfect for remote system administration from anywhere in the world. It ranges from disk usage analyzer, system monitors and backup of your data.

Do you know any other useful Linux command line tools? Let me know in the comment box below, and we will feature it in the next article.

--------------------------------------------------------------------------------

via: https://www.debugpoint.com/2022/06/useful-linux-command/

作者：[Arindam][a]
选题：[lkxed][b]
译者：[译者ID](https://github.com/译者ID)
校对：[校对者ID](https://github.com/校对者ID)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]: https://www.debugpoint.com/author/admin1/
[b]: https://github.com/lkxed
[1]: https://rmlint.readthedocs.io/en/latest/index.html
[2]: https://www.debugpoint.com/wp-content/uploads/2022/06/rmlint-output-Figure-1.jpg
[3]: https://www.debugpoint.com/wp-content/uploads/2022/06/rmlint-output-Figure-2.jpg
[4]: https://rmlint.readthedocs.io/en/latest/tutorial.html#beginner-examples
[5]: https://www.debugpoint.com/wp-content/uploads/2022/06/ntfy-output.jpg
[6]: https://ntfy.readthedocs.io/en/v2.0.1/
[7]: https://www.debugpoint.com/wp-content/uploads/2022/06/btop.jpg
[8]: https://github.com/aristocratos/btop/releases/
[9]: https://www.debugpoint.com/wp-content/uploads/2022/06/ncdu.jpg
[10]: https://dev.yorhel.nl/ncdu
[11]: https://rclone.org/#providers
[12]: https://rclone.org/