# Knowledge Base — Common Technology Issues Self-Help Guide

This document served as the knowledge foundation for the Helpdesk AI assistant. It was loaded into the Claude Project alongside the system prompt to give the assistant accurate, structured reference material for the most common IT issues employees encounter.

The guide is written for non-technical users -- plain language, step-by-step format, with clear escalation signals built into each section. This mirrors the assistant's own communication approach and ensures consistent guidance whether a user is reading this doc directly or interacting with the assistant.

---

# Common Technology Issues - Self-Help Guide

## 📖 How to Use This Guide

This guide helps you solve common tech problems yourself. Each section starts with simple fixes anyone can try, and tells you clearly when it's time to contact IT for help.

**Quick Navigation:**
- 📧 Email Issues
- 🌐 Internet/WiFi Problems
- 🖨️ Printer Not Working
- 🔑 Password & Login Issues
- 📁 Can't Access Files/Folders
- 🐌 Slow Computer Performance
- 📱 Mobile Device Problems
- 💻 Software Won't Open/Crashes
- 🔌 Hardware Problems
- 🚨 When to Contact IT Immediately
- 📞 How to Write a Great IT Ticket
- 💡 Prevention Tips

---

## 📧 EMAIL ISSUES

### Problem: "I can't send or receive email"

**Try these steps in order:**

**Step 1: Check your internet connection**
- Can you open a website like google.com?
- If NO → Jump to "Internet Not Working" section below
- If YES → Continue to Step 2

**Step 2: Close and reopen your email app completely**
- Don't just minimize it - fully close it
- Wait 10 seconds
- Open it again
- Try sending a test email to yourself

**Why this works**: Email apps sometimes lose their connection to the server. Closing completely forces a fresh connection.

**Step 3: Is it just one email or all emails?**
- **Can't send ONE specific email** → That email might have an issue:
  - Attachment too large? (Most systems limit to 25MB)
  - Email address typed wrong?
  - Try sending without attachments
- **Can't send ANY emails** → Continue to Step 4

**Step 4: Restart your device**
- **Laptop/Desktop**: Click Start menu → Power → Restart (not Shut Down)
- **Phone/Tablet**: Hold power button until you see Restart option
- **Wait**: Give it 2-3 minutes to fully restart and reconnect

**Why this works**: Clears temporary glitches in your email connection and network settings.

**Step 5: Test on a different device**
- Try accessing your email on your phone, or webmail on a different computer
- **Works on other device?** → Problem is specific to your main device (contact IT)
- **Doesn't work anywhere?** → Might be an account or server issue (contact IT)

**⚠️ CONTACT IT IF:**
- You've restarted but still can't send/receive after 15 minutes
- Error messages appear that you don't understand
- Email worked yesterday but suddenly stopped today
- Multiple coworkers are having the same problem at the same time

**What to tell IT:**
"My email isn't working. I can/cannot access the internet on other sites. I've restarted my [device type]. The error message says: '[exact words]'. This started: [when - date and time]."

---

### Problem: "I can't find an email I know I received"

**Check these locations first:**

**1. Search for it**
- Click the search box at the top of your email window
- Type the sender's name OR a unique word from the subject line
- Look through all the results - it might be in a folder you didn't expect

**2. Check these folders:**
- **Deleted Items / Trash** - You or someone else might have deleted it
- **Junk / Spam** - Emails from new senders often land here automatically
- **Archive** - Some people archive instead of delete
- **Any custom folders** - You or email rules might have moved it automatically

**3. Check the date range in your view**
- Some email views only show "last 30 days" or "this week"
- Look for date filter options to expand the range

**4. If you share your mailbox with others**
- A colleague might have moved or deleted it
- Check with them before assuming it's lost

**5. Search your Sent folder**
- Maybe you sent it but didn't receive it? Worth checking if you're confused about direction

**🔴 URGENT - CONTACT IT IMMEDIATELY IF:**
Important emails are missing AND:
- You definitely didn't delete them yourself
- They're not in trash, spam, or any other folder
- They contained sensitive client information or financial data
- Multiple emails disappeared at once
- You suspect your account was compromised

**What to tell IT:**
"I'm missing emails from [date range] from [sender]. I've checked all folders including trash and spam. Last time I saw it was [when]. I need to recover: [brief description of content and why it's important]."

---

### Problem: "Email keeps crashing when I open it"

**Try these fixes:**

**Step 1: Does it crash immediately or when you do something specific?**
- **Crashes on open** → Might be a corrupted setting
- **Crashes when opening specific email** → That email might be corrupted
- **Crashes when typing** → Might be add-in conflict

**Step 2: Start in Safe Mode** (disables add-ins temporarily)

**For Outlook on Windows:**
1. Close Outlook completely
2. Press Windows key + R
3. Type: `outlook.exe /safe`
4. Press Enter

**Does it work in Safe Mode?**
- **YES** → An add-in is causing the problem (contact IT to identify which one)
- **NO** → Continue to Step 3

**Step 3: Clear email cache**

**Outlook:**
1. Close Outlook
2. Press Windows key + R
3. Type: `%localappdata%\Microsoft\Outlook`
4. Delete files that end in `.ost` (these will rebuild automatically)
5. Restart Outlook (will take 5-10 minutes to re-sync)

**Step 4: Repair Office installation**

**Windows:**
1. Settings → Apps → Microsoft Office → Modify
2. Choose "Quick Repair" first
3. If that doesn't work, try "Online Repair" (requires internet, takes longer)

**⚠️ CONTACT IT IF:**
- Safe Mode didn't help
- You're not comfortable deleting cache files
- Crashes started after a recent update
- You need your email working urgently (they can rebuild your profile faster)

---

## 🌐 INTERNET / WIFI ISSUES

### Problem: "I can't connect to the internet"

**Quick diagnostic steps:**

**Step 1: Are you connected to WiFi or Ethernet?**

**Check your connection icon:**
- **Windows**: Bottom-right corner of screen
- **Mac**: Top-right corner of screen
- **Symbols**:
  - 📶 Bars = WiFi connected
  - 🌐 Globe = Ethernet connected
  - ❌ Red X or ⚠️ = Not connected

**Not connected?** → Click the icon and select your office network

**Step 2: The Airplane Mode trick**
This forces your device to make a fresh connection:

**On Phones/Tablets:**
1. Swipe down from top of screen
2. Tap Airplane Mode icon (✈️) to turn it ON
3. Wait 10 seconds
4. Tap again to turn it OFF

**On Laptops:**
1. Click WiFi icon
2. Turn WiFi OFF
3. Wait 10 seconds
4. Turn WiFi ON

**Why this works**: Clears corrupted network settings and forces your device to reconnect fresh.

**Step 3: Restart your device**
- This fixes about 70% of connection issues
- Do a full restart from the Start/Power menu (not just closing the lid)

**Step 4: Check if others have internet**
- Ask a nearby coworker if their internet is working
- **Just you?** → Problem is your device (continue troubleshooting)
- **Everyone affected?** → Network outage (contact IT immediately)

**Step 5: Move closer to WiFi access point** (if in office)
- WiFi signal weakens through walls and with distance
- Try a conference room or different area
- If this helps, you might need a WiFi extender in your area (let IT know)

**Step 6: Forget and reconnect to WiFi**

**Windows:**
1. Click Start → Settings → Network & Internet
2. Click WiFi → Manage Known Networks
3. Click your office network → Forget
4. Click WiFi icon in taskbar → Your network name
5. Enter password as if connecting for first time

**Mac:**
1. Click  → System Preferences → Network
2. Select WiFi → Advanced
3. Find your office network in the list
4. Click it → Click the minus (-) button → OK
5. Click WiFi icon in menu bar → Join your network
6. Enter password

**⚠️ CONTACT IT IF:**
- Restart didn't fix it after 10 minutes
- Only your device is affected (others can connect fine)
- You're in the office but can't see or connect to the office WiFi network
- You don't have the WiFi password
- Internet is extremely slow (takes 30+ seconds to load a simple webpage)
- You can connect but get "No Internet Access" message

**What to tell IT:**
"I can't connect to [network name]. I'm located at [office/location]. I've tried restarting and the airplane mode trick. Other people can/cannot connect. Error message: [exact words]."

---

### Problem: "Internet is connected but really slow"

**Troubleshooting steps:**

**Step 1: Test your speed**
- Go to fast.com or speedtest.net
- Run a test
- **Normal office speeds**: 50+ Mbps download
- **If under 10 Mbps**: Something is wrong

**Step 2: Is it just you or everyone?**
- Ask coworkers to test their speed
- **Just you?** → Problem with your device or connection
- **Everyone?** → Network issue (contact IT)

**Step 3: Check what's running on your device**

**Windows - Check Task Manager:**
1. Press Ctrl + Shift + Esc
2. Click "More details" if needed
3. Click "Network" column to sort by network usage
4. Look for programs using a lot of bandwidth

**Mac - Check Activity Monitor:**
1. Spotlight search (Cmd + Space) → Type "Activity Monitor"
2. Click "Network" tab
3. Sort by "Sent Bytes" or "Received Bytes"

**Common bandwidth hogs:**
- Video streaming (YouTube, Netflix)
- Video calls (Zoom, Teams)
- Large file downloads/uploads
- Cloud backup services syncing
- System updates downloading

**Step 4: Close bandwidth-heavy programs you're not using**
- Save your work first
- Close streaming, large downloads, backup syncs
- Try your work again

**Step 5: Try Ethernet cable** (if available)
- Ethernet is faster and more stable than WiFi
- If Ethernet works fine but WiFi is slow → WiFi issue (contact IT)

**Step 6: Restart your computer**
- Clears network cache and connections

**⚠️ CONTACT IT IF:**
- Slow speeds persist for multiple days
- Only slow at certain times (pattern indicates network capacity issue)
- Ethernet also slow (not just WiFi)
- Speed test shows much slower than expected for your location

---

## 🖨️ PRINTER ISSUES

### Problem: "The printer won't print"

**Before you troubleshoot, check the obvious:**

**Physical checks:**
1. **Is the printer turned on?** Look for lights/display
2. **Is there paper in the tray?** Check the input tray
3. **Does the printer display show an error?** Write down the exact error message
4. **Is it connected?**
   - Wired: Cable plugged into printer AND computer/network
   - Wireless: WiFi indicator light should be on

**Step 1: Is it just you or everyone?**
- Ask coworkers if they can print to the same printer
- **Just you?** → Problem is your computer's connection to the printer (continue below)
- **Nobody can print?** → Problem is the printer itself (skip to Step 4)

**Step 2: Check if your print job is stuck**

**Windows:**
1. Click Start → Settings → Devices → Printers & Scanners
2. Click your printer name
3. Click "Open queue"
4. See old jobs stuck there?
5. Select all jobs → Right-click → Cancel

**Mac:**
1. Click  → System Preferences → Printers & Scanners
2. Click your printer
3. Click "Open Print Queue"
4. Select stuck jobs → Click X to delete them

**Why this works**: One stuck print job blocks everything behind it, like a clog in a pipe.

**Step 3: Restart your computer**
- Clears the print queue and resets the connection to the printer
- After restart, try printing a test page

**Step 4: Restart the printer**
1. Press and hold the power button until printer turns completely off
2. OR unplug the power cable from the back
3. Wait 30 seconds
4. Turn back on or plug back in
5. Wait 2 minutes for printer to fully wake up
6. Try printing again

**Step 5: Print a test page from the printer itself**
- Most printers have a button/menu option to print a test page
- **YES prints** → Printer is fine; issue is computer-to-printer connection (continue to Step 6)
- **NO print** → Hardware problem with printer (contact IT)

**Step 6: Remove and re-add the printer on your computer**

**Windows:**
1. Settings → Devices → Printers & Scanners
2. Click the printer → Remove device
3. Click "Add a printer or scanner"
4. Wait for it to appear → Click it → Add device

**Mac:**
1. System Preferences → Printers & Scanners
2. Click the printer → Click minus (-) button to remove
3. Click plus (+) button to add it back

**⚠️ CONTACT IT IF:**
- Paper is jammed inside the printer (don't force it out)
- Printer displays error codes you don't understand
- Toner/ink low warning (they'll order/replace)
- You've tried all steps but still can't print
- Printer prints but pages are blank, smudged, or faded
- Multiple people cannot print to the same printer

**What to tell IT:**
"I can't print to [printer name or location]. The printer is/isn't showing an error message: [exact message]. I've restarted my computer and the printer. Other people can/cannot print to it."

---

## 🔑 PASSWORD & LOGIN ISSUES

### Problem: "I forgot my password"

**Self-service password reset (if available):**

1. On the login screen, look for "Forgot Password" or "Reset Password" link
2. Click it and follow the prompts
3. Usually requires answering security questions OR a verification code sent to your email or phone
4. Create a new password following the requirements shown

**Creating a strong password:**
- **Length**: At least 12 characters
- **Mix**: Uppercase, lowercase, numbers, symbols
- **Avoid**: Dictionary words, personal info (birthday, pet names, family names)
- **Good example**: `Coffee!Helps@Me-Think2024`
- **Even better**: Use a passphrase like `Purple-Elephants-Dance-Everywhere-7!`

**⚠️ CONTACT IT IF:**
- There's no "Forgot Password" option on your login screen
- The password reset link doesn't work or times out
- You don't have access to the recovery email or phone number on file
- Your account is locked after too many wrong password attempts

---

### Problem: "I can't log into my computer"

**Step 1: Check Caps Lock**
- Passwords are case-sensitive
- Look for Caps Lock indicator light on your keyboard
- Press Caps Lock to turn it off if it's on

**Step 2: Verify you're typing the correct password**
- If you recently changed your password, are you using the new one or the old one?

**Step 3: Are you connected to the network?**
- In the office: Check ethernet or WiFi
- Remote: Make sure VPN is connected first

**Step 4: Is your account locked?**
Common locked account messages:
- "Account is locked out"
- "Too many failed login attempts"
- "Account disabled"

Contact IT immediately -- they can unlock it in 5-10 minutes.

**🔴 CONTACT IT URGENTLY IF:**
- Message says your password is incorrect but you're certain it's right
- "Account disabled" or "Account expired" message
- You're at a client site or traveling and can't log in

---

### Problem: "System says I need to change my password"

**This is normal -- most companies require regular password changes.**

1. Enter your current password in the first field
2. Create a new password following the rules shown
3. Confirm by typing it again exactly
4. Save it securely or in a password manager

**Tips:**
- Don't just add "1" to the end of your old password
- Don't use predictable patterns like "Summer2024" → "Fall2024"
- Use a passphrase: `ILove2DrinkCoffee@Work!`

---

## 📁 FILE ACCESS ISSUES

### Problem: "I can't access a shared folder or network drive"

**Step 1: Are you on the company network?**
- In the office: Connected to office WiFi or ethernet?
- Remote: Is your VPN connected?

**Step 2: Do you have permission to access this folder?**
- Try accessing a different shared folder you know you have access to
- **Other folder works?** → You may not have permission to the first folder
- **Nothing works?** → Network connection issue

**Step 3: Restart your computer**
- Refreshes network connections and reloads security group memberships

**Step 4: Try accessing via direct path**

**Windows:**
1. Open File Explorer
2. Click in the address bar
3. Type: `\\servername\foldername`
4. Press Enter

**Mac:**
1. Open Finder
2. Press Cmd + K
3. Type: `smb://servername/foldername`
4. Click Connect

**⚠️ CONTACT IT IF:**
- You should have access but get "Access Denied"
- You had access yesterday but not today
- Error says "Network path not found"
- VPN is connected but you still can't access internal resources
- You need access granted to a new folder

---

## 🐌 SLOW COMPUTER PERFORMANCE

### Problem: "My computer is running really slow"

**Step 1: Restart your computer**
- Restart at least once a week
- Choose "Restart" not "Shut Down" -- Restart does a deeper refresh

**Step 2: Close programs you're not using**
- Close browser tabs you don't need
- Close applications you're finished with -- don't just minimize

**Step 3: Check if something is updating in the background**
- Windows Update often downloads automatically
- Antivirus scans run periodically
- Give it 20-30 minutes if updates are running

**Step 4: Check what's using your resources**

**Windows - Task Manager:**
1. Press Ctrl + Shift + Esc
2. Look at CPU, Memory, and Disk columns
3. Sort to find what's using the most

**Mac - Activity Monitor:**
1. Spotlight Search → "Activity Monitor"
2. Check CPU and Memory tabs
3. Memory Pressure at bottom should be green, not red

**Step 5: Free up disk space**
Your computer needs at least 15% free space to work efficiently.

**Windows:**
- Empty Recycle Bin
- Clean Downloads folder
- Use Disk Cleanup (search in Start menu)

**Mac:**
- Empty Trash
- Clean Downloads folder
- Check About This Mac → Storage → Manage

**⚠️ CONTACT IT IF:**
- Computer suddenly much slower than normal
- Slowness persists for several days after restarts
- Disk stuck at 100% usage constantly
- Unusual programs running that you don't recognize

---

## 📱 MOBILE DEVICE ISSUES

### Problem: "My work email won't sync on my phone"

**Step 1: Check internet connection**
- Can you browse websites?

**Step 2: Force a manual sync**
- Pull down to refresh in your email list

**Step 3: Check storage space**
If your phone is full, email can't download new messages:
- Need at least 1-2 GB free

**Step 4: Restart your phone**

**Step 5: Remove and re-add your work email account**
Write down your server settings before removing -- you'll need them to re-add.

**⚠️ CONTACT IT IF:**
- You don't know your email server settings
- Phone says "Cannot connect to server" or "Authentication failed"
- Email worked fine until a specific date

---

## 💻 SOFTWARE WON'T OPEN OR KEEPS CRASHING

### Problem: "Program keeps crashing or freezing"

**Step 1: Check for updates**
- Bugs are often fixed in newer versions
- Help menu → Check for Updates

**Step 2: Restart your computer**

**Step 3: Repair the program installation**

**Windows:**
1. Settings → Apps → Apps & features
2. Find the program → Modify or Repair

**Mac:**
1. Delete the app
2. Reinstall fresh from official source

**⚠️ CONTACT IT IF:**
- Crashes started after a recent Windows/macOS update
- Program crashes only on your computer
- Critical work program you can't do your job without
- Blue Screen of Death appears

---

## 🔌 HARDWARE PROBLEMS

### Problem: "Mouse or keyboard not working"

**Wired:**
- Unplug and try a different USB port
- Check for bent pins or debris in connector
- Restart computer

**Wireless:**
- Replace batteries first -- most wireless issues are just low battery
- Unplug and replug the USB receiver
- Try re-pairing if device has a pairing button

**Bluetooth:**
- Check Bluetooth is turned on
- Remove and re-pair the device

---

### Problem: "Laptop won't turn on or charge"

**Step 1: Check power connection**
- Power brick plugged into working outlet?
- Cable firmly connected to laptop?

**Step 2: Hard reset**
1. Unplug power cable
2. Remove battery (if removable)
3. Hold power button for 30 seconds
4. Reconnect everything
5. Try powering on

**⚠️ CONTACT IT IMMEDIATELY IF:**
- Laptop won't turn on at all
- You smell burning or see smoke
- Battery is swollen or bulging (DO NOT USE -- safety hazard)

---

## 🚨 WHEN TO CONTACT IT IMMEDIATELY

**These situations require immediate IT intervention. Don't troubleshoot yourself.**

### Security Issues

Contact IT right away if you experience:
- Suspicious emails asking for passwords or requesting unusual financial actions
- Fake virus warnings or popups that won't close
- Message saying "Your files are encrypted -- pay ransom"
- Password changed and you didn't change it
- Emails in your Sent folder you didn't send
- Lost or stolen device with company data

**What to do:**
- STOP using the device immediately
- Don't click anything in suspicious messages
- Don't enter any passwords
- Call IT using your emergency contact method
- Take screenshots if possible

### Data Emergencies

- Critical files missing or deleted that you didn't remove
- Multiple files corrupted simultaneously
- Can't access critical system before an important deadline

### System Completely Down

- Blue Screen of Death (Windows)
- Kernel Panic (Mac)
- Won't boot at all
- Repeated crashes every few minutes

### Office-Wide Issues

- Nobody in office can access internet
- Main company application down for multiple people
- Power outage or building emergency affecting systems

---

## 📞 HOW TO CREATE A GREAT IT TICKET

**The better information you provide upfront, the faster IT can help.**

### Essential Information to Include

**WHO you are:** Full name, department, location, phone number

**WHAT the problem is -- be specific:**
- ❌ "My computer doesn't work"
- ✅ "My laptop won't turn on even when plugged in"

**WHEN it started:** Specific date and time if possible

**WHAT you've already tried:** List troubleshooting steps and results

**ERROR messages:** Exact wording, copy/paste if possible, screenshot if you have one

**URGENCY level:**
- CRITICAL: Can't do your job, blocking others, security issue
- HIGH: Major workaround needed, deadline approaching
- MEDIUM: Inconvenient but have a workaround
- LOW: Minor annoyance, no immediate impact

---

### Example of a great IT ticket:

```
SUBJECT: [URGENT] Laptop won't turn on - Presentation in 3 hours

NAME: Jordan Smith
DEPARTMENT: Sales
LOCATION: Office - 3rd Floor
PHONE: x5678

ISSUE:
My laptop won't turn on at all. When I press the power button, nothing happens -- no lights, no sounds, no display.

WHEN IT STARTED:
This morning at 8:30am. Worked fine Friday afternoon.

WHAT I'VE TRIED:
- Confirmed power adapter is plugged into working outlet
- Tried different outlets
- Power adapter LED is on (glowing green)
- Held power button for 30 seconds (hard reset)
- Tried powering on without battery

ERROR MESSAGES: None -- completely unresponsive

URGENCY: CRITICAL
Client presentation at 11:30am today. Presentation file is on this laptop.

WHAT I NEED:
Either get this laptop working OR access to the file on a loaner laptop ASAP
```

---

## 💡 PREVENTION TIPS

### Daily Habits
- Save your work every 10-15 minutes
- Lock your computer when stepping away (Windows: Win+L / Mac: Ctrl+Cmd+Q)
- Close apps you're not using

### Weekly Habits
- Restart your computer at least once
- Clear browser cache and cookies
- Empty trash/recycle bin

### Always Do
- Use strong, unique passwords for each account
- Enable multi-factor authentication (MFA) where available
- Think before you click -- hover over links to see the real destination
- Report issues early -- small problems become big problems
- Keep software updated

### Never Do
- Share your password with anyone (real IT will never ask for it)
- Click links in suspicious emails
- Download unauthorized software
- Disable antivirus or firewall
- Ignore security warnings

---

**Last Updated**: 2026-03-16
**Questions about this guide?** Contact IT or your department manager.
