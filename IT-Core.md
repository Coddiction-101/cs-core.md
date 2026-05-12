# 🖥️ IT FUNDAMENTALS - Complete Beginner to Advanced Guide

**What is IT?**
IT (Information Technology) = Using computers and technology to store, process, and share information.

---

## 📚 Table of Contents

1. [Part 1: Computer Hardware Basics](#part-1-computer-hardware-basics)
2. [Part 2: Software Fundamentals](#part-2-software-fundamentals)
3. [Part 3: Operating Systems](#part-3-operating-systems)
4. [Part 4: Storage & File Systems](#part-4-storage--file-systems)
5. [Part 5: Networking Basics](#part-5-networking-basics)
6. [Part 6: Internet & Web](#part-6-internet--web)
7. [Part 7: Cybersecurity Essentials](#part-7-cybersecurity-essentials)
8. [Part 8: Data & Databases](#part-8-data--databases)
9. [Part 9: Cloud Computing](#part-9-cloud-computing)
10. [Part 10: IT Support & Troubleshooting](#part-10-it-support--troubleshooting)

---

# PART 1: COMPUTER HARDWARE BASICS

## 1.1 What is Inside a Computer?

Think of a computer like a human body:
- **CPU** = Brain (thinks and makes decisions)
- **RAM** = Short-term memory (remembers while thinking)
- **Storage** = Long-term memory (remembers after shutting down)
- **Motherboard** = Nervous system (connects everything)
- **Power Supply** = Heart (pumps energy)

## 1.2 The Main Components

### **CPU (Central Processing Unit)**

**In Simple Terms:** The brain of the computer. It reads instructions and executes them.

**Key Points:**
- Measured in **GHz** (how fast it thinks)
- More GHz = faster processing
- Modern computers: 2-4 GHz

**Real World Example:**
```
If CPU is a worker:
- 1 GHz = 1 task per second
- 3 GHz = 3 tasks per second
- Faster CPU = more tasks done = faster computer
```

**Cores:**
- Single-core: 1 worker
- Dual-core: 2 workers (can do 2 things at once)
- Quad-core: 4 workers
- More cores = can do more things simultaneously

### **RAM (Random Access Memory)**

**In Simple Terms:** Your computer's short-term memory. Stores data while programs are running.

**Key Points:**
- **Volatile** = loses all data when powered off
- **Fast** = much faster than storage
- **Temporary** = only for active programs
- **Measured in GB** (gigabytes)

**How Much Do You Need?**
```
Basic Tasks (browsing, documents):    4-8 GB
Gaming, Video Editing:                16-32 GB
Professional Work:                    32+ GB
Server Computers:                     64-256+ GB
```

**Example:**
```
Scenario: Opening Microsoft Word

1. Word program stored on disk (slow storage)
2. You click Word icon
3. Computer loads Word into RAM (fast memory)
4. You can now use Word quickly
5. Close Word → RAM is freed up
6. Word program still on disk
```

### **Storage Devices**

**HDD (Hard Disk Drive) - Traditional**
```
How it works: Spinning magnetic disk + mechanical arm

Pros:
✓ Very cheap per GB
✓ Large capacity (up to 20TB)
✓ Good for backups

Cons:
✗ Slow (mechanical parts)
✗ Fragile (can fail from shock)
✗ Uses more power
```

**SSD (Solid State Drive) - Modern**
```
How it works: No moving parts, uses flash memory (like USB drives)

Pros:
✓ Very fast (10x faster than HDD)
✓ Durable (no moving parts)
✓ Uses less power
✓ Quieter

Cons:
✗ More expensive per GB
✗ Smaller capacity
✗ Can wear out over time (rarely)
```

**Speed Comparison:**
```
HDD:     150-200 MB/s (like a slow mail truck)
SSD:     500-7000 MB/s (like a jet airplane)

Real example: Copying 10GB file
HDD:      ~50 seconds
SSD:      ~2-4 seconds
```

### **Motherboard**

**In Simple Terms:** The circuit board that connects all computer parts together.

Think of it like:
```
Your computer parts = People
Motherboard = Roads connecting cities
Electricity flows through connections = Messages between parts
```

### **Power Supply Unit (PSU)**

**In Simple Terms:** Converts wall electricity to safe power for computers.

**Key Points:**
- Measured in **Watts (W)**
- Must match computer needs
- Provides clean, stable power

### **GPU (Graphics Processing Unit)**

**In Simple Terms:** Special processor for graphics and images.

**Originally Used For:**
- Games (rendering 3D graphics)
- Video editing

**Now Also Used For:**
- Artificial Intelligence (AI)
- Machine Learning
- Scientific calculations

---

## 1.3 Memory Hierarchy (Speed vs Storage)

Your computer has different types of memory, each with different speeds and sizes:

```
SPEED         SIZE          LOCATION
═════════════════════════════════════════════════════════════

Fast, Small   Registers     Inside CPU
              (bytes)       

              L1 Cache      Inside CPU
              (32 KB)       

              L2 Cache      Inside CPU
              (256 KB)      

              L3 Cache      Inside CPU
              (8 MB)        

              RAM           Connected to motherboard
              (8-64 GB)     

Slow, Big     SSD/HDD       Inside/External
              (256 GB-2 TB)
```

**Analogy:**
```
Finding information in different memories:

Registers    = Your brain (instant, small)
L1 Cache     = Your desk (very quick, limited)
RAM          = Your office (quick, medium)
SSD          = Your filing cabinet (slower, larger)
HDD/Cloud    = Off-site storage (very slow, huge)
```

---

## 1.4 How Different Computers Compare

### **Laptop vs Desktop**

| Feature | Laptop | Desktop |
|---------|--------|---------|
| Portability | ✓ Can carry | ✗ Fixed |
| Power | ◐ Medium | ✓ Maximum |
| Cost | ◐ More expensive | ✓ Cheaper |
| Upgradable | ✗ Limited | ✓ Easy |
| Heat | ◐ Gets hot | ✓ Better cooling |

### **Smartphone**

**Key Differences:**
```
Desktop/Laptop CPU:  Desktop-grade processors
Smartphone CPU:      Optimized for low power use
                     Much slower but very efficient

Desktop RAM:         8-64 GB
Smartphone RAM:      4-12 GB

Desktop Storage:     256 GB - 2 TB
Smartphone Storage:  64 GB - 512 GB (+ cloud)
```

### **Server Computers**

**Used For:**
- Running websites (hosts.com stores websites here)
- Storing company data
- Email servers
- Database servers

**Differences from Personal Computer:**
```
Your Computer:
- 1 user
- Shuts down at night
- Crashes once a month is OK

Server Computer:
- 1000s of users simultaneously
- Runs 24/7/365
- CANNOT crash (critical systems)
- Has backup power (generators)
- Has RAID storage (multiple copies)
```

---

# PART 2: SOFTWARE FUNDAMENTALS

## 2.1 What is Software?

**In Simple Terms:** Instructions that tell computers what to do.

Think of it like:
```
Hardware = Your car's engine and parts
Software = The driver who controls the car

Without driver: Car is useless
Without software: Computer is useless
```

## 2.2 Types of Software

### **1. Operating System (OS)**

**What it does:**
- Manages hardware (CPU, RAM, disk)
- Provides interface for users
- Manages files and folders
- Controls permissions
- Runs multiple programs

**Popular Operating Systems:**

```
Windows
├─ Made by: Microsoft
├─ Works on: Desktops, Laptops
├─ Market share: ~75%
└─ Known for: Games, Office work, Easy for beginners

macOS
├─ Made by: Apple
├─ Works on: Mac computers
├─ Market share: ~15%
└─ Known for: Design, Video editing, Quality

Linux
├─ Made by: Community (free and open-source)
├─ Works on: Servers, Desktops, Everything
├─ Market share: 2-5% (desktop), 96% (servers)
└─ Known for: Power users, Servers, Programmers

Android
├─ Made by: Google
├─ Works on: Smartphones, Tablets
├─ Market share: ~70% (mobile)
└─ Known for: Customization, Many devices

iOS
├─ Made by: Apple
├─ Works on: iPhones, iPads
├─ Market share: ~27% (mobile)
└─ Known for: Quality, Security, Simplicity
```

### **2. Application Software**

**Examples:**
```
Web Browsers:     Chrome, Firefox, Safari, Edge
Messaging:        WhatsApp, Telegram, Discord
Productivity:     Microsoft Office, Google Docs
Media:            Netflix, Spotify, YouTube
Games:            Fortnite, Call of Duty, Candy Crush
```

### **3. System Software**

**Purpose:** Keeps computer running smoothly

```
Drivers:           Tell OS how to use hardware (printer driver, GPU driver)
Utilities:         Cleanup tools, antivirus, file managers
Firmware:          Instructions stored in hardware (BIOS)
```

---

## 2.3 How Software Works

**Simple Explanation:**

```
You click an icon
         ↓
OS finds the program on storage (disk)
         ↓
Program loaded into RAM (memory)
         ↓
CPU executes the program's instructions
         ↓
GPU renders graphics
         ↓
You see the application on screen
```

**Real Example: Opening Google Chrome**

```
1. Chrome files stored on SSD/HDD
2. You double-click Chrome icon
3. OS loads Chrome into RAM
4. CPU starts executing Chrome code
5. Chrome window appears
6. You type in search box
7. Chrome sends data to Google servers
8. Google responds with search results
9. Chrome displays results on screen
```

---

# PART 3: OPERATING SYSTEMS

## 3.1 What Does an OS Do?

### **1. Resource Management**

**CPU Management:**
```
Problem: Many programs want CPU time simultaneously
Solution: OS divides CPU time among programs

Your computer might have:
- Chrome using 20% CPU
- Antivirus scanning: 30% CPU
- Background updates: 10% CPU
- Available for you: 40% CPU

OS decides who gets CPU time and when
```

**RAM Management:**
```
Problem: Programs want more RAM than you have
Solution: OS uses virtual memory (disk as overflow)

You have 8 GB RAM but need 12 GB:
- 8 GB in actual RAM
- 4 GB on SSD (virtual memory)
Slower but works!
```

**Disk Management:**
```
OS handles:
- Where files go on disk
- Finding files quickly
- Deleting files safely
- Preventing data loss
```

### **2. Device Management**

```
You plug in printer
         ↓
OS detects printer (Plug & Play)
         ↓
OS downloads/installs driver
         ↓
Applications can use printer
```

### **3. File Management**

```
Your folders and files organization:

C:\ (Windows) or / (Mac/Linux)
├── Users/
│   ├── YourName/
│   │   ├── Documents/
│   │   │   └── MyFile.docx
│   │   ├── Downloads/
│   │   └── Pictures/
├── Program Files/
└── Windows/ (system files)
```

### **4. Security**

```
OS provides:
✓ User accounts (different users, different files)
✓ Permissions (who can access what)
✓ Encryption (protect sensitive data)
✓ Firewall (protect from internet attacks)
```

## 3.2 Running Multiple Programs

**How can OS run 100s of programs simultaneously?**

```
Answer: It doesn't really. It switches very fast!

Timeline (milliseconds):

Time 1ms:  Run Chrome for 10ms
Time 11ms: Run Spotify for 10ms
Time 21ms: Run Word for 10ms
Time 31ms: Run Chrome for 10ms
...and so on

Switches happen so fast (milliseconds)
You think programs run simultaneously!
```

**This is called "Multitasking"**

---

# PART 4: STORAGE & FILE SYSTEMS

## 4.1 Understanding File Systems

**What is a File System?**

Think of it like a library:
```
Library:
├── Shelves (hard drive)
├── Sections (folders)
├── Books (files)
└── Card catalog (file system - tells you where everything is)
```

## 4.2 Common File Types

```
Documents:
.pdf       Portable Document Format (universal, unchangeable)
.doc/.docx Microsoft Word document
.txt       Plain text (any program can open)

Spreadsheets:
.xls/.xlsx Microsoft Excel
.csv       Comma-separated values (data format)

Images:
.jpg       Compressed photo format
.png       Lossless image (good quality)
.gif       Animation format

Videos:
.mp4       Most common video format
.avi       Video format (older)
.mkv       Video format (high quality)

Audio:
.mp3       Compressed audio
.wav       High-quality audio
.flac      Lossless audio

Code:
.py        Python program
.js        JavaScript code
.html      Web page

Compressed:
.zip       Compressed folder (like suitcase)
.rar       Another compression format
```

## 4.3 File Naming & Organization

**Bad Organization:**
```
C:\Desktop\
├── Document1.doc
├── Document2.doc
├── MyPhoto.jpg
├── Budget.xlsx
├── Vacation.jpg
└── Import.txt
(Chaos! Can't find anything)
```

**Good Organization:**
```
C:\Users\YourName\
├── Documents/
│   ├── Work/
│   │   ├── Budget.xlsx
│   │   └── Reports/
│   └── Personal/
├── Pictures/
│   ├── Vacation/
│   │   ├── Photo1.jpg
│   │   └── Photo2.jpg
│   └── Family/
└── Downloads/
(Clear structure, easy to find things)
```

## 4.4 Storage Needs

```
1 Photo (5 MB)
10 Videos (1 GB each = 10 GB)
100 Documents (1 MB each = 100 MB)
Your OS (Windows/Mac = 20-30 GB)
Applications (all software = 100-200 GB)
Free space for working (10-20% = important!)
────────────────────────────────────
Total needed: 256 GB to 1 TB (1000 GB)

That's why computers come with:
- 256 GB (small laptop)
- 512 GB (medium laptop)
- 1 TB (large, comfortable)
- 2 TB+ (professional, lots of files)
```

---

# PART 5: NETWORKING BASICS

## 5.1 What is a Network?

**In Simple Terms:** Computers connected together so they can share information.

```
Scenario: Your Home Network

    Your Smartphone
    Your Laptop
    Your Smart TV
    Your Printer
         ↓
    Router (WiFi box)
         ↓
    Internet (modem to ISP)
```

## 5.2 IP Addresses

**What is an IP Address?**

Think of it like:
```
Physical Address: 123 Main Street, Anytown
IP Address: 192.168.1.5

Every device on internet has unique IP address
So data knows where to go
```

### **IPv4 (Current Standard)**

```
Format: 192.168.1.1
Looks like: XXX.XXX.XXX.XXX
Each number: 0-255
Total possibilities: ~4 billion addresses

Problem: Only 4 billion addresses for 8 billion people!
Solution: IPv6 (next generation)
```

### **IPv6 (Future Standard)**

```
Format: 2001:0db8:85a3:0000:0000:8a2e:0370:7334
Length: Much longer
Possibilities: 340 undecillion (340 + 36 zeros)
Basically: Unlimited addresses forever
```

## 5.3 Internet Speed

```
Units:
Mbps = Megabits per second (for internet speed)
MBps = Megabytes per second (for file transfer)

Conversion: 1 MBps = 8 Mbps

Speed Comparison:
Dial-up (1990s):        56 Kbps (very slow)
DSL/Cable (2000s):      10-100 Mbps
Fiber (2010s+):         100-1000 Mbps
5G Network:             100-1000 Mbps

What speed do you need?
Browsing websites:      5 Mbps
Streaming HD video:     25 Mbps
4K video streaming:     50 Mbps
Gaming:                 10-25 Mbps
Work from home:         10-50 Mbps
Multiple people:        100+ Mbps
```

## 5.4 WiFi vs Ethernet

```
Ethernet (Cable)
Pros:
✓ Faster (no interference)
✓ More stable
✓ Lower latency (delay)

Cons:
✗ Need physical cable
✗ Less convenient

WiFi (Wireless)
Pros:
✓ Convenient (no cables)
✓ Mobile
✓ Easy setup

Cons:
✗ Slower than ethernet
✗ Can be unstable (interference)
✗ Slight delay

When to use each:
- Gaming/Video Call:    Ethernet (needs stable connection)
- Browsing/Email:       WiFi (fine for these)
- Downloading files:    Either (but ethernet faster)
```

---

# PART 6: INTERNET & WEB

## 6.1 Internet vs World Wide Web

**Internet:**
```
The actual network of computers worldwide
Like: The roads system
```

**World Wide Web (www):**
```
Websites and web pages on the internet
Like: Vehicles and signs on the roads system
```

**Other Things on Internet (Not Web):**
```
Email
Video streaming (Netflix, YouTube)
Video calling (Zoom, Skype)
Online games
Cloud storage
IoT (Smart home devices)
```

## 6.2 How Web Works

```
Step 1: You type URL in browser
        www.example.com
         ↓
Step 2: Browser sends request to find this website
         ↓
Step 3: DNS (like phone directory) looks up IP address
        example.com → 93.184.216.34
         ↓
Step 4: Browser connects to server at that IP
         ↓
Step 5: Server sends website files (HTML, CSS, images)
         ↓
Step 6: Browser displays website on screen
         ↓
Step 7: You interact with website
```

## 6.3 Web Browsers

**What they do:**
- Request websites from servers
- Translate HTML/CSS/JavaScript into visual pages
- Manage history, bookmarks, passwords
- Block malicious content

**Popular Browsers:**
```
Chrome:      Made by Google, most popular
Firefox:     Open-source, privacy-focused
Safari:      Made by Apple, for Mac
Edge:        Made by Microsoft
```

## 6.4 Websites vs Web Applications

**Static Website:**
```
Example: News article website

You visit → Website same for everyone
You refresh → Same content
It just displays information
```

**Web Application:**
```
Example: Gmail, Facebook, Google Docs

You visit → Website unique to YOU
Sign in → Your data loads
You can create/edit/delete things
Like desktop application but in browser
```

---

# PART 7: CYBERSECURITY ESSENTIALS

## 7.1 Common Threats

### **Malware**

```
Virus:
- Attaches to files
- Spreads when files shared
- Example: Email attachment with virus

Worm:
- Self-replicating
- Spreads via network
- Doesn't need user action

Trojan:
- Looks like legitimate software
- Hides malicious code
- Example: "Free video player" that steals data

Ransomware:
- Encrypts your files
- Demands payment to unlock
- Very dangerous for businesses

Spyware:
- Watches what you do
- Steals passwords, data
- Runs silently in background
```

### **Social Engineering**

```
Phishing:
You get email: "Verify your PayPal account (fake)"
You click link → Fake website
You enter password → Hacker has it!

Solution: Hover over links, check sender address

Pretexting:
Hacker calls: "I'm IT support, need your password"
You give it
Hacker gets access

Solution: Never give passwords to anyone

Password Sharing:
You share password with friend
Friend shares with someone else
10 people know your password now!

Solution: Use unique passwords
```

## 7.2 How to Stay Safe

### **1. Strong Passwords**

**Bad Passwords:**
```
123456
password
admin
YourName123
MyDog (people know your dog's name)
```

**Good Passwords:**
```
Tr0pic@lSunset42!Rain
May$20Coffee#Blue9Stars
K3y_Board$Hot@24Seven

Requirements for strong password:
✓ At least 12 characters
✓ Mix of uppercase and lowercase
✓ Numbers
✓ Special characters (!@#$%^&*)
✓ Not related to you personally
✓ Unique (different for each site)
```

### **2. Two-Factor Authentication (2FA)**

```
Old way (Weak):
1. Enter password
2. You're logged in

New way (Secure):
1. Enter password
2. Enter code from your phone (code changes every 30 seconds)
3. You're logged in

If hacker knows password, they can't login without your phone!
```

### **3. Antivirus Software**

```
What it does:
✓ Scans files for viruses
✓ Blocks malicious websites
✓ Monitors for suspicious activity
✓ Provides real-time protection

Good options:
- Windows Defender (built into Windows, free)
- Norton, McAfee (paid, comprehensive)
- Avast, AVG (free versions available)
```

### **4. Firewall**

```
What it does:
- Controls incoming/outgoing network traffic
- Blocks unauthorized access
- Like security guard for your computer

Windows has built-in firewall
Most routers have firewall built-in
```

### **5. Regular Updates**

```
Why software gets updates:
- Security patches (fix vulnerabilities)
- Bug fixes (problems discovered)
- New features (improvements)

When to update:
✓ Security updates: Immediately
✓ System updates: Soon (maybe wait a day)
✓ App updates: Within a week

Hackers love old software!
Outdated = known vulnerabilities
```

## 7.3 Safe Internet Habits

```
✓ DO:
- Use strong, unique passwords
- Enable 2FA on important accounts
- Keep software updated
- Be suspicious of emails from unknown people
- Use official apps (not weird alternatives)
- Back up important data
- Check website URL before entering data

✗ DON'T:
- Reuse passwords
- Click links in emails
- Download from suspicious websites
- Share personal information online
- Connect to public WiFi without VPN
- Leave computer unlocked unattended
- Tell people your passwords
- Open emails from strangers
```

---

# PART 8: DATA & DATABASES

## 8.1 What is Data?

**In Simple Terms:** Information stored in organized way.

```
Examples of data:
- Your name: "Alice"
- Your age: 25
- Your email: alice@example.com
- Bank transaction: $100 transferred
- Medical record: Blood type O+
```

## 8.2 Data Organization

### **Unorganized Data (Chaos)**

```
Computer files spread everywhere:
Desktop:
├── Budget.xlsx
├── Invoice.docx
├── Notes.txt
├── MyPhoto.jpg

Downloads:
├── AnotherBudget.xlsx
├── Invoice2.docx

Email:
├── Budget updated.xlsx
├── Latest invoice.pdf

Hard to find, easy to lose, confusing!
```

### **Organized Data (Database)**

```
Database structure:

Customers Table:
ID | Name   | Email              | Phone
1  | Alice  | alice@example.com  | 555-1234
2  | Bob    | bob@example.com    | 555-5678

Orders Table:
ID | CustomerID | Product      | Amount
1  | 1          | Laptop       | $800
2  | 2          | Mouse        | $25
3  | 1          | Keyboard     | $50

Easy to find, organized, searchable!
```

## 8.3 Types of Databases

### **1. SQL (Relational)**

```
Data in tables (like spreadsheet)
Tables can connect/relate to each other

Examples: MySQL, PostgreSQL, SQL Server, Oracle

Best for: Business data, structured information
```

### **2. NoSQL**

```
Data in documents (like JSON format)

Examples:
- MongoDB (document storage)
- Redis (key-value pairs)
- Neo4j (graph/relationships)
- Cassandra (wide columns)

Best for: Flexible data, social media, real-time
```

## 8.4 Cloud Storage

```
What is Cloud Storage?
- Your files on someone else's computer
- Accessible from anywhere with internet
- Synced across your devices

Examples:
- Google Drive (15 GB free)
- OneDrive (5 GB free)
- Dropbox (2 GB free)
- iCloud (5 GB free)

Advantages:
✓ Access from anywhere
✓ Automatic backup
✓ Share easily with others
✓ Don't lose files if computer fails

Disadvantages:
✗ Internet connection required
✗ Privacy concerns
✗ Monthly subscription for more storage
```

---

# PART 9: CLOUD COMPUTING

## 9.1 What is Cloud Computing?

**In Simple Terms:** Using computer resources (servers, storage, software) over the internet instead of owning them yourself.

```
Old Way (Buy Everything):
1. Buy expensive server
2. Set up in your office
3. Maintain 24/7
4. Pay electricity bills
5. Handle backups yourself
6. Risk data loss

Cloud Way:
1. Sign up for service
2. Use as much as needed
3. Provider handles everything
4. Pay monthly subscription
5. Automatic backups
6. Data is safe
```

## 9.2 Types of Cloud Services

### **1. IaaS (Infrastructure as a Service)**

```
Provider gives you: Computers to use (virtual servers)
You manage: Applications, data, security
Provider manages: Hardware, internet

Example: Amazon EC2, Google Cloud Compute
Like: Renting an empty office building
```

### **2. PaaS (Platform as a Service)**

```
Provider gives you: Hosting + development tools
You manage: Your application code
Provider manages: Everything else

Example: Heroku, Google App Engine
Like: Renting furnished office with utilities included
```

### **3. SaaS (Software as a Service)**

```
Provider gives you: Complete software application
You manage: Nothing (just use it)
Provider manages: Everything

Examples:
- Google Docs (word processor)
- Salesforce (business software)
- Slack (messaging)
- Netflix (video streaming)
- Zoom (video calls)

Like: Using Google Maps app (you use, Google maintains)
```

## 9.3 Major Cloud Providers

```
AWS (Amazon Web Services)
├─ Biggest market share: 32%
├─ Services: Everything
├─ Price: Expensive
└─ Learning curve: Steep

Azure (Microsoft)
├─ Market share: 23%
├─ Services: Everything
├─ Price: Reasonable
└─ Good with: Windows, Office 365

Google Cloud
├─ Market share: 10%
├─ Services: Everything
├─ Price: Reasonable
└─ Good at: Data, AI, Machine Learning
```

---

# PART 10: IT SUPPORT & TROUBLESHOOTING

## 10.1 Basic Troubleshooting

### **Principle: "Turn It Off and On Again"**

```
Why this works:
- Clears memory (RAM resets)
- Stops processes stuck in infinite loop
- Reloads drivers
- Fixes temporary glitches

95% of computer problems solved by restart!

How to restart properly:
1. Save all your work
2. Close all programs
3. Click Start → Power → Restart
4. Wait for restart to complete
5. Don't force restart (hold power button)
```

## 10.2 Common Problems & Solutions

### **Problem: Computer is Slow**

```
Check these things:

1. Is it a new slowness or always slow?
   New → Something changed
   Always → Normal for this computer

2. Look at CPU/Memory usage:
   Windows: Ctrl + Shift + Esc (Task Manager)
   
   If one program using 80% CPU → close it
   If overall 80% → too many programs open

3. Restart computer (clears RAM)

4. Check disk space:
   If less than 10% free → free up space (delete files)
   Computer gets slower when full

5. Check for malware:
   Run antivirus scan
```

### **Problem: Internet Not Working**

```
Troubleshooting steps:

1. Can you see WiFi network?
   No → Router problem
   Yes → Continue

2. Can you connect to WiFi?
   No → Try forgetting network and reconnecting
   Yes → Continue

3. Is internet actually down?
   Restart router (turn off 30 seconds, back on)

4. Check with other device:
   Other device works → Your device problem
   No devices work → Internet is down (ISP issue)

5. If router doesn't work:
   - Check cables are connected
   - Check WiFi is enabled
   - Restart router
   - Factory reset if stuck
```

### **Problem: File Deleted by Accident**

```
Quick action: Check Recycle Bin (Windows) or Trash (Mac)
If there: Right-click → Restore

If not there (emptied):
- Recently deleted: Recovery software might work
- Long time ago: Professional recovery (expensive)

Prevention: Regular backups!
```

### **Problem: Password Forgotten**

```
Windows Account:
1. Use password reset disk (if you made one)
2. Use email recovery
3. Use security questions

Gmail Account:
1. Click "Forgot password?"
2. Answer recovery email or phone
3. Reset password

Important: Keep recovery info updated!
```

## 10.3 Maintenance Tips

### **Daily**
```
✓ Shut down computer at end of day
✓ Don't leave it running unnecessary
✓ Back up important files
```

### **Weekly**
```
✓ Restart computer
✓ Check for Windows/app updates
✓ Clean desktop (delete unnecessary files)
```

### **Monthly**
```
✓ Update antivirus definitions
✓ Clean temporary files (CCleaner)
✓ Check available storage space
✓ Review installed programs (uninstall unused)
```

### **Quarterly**
```
✓ Full antivirus scan
✓ Disk cleanup
✓ Defragment HDD (if you have one, not SSD)
✓ Update BIOS/firmware
```

## 10.4 When to Call IT Support

```
You CAN handle:
- Computer is slow → restart, check programs
- WiFi down → restart router
- Forgot password → use recovery options
- File deleted → check trash
- Software problem → restart/reinstall

Call IT Support for:
- Don't know how to fix it
- Something broke that you didn't cause
- Security concerns
- Network problems affecting multiple people
- Hardware failure
- Need to set up new device
```

---

## 🎯 Quick Reference

### **File Size Chart**
```
1 KB = 1,000 bytes (text file)
1 MB = 1,000 KB (photo)
1 GB = 1,000 MB (movie or app)
1 TB = 1,000 GB (full backup)
```

### **Password Manager Recommendations**
```
Bitwarden      ✓ Free, secure
LastPass       ✓ Popular
1Password      ✓ Premium, excellent
KeePass        ✓ Local (no cloud)
```

### **VPN Services**
```
When to use: Public WiFi, privacy concerns
Popular: ExpressVPN, NordVPN, Proton VPN
```

### **Backup Strategy (3-2-1)**
```
3 copies of data:
- 1 on computer
- 2 on external drives/cloud

2 different types of storage:
- Cloud backup (Google Drive, Dropbox)
- External hard drive (plug in sometimes)

1 copy off-site:
- Cloud backup (safe if house burns down)
```

---

## 📚 Summary

**What You Now Know:**

1. ✓ How computer hardware works and what each part does
2. ✓ What software is and different types
3. ✓ How operating systems manage everything
4. ✓ How storage works and file organization
5. ✓ How networks and internet work
6. ✓ How websites and browsers work
7. ✓ How to stay safe online
8. ✓ What databases and cloud are
9. ✓ How to troubleshoot common problems
10. ✓ Basic IT maintenance

**Next Steps:**

- Experiment with computers (don't be afraid to break things)
- Learn one operating system well (Windows or Mac)
- Try Linux (free operating system, great for learning)
- Explore cloud services (try Google Drive, OneDrive)
- Build a home lab with old computers
- Help friends and family with their IT problems

---

**Last Updated:** May 2026
**Difficulty:** Beginner to Intermediate
**Estimated Time to Learn:** 2-4 weeks of casual reading

Good luck! You're now an IT Fundamentals expert! 🎉
