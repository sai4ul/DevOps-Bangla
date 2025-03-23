# Top 30 Linux Commands for DevOps (Bangla and English)
এই কমান্ডগুলি একজন DevOps ইঞ্জিনিয়ারের দৈনন্দিন কাজের জন্য অত্যন্ত গুরুত্বপূর্ণ। এগুলি ভালোভাবে জানা থাকলে সিস্টেম অ্যাডমিনিস্ট্রেশন, অটোমেশন, মনিটরিং, এবং ট্রাবলশুটিং কাজগুলি অনেক সহজ হয়ে যায়।


## 1. `ls`
**English:** Used to list files and directories within a folder.
**বাংলা:** ডিরেক্টরি বা ফোল্ডারের ভিতরে থাকা ফাইল এবং ফোল্ডারগুলি দেখার জন্য ব্যবহৃত হয়।
```bash
ls -la  # Lists all files (including hidden ones) with detailed information
        # সমস্ত ফাইল (লুকানো ফাইলসহ) বিস্তারিত তথ্যসহ দেখায়
```

## 2. `cd`
**English:** Used to change from one directory to another.
**বাংলা:** এক ডিরেক্টরি থেকে অন্য ডিরেক্টরিতে যাওয়ার জন্য ব্যবহৃত হয়।
```bash
cd /var/log  # Changes to the /var/log directory
             # /var/log ডিরেক্টরিতে যাবে
cd ..        # Moves up one level in the directory structure
             # একধাপ উপরের ডিরেক্টরিতে যাবে
```

## 3. `pwd`
**English:** Used to display the current directory path.
**বাংলা:** বর্তমানে আপনি কোন ডিরেক্টরিতে আছেন তা দেখার জন্য ব্যবহৃত হয়।
```bash
pwd  # Shows the full path of the current directory
     # বর্তমান ডিরেক্টরির পূর্ণ পাথ দেখাবে
```

## 4. `grep`
**English:** Used to search for specific patterns or text in files.
**বাংলা:** ফাইলের মধ্যে নির্দিষ্ট প্যাটার্ন বা টেক্সট খোঁজার জন্য ব্যবহৃত হয়।
```bash
grep "error" /var/log/syslog  # Searches for the word "error" in the system log
                              # সিস্টেম লগে "error" শব্দটি খুঁজবে
grep -r "text" /path/to/dir   # Recursively searches for "text" in all files
                              # রিকার্সিভভাবে সব ফাইলে খোঁজে
```

## 5. `find`
**English:** Used to search for files and directories.
**বাংলা:** ফাইল এবং ডিরেক্টরি খোঁজার জন্য ব্যবহৃত হয়।
```bash
find /home -name "*.txt"      # Finds all .txt files in the /home directory
                              # /home ডিরেক্টরিতে সব .txt ফাইল খুঁজবে
find / -type f -size +100M    # Finds files larger than 100MB
                              # 100MB-এর বেশি সাইজের ফাইল খুঁজবে
```

## 6. `ps`
**English:** Used to view currently running processes.
**বাংলা:** বর্তমানে চলমান প্রসেসগুলি দেখার জন্য ব্যবহৃত হয়।
```bash
ps aux  # Displays all running processes on the system
        # সিস্টেমে চলমান সমস্ত প্রসেস দেখাবে
```

## 7. `top` / `htop`
**English:** Used for real-time system performance monitoring.
**বাংলা:** সিস্টেমের রিয়েল-টাইম পারফরম্যান্স মনিটরিং করার জন্য ব্যবহৃত হয়।
```bash
top     # Shows processes, CPU and memory usage
        # প্রসেস, CPU এবং মেমরি ব্যবহার দেখাবে
htop    # An improved version of top, more user-friendly
        # top-এর উন্নত সংস্করণ, আরও ইউজার-ফ্রেন্ডলি
```

## 8. `systemctl`
**English:** Used to manage system services.
**বাংলা:** সিস্টেম সার্ভিসগুলি পরিচালনা করার জন্য ব্যবহৃত হয়।
```bash
systemctl status nginx     # Shows the status of the nginx service
                          # nginx সার্ভিসের স্টেটাস দেখাবে
systemctl restart docker   # Restarts the docker service
                          # ডকার সার্ভিস পুনরায় চালু করবে
```

## 9. `journalctl`
**English:** Used to view logs for systemd services.
**বাংলা:** systemd সার্ভিসগুলির লগ দেখার জন্য ব্যবহৃত হয়।
```bash
journalctl -u nginx        # Shows logs for the nginx service
                          # nginx সার্ভিসের লগ দেখাবে
journalctl -f              # Shows live logs (in follow mode)
                          # লাইভ লগ দেখাবে (follow মোড)
```

## 10. `netstat` / `ss`
**English:** Used to view network connections, routing tables, and interfaces.
**বাংলা:** নেটওয়ার্ক কানেকশন, রাউটিং টেবিল এবং ইন্টারফেস দেখার জন্য ব্যবহৃত হয়।
```bash
netstat -tulpn    # Shows open ports and associated processes
                 # খোলা পোর্ট এবং সম্পর্কিত প্রসেস দেখাবে
ss -tunlp         # Modern alternative to netstat
                 # netstat-এর আধুনিক বিকল্প
```

## 11. `df`
**English:** Used to display disk space usage.
**বাংলা:** ডিস্ক স্পেস ব্যবহার দেখার জন্য ব্যবহৃত হয়।
```bash
df -h    # Shows disk space in human-readable format
        # মানব-পঠনযোগ্য ফরম্যাটে ডিস্ক স্পেস দেখাবে
```

## 12. `du`
**English:** Used to check the size of files and directories.
**বাংলা:** ফাইল এবং ডিরেক্টরির সাইজ দেখার জন্য ব্যবহৃত হয়।
```bash
du -sh /var/log   # Shows the total size of the /var/log directory
                 # /var/log ডিরেক্টরির মোট সাইজ দেখাবে
du -sh *          # Shows the size of each item in the current directory
                 # বর্তমান ডিরেক্টরির প্রতিটি আইটেমের সাইজ দেখাবে
```

## 13. `tail`
**English:** Used to view the end of a file, especially for monitoring log files.
**বাংলা:** ফাইলের শেষাংশ দেখার জন্য ব্যবহৃত হয়, বিশেষ করে লগ ফাইল মনিটর করতে।
```bash
tail -f /var/log/syslog    # Shows the last lines of the system log and follows updates
                          # সিস্টেম লগের শেষ লাইনগুলি দেখাবে এবং আপডেট ফলো করবে
tail -n 100 file.log       # Shows the last 100 lines of the file
                          # ফাইলের শেষ 100 লাইন দেখাবে
```

## 14. `sed`
**English:** Used for text transformation, filtering, and replacement.
**বাংলা:** টেক্সট ট্রান্সফরমেশন, ফিল্টারিং এবং রিপ্লেসমেন্টের জন্য ব্যবহৃত হয়।
```bash
sed 's/old/new/g' file.txt    # Replaces "old" with "new" in the file
                             # ফাইলে "old" কে "new" দিয়ে প্রতিস্থাপন করবে
```

## 15. `awk`
**English:** Used for text processing and data extraction.
**বাংলা:** টেক্সট প্রসেসিং এবং ডেটা এক্সট্রাকশনের জন্য ব্যবহৃত হয়।
```bash
awk '{print $1}' file.txt    # Prints the first column of each line in the file
                            # ফাইলের প্রতি লাইনের প্রথম কলাম প্রিন্ট করবে
```

## 16. `curl`
**English:** Used to transfer data from the command line.
**বাংলা:** কমান্ড লাইন থেকে ডেটা ট্রান্সফার করার জন্য ব্যবহৃত হয়।
```bash
curl -I https://example.com    # Shows HTTP headers of the website
                              # ওয়েবসাইটের HTTP হেডার দেখাবে
curl -o file.txt https://example.com/file    # Downloads a file
                                            # ফাইল ডাউনলোড করবে
```

## 17. `wget`
**English:** Used to download files from the internet.
**বাংলা:** ইন্টারনেট থেকে ফাইল ডাউনলোড করার জন্য ব্যবহৃত হয়।
```bash
wget https://example.com/file.zip    # Downloads the file
                                    # ফাইল ডাউনলোড করবে
```

## 18. `docker`
**English:** Used to manage Docker containers.
**বাংলা:** ডকার কন্টেইনার পরিচালনা করার জন্য ব্যবহৃত হয়।
```bash
docker ps          # Shows running containers
                  # চলমান কন্টেইনার দেখাবে
docker images      # Shows downloaded images
                  # ডাউনলোড করা ইমেজ দেখাবে
docker-compose up  # Starts docker-compose services
                  # ডকার-কম্পোজ সার্ভিস শুরু করবে
```

## 19. `kubectl`
**English:** Used to manage Kubernetes clusters.
**বাংলা:** কুবারনেটিস ক্লাস্টার পরিচালনা করার জন্য ব্যবহৃত হয়।
```bash
kubectl get pods             # Shows pods
                            # পড দেখাবে
kubectl describe deployment  # Shows detailed info about a deployment
                            # ডিপ্লয়মেন্টের বিস্তারিত তথ্য দেখাবে
```

## 20. `git`
**English:** Used for version control and code management.
**বাংলা:** ভার্সন কন্ট্রোল এবং কোড পরিচালনার জন্য ব্যবহৃত হয়।
```bash
git clone repo-url           # Clones a repository
                            # রিপোজিটরি ক্লোন করবে
git pull                     # Pulls changes
                            # পরিবর্তন পুল করবে
git commit -m "message"      # Commits changes
                            # পরিবর্তন কমিট করবে
```

## 21. `ssh`
**English:** Used to establish secure connections to remote servers.
**বাংলা:** রিমোট সার্ভারে সিকিউর কানেকশন স্থাপন করার জন্য ব্যবহৃত হয়।
```bash
ssh user@hostname            # Logs into a remote server
                            # রিমোট সার্ভারে লগইন করবে
ssh -i key.pem user@hostname # Logs in using a key file
                            # কী ফাইল ব্যবহার করে লগইন করবে
```

## 22. `scp`
**English:** Used to securely copy files between two hosts.
**বাংলা:** দুটি হোস্টের মধ্যে সিকিউরভাবে ফাইল কপি করার জন্য ব্যবহৃত হয়।
```bash
scp file.txt user@hostname:/path    # Copies file from local to remote server
                                   # লোকাল থেকে রিমোট সার্ভারে ফাইল কপি করবে
scp user@hostname:/path/file.txt .  # Copies file from remote to local
                                   # রিমোট থেকে লোকালে ফাইল কপি করবে
```

## 23. `tar`
**English:** Used to archive and compress files.
**বাংলা:** ফাইল আর্কাইভ করার এবং কম্প্রেস করার জন্য ব্যবহৃত হয়।
```bash
tar -cvzf archive.tar.gz /path/to/dir    # Compresses a directory
                                        # ডিরেক্টরি কম্প্রেস করবে
tar -xvzf archive.tar.gz                 # Extracts an archive
                                        # আর্কাইভ এক্সট্রাক্ট করবে
```

## 24. `crontab`
**English:** Used to schedule automatic tasks at specific times.
**বাংলা:** নির্দিষ্ট সময়ে স্বয়ংক্রিয় কাজ সম্পাদন করার জন্য ব্যবহৃত হয়।
```bash
crontab -l    # Lists current cron jobs
             # বর্তমান cron জব দেখাবে
crontab -e    # Edits cron jobs
             # cron জব সম্পাদনা করবে
```

## 25. `vim` / `nano`
**English:** Used to edit text files.
**বাংলা:** টেক্সট ফাইল সম্পাদনা করার জন্য ব্যবহৃত হয়।
```bash
vim file.txt    # Opens file in vim editor
               # vim এডিটরে ফাইল খুলবে
nano file.txt   # Opens file in nano editor (easier for beginners)
               # nano এডিটরে ফাইল খুলবে (শুরু করার জন্য সহজ)
```

## 26. `chmod`
**English:** Used to change permissions of files and directories.
**বাংলা:** ফাইল এবং ডিরেক্টরির অনুমতি পরিবর্তন করার জন্য ব্যবহৃত হয়।
```bash
chmod +x script.sh    # Makes the script executable
                     # স্ক্রিপ্টকে এক্সিকিউটেবল করবে
chmod 755 file        # Sets rwx permissions
                     # rwx ছক সেট করবে
```

## 27. `chown`
**English:** Used to change ownership of a file or directory.
**বাংলা:** ফাইল বা ডিরেক্টরির মালিকানা পরিবর্তন করার জন্য ব্যবহৃত হয়।
```bash
chown user:group file.txt    # Changes the user and group of the file
                            # ফাইলের ইউজার এবং গ্রুপ পরিবর্তন করবে
```

## 28. `iptables`
**English:** Used to manage the Linux firewall.
**বাংলা:** লিনাক্স ফায়ারওয়াল পরিচালনা করার জন্য ব্যবহৃত হয়।
```bash
iptables -L    # Lists firewall rules
              # ফায়ারওয়াল রুল দেখাবে
```

## 29. `ping`
**English:** Used to test network connectivity.
**বাংলা:** নেটওয়ার্ক কানেক্টিভিটি পরীক্ষা করার জন্য ব্যবহৃত হয়।
```bash
ping google.com    # Sends ping to google.com
                  # google.com-এ পিং পাঠাবে
```

## 30. `history`
**English:** Used to view previously used commands.
**বাংলা:** আগে ব্যবহৃত কমান্ডগুলি দেখার জন্য ব্যবহৃত হয়।
```bash
history     # Shows command history
           # কমান্ড হিস্টরি দেখাবে
!123        # Re-runs command number 123 from history
           # হিস্টরিতে 123 নম্বর কমান্ড আবার চালাবে
```

**English Summary:** These commands are essential for the daily work of a DevOps engineer. Having a good understanding of these commands makes system administration, automation, monitoring, and troubleshooting tasks much easier.

**বাংলা সারাংশ:** এই কমান্ডগুলি একজন DevOps ইঞ্জিনিয়ারের দৈনন্দিন কাজের জন্য অত্যন্ত গুরুত্বপূর্ণ। এগুলি ভালোভাবে জানা থাকলে সিস্টেম অ্যাডমিনিস্ট্রেশন, অটোমেশন, মনিটরিং, এবং ট্রাবলশুটিং কাজগুলি অনেক সহজ হয়ে যায়।
