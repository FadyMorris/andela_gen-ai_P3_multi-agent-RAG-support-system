# 1. Password Reset Procedures

## 1.1 Standard Password Reset
Employees can reset their passwords through the self-service portal at https://portal.company.com/reset. The process requires:
- Valid employee email address
- Two-factor authentication via mobile device
- Answer to security questions (minimum 2 of 3)
- Password must meet complexity requirements: 12+ characters, uppercase, lowercase, numbers, and special characters

## 1.2 Emergency Password Reset
For locked accounts requiring immediate access, contact IT support at ext. 5555. Emergency resets require:
- Manager approval via email
- Verification of employee ID number
- Temporary password valid for 24 hours
- Mandatory password change on first login

## 1.3 Password Policy Requirements
All company passwords must adhere to:
- Minimum length: 12 characters
- Must include: uppercase letters, lowercase letters, numbers, special characters
- Cannot reuse last 10 passwords
- Expires every 90 days
- Maximum 3 failed attempts before lockout
- Cannot contain username or common dictionary words

---

# 2. VPN Access and Configuration

## 2.1 VPN Installation Process
To install company VPN (Cisco AnyConnect):
1. Navigate to https://vpn.company.com
2. Download the appropriate client for your OS (Windows/Mac/Linux)
3. Run installer with administrator privileges
4. Enter company credentials when prompted
5. Configure split-tunneling if approved by security team

## 2.2 VPN Connection Troubleshooting
Common VPN issues and solutions:
- **Error: "Connection timeout"** - Check firewall settings, ensure ports 443 and 10000 are open
- **Error: "Authentication failed"** - Verify credentials, check if account is locked
- **Error: "Certificate error"** - Download latest certificate from IT portal, import to system keychain
- **Slow connection** - Switch VPN server (US-East, US-West, EU-Central available)

## 2.3 VPN Best Practices
- Always connect to VPN when accessing company resources remotely
- Disconnect when not in use to free up licenses
- Report connection drops immediately to IT
- Use nearest geographic server for optimal performance
- Never share VPN credentials

---

# 3. Email Configuration and Issues

## 3.1 Outlook Configuration
Setting up Microsoft Outlook for company email:
- **Server**: mail.company.com
- **Port**: 993 (IMAP) or 587 (SMTP)
- **Encryption**: SSL/TLS required
- **Authentication**: OAuth 2.0 with company credentials
- **Archive settings**: Auto-archive emails older than 1 year

## 3.2 Common Email Problems
**Problem: Emails not sending**
- Check outbox for stuck messages
- Verify internet connection
- Ensure mailbox not over quota (limit: 50GB)
- Clear Outlook cache: File > Options > Advanced > Outlook Data File Settings

**Problem: Not receiving emails**
- Check spam/junk folder
- Verify forwarding rules not redirecting mail
- Confirm sender not blocked
- Check inbox rules for auto-delete conditions

## 3.3 Email Security Guidelines
- Never open attachments from unknown senders
- Verify sender email address matches known contacts
- Report phishing attempts to security@company.com
- Use encrypted email for sensitive information
- Enable multi-factor authentication for email access

---

# 4. Laptop and Desktop Hardware Support

## 4.1 Standard Hardware Specifications
**Approved Laptop Models:**
- Dell Latitude 5420: 16GB RAM, 512GB SSD, Intel i7
- Lenovo ThinkPad X1: 16GB RAM, 1TB SSD, Intel i7
- MacBook Pro 14": 16GB RAM, 512GB SSD, M2 chip

**Standard Desktop Configuration:**
- Dell OptiPlex 7090: 32GB RAM, 1TB SSD, Intel i7
- Dual 27" monitors (Dell P2722H)
- Wired keyboard and mouse
- Docking station for laptops

## 4.2 Hardware Replacement Process
To request hardware replacement:
1. Submit ticket via IT portal with asset tag number
2. Describe issue in detail with error messages
3. Attach photos of physical damage if applicable
4. Backup all data before replacement
5. Standard turnaround: 3-5 business days
6. Loaner equipment available for critical roles

## 4.3 Preventive Maintenance
Monthly maintenance tasks:
- Clean dust from vents and fans
- Check for Windows/macOS updates
- Run disk cleanup utilities
- Verify backup completion
- Test battery health (laptops)
- Update antivirus definitions

---

# 5. Software Installation and Licensing

## 5.1 Approved Software List
Employees can install the following without approval:
- Microsoft Office 365 Suite
- Zoom (latest version)
- Slack Desktop App
- Google Chrome, Mozilla Firefox
- Adobe Acrobat Reader
- 7-Zip or WinRAR

## 5.2 Software Request Process
For software not on approved list:
1. Submit request via ServiceNow portal
2. Provide business justification
3. Include cost estimate and licensing model
4. Manager approval required for purchases over $100
5. Security review (5-7 business days)
6. Installation scheduled after approval

## 5.3 License Management
- All software licenses tracked in IT asset management system
- License compliance audits quarterly
- Report unused licenses for reassignment
- Notify IT within 24 hours of employee departure
- Licenses reclaimed within 48 hours of termination

---

# 6. Network Connectivity Issues

## 6.1 WiFi Troubleshooting Steps
**Cannot connect to corporate WiFi:**
1. Verify WiFi enabled on device
2. Select correct network: "CompanySecure"
3. Enter domain credentials: DOMAIN\username
4. Check for IP address assignment (ipconfig/ifconfig)
5. Flush DNS cache: ipconfig /flushdns (Windows) or sudo dscacheutil -flushcache (Mac)
6. Forget network and reconnect

## 6.2 Ethernet Connection Issues
**No network connection via Ethernet:**
- Check cable connections at both ends
- Try different Ethernet port on switch/wall
- Verify link lights on network adapter
- Update network adapter drivers
- Check for IP conflicts: ipconfig /release then ipconfig /renew
- Disable and re-enable network adapter

## 6.3 Network Performance Optimization
To improve network speed:
- Close unnecessary applications consuming bandwidth
- Disable automatic cloud sync during business hours
- Use wired connection for large file transfers
- Clear browser cache and cookies
- Disable VPN when accessing local resources
- Run speed test: https://speedtest.company.com

---

# 7. Printer Setup and Troubleshooting

## 7.1 Network Printer Installation
Adding network printers:
1. Open Devices and Printers in Control Panel
2. Click "Add a printer"
3. Select "Add a network printer"
4. Enter printer path: \\printserver\PrinterName
5. Install drivers when prompted
6. Set as default if primary printer

## 7.2 Common Printer Problems
**Print jobs stuck in queue:**
- Open print queue, cancel all documents
- Restart print spooler service
- Delete printer and re-add
- Check printer network connectivity
- Verify printer has paper and toner

**Poor print quality:**
- Clean printer heads (maintenance menu)
- Replace toner/ink cartridges
- Check paper quality and type settings
- Run printer calibration utility
- Update printer firmware

## 7.3 Print Quotas and Policies
- Each employee allocated 500 pages/month
- Color printing: 100 pages/month
- Excess printing requires manager approval
- Track usage: https://printmanager.company.com
- Secure printing enabled: requires badge swipe at printer

---

# 8. Mobile Device Management (MDM)

## 8.1 Enrolling Mobile Devices
To enroll smartphone/tablet in MDM:
1. Download Microsoft Intune Company Portal
2. Sign in with company credentials
3. Accept device management policies
4. Install required certificates
5. Configure email and calendar sync
6. Enable device encryption

## 8.2 Mobile Device Policies
Required security settings:
- PIN/biometric lock required (6+ digits)
- Auto-lock after 2 minutes inactivity
- Remote wipe enabled
- Encrypted storage mandatory
- Jailbroken/rooted devices not permitted
- Regular OS updates required

## 8.3 BYOD (Bring Your Own Device) Guidelines
Personal devices accessing company data must:
- Enroll in MDM system
- Maintain separate work profile/container
- Accept remote wipe of work data only
- Install company security apps
- Pass quarterly security scans
- Report lost/stolen devices within 2 hours

---

# 9. Cloud Storage and File Sharing

## 9.1 OneDrive Configuration
Company OneDrive setup:
- Storage allocation: 1TB per user
- Desktop sync enabled automatically
- Files On-Demand feature activated
- Backup folders: Desktop, Documents, Pictures
- Sync conflicts resolved via version history
- Share links expire after 30 days

## 9.2 SharePoint Access
Accessing team SharePoint sites:
- Navigate to https://company.sharepoint.com
- Sites accessible based on group membership
- Request access via site owner
- External sharing requires approval
- Maximum file size: 15GB
- Version history retained for 60 days

## 9.3 File Sharing Best Practices
- Use SharePoint for team collaboration
- OneDrive for personal work files
- Never use personal cloud storage (Dropbox, Google Drive)
- Set appropriate permissions (view/edit/full control)
- Remove access when project completes
- Use password protection for sensitive shares

---

# 10. Video Conferencing Support

## 10.1 Zoom Configuration
Company Zoom settings:
- Sign in via SSO: company.zoom.us
- Enable waiting room for security
- Use virtual backgrounds (approved templates)
- Record to cloud (auto-delete after 30 days)
- Screen sharing restricted to host/co-host
- Enable closed captions

## 10.2 Meeting Room Equipment
Conference room technology:
- Poly Studio cameras and microphones
- Logitech Tap room controllers
- Wireless HDMI presentation (ClickShare)
- Scheduling via Outlook room calendars
- Report issues via room email: roomname@company.com
- Reset room system: press power button 10 seconds

## 10.3 Video Quality Troubleshooting
**Poor video/audio quality:**
- Close bandwidth-intensive applications
- Use wired connection instead of WiFi
- Disable HD video in Zoom settings
- Mute when not speaking
- Check microphone/camera permissions
- Update Zoom to latest version

---

# 11. Multi-Factor Authentication (MFA)

## 11.1 MFA Enrollment
Setting up MFA:
1. Visit https://mfa.company.com
2. Download Microsoft Authenticator app
3. Scan QR code with app
4. Enter verification code
5. Add backup phone number
6. Save backup codes securely

## 11.2 MFA Device Management
Managing authentication devices:
- Maximum 3 devices per user
- Remove lost devices immediately
- Primary device required for sensitive operations
- Backup methods: SMS, phone call, hardware token
- Replace hardware tokens every 2 years
- Update phone number changes within 24 hours

## 11.3 MFA Troubleshooting
**Cannot receive MFA codes:**
- Check device time sync (must be accurate)
- Verify phone number registered correctly
- Try backup authentication method
- Use backup codes (one-time use)
- Contact IT for MFA reset (requires manager approval)
- Re-enroll device after reset

---

# 12. Antivirus and Endpoint Protection

## 12.1 Corporate Antivirus (Crowdstrike)
Company endpoint protection:
- Installed automatically via policy
- Real-time scanning always enabled
- Weekly full system scans (scheduled)
- Quarantine notifications sent to IT
- Cannot disable without admin password
- Auto-updates daily

## 12.2 Responding to Security Alerts
If antivirus detects threat:
1. Do not dismiss alert
2. Note filename and location
3. Disconnect from network immediately
4. Contact IT Security: ext. 5500
5. Do not attempt to remove manually
6. Allow IT remote access for remediation

## 12.3 Safe Computing Practices
- Don't download files from untrusted sources
- Verify URL before clicking links
- Use company VPN on public WiFi
- Lock computer when leaving desk (Win+L or Cmd+Ctrl+Q)
- Report suspicious emails to security@company.com
- Never disable antivirus software

---

# 13. Data Backup and Recovery

## 13.1 Automatic Backup Systems
Company backup strategy:
- OneDrive: continuous sync backup
- Local files: daily backup to network storage
- Email: backed up to compliance archive
- Retention: 90 days online, 7 years archive
- Backup verification: weekly automated tests

## 13.2 File Recovery Process
To restore deleted/corrupted files:
1. Check OneDrive version history
2. Submit recovery request via IT portal
3. Specify file path and approximate date
4. Recovery SLA: 24-48 hours
5. Large recoveries may take longer
6. Test restored files before confirming

## 13.3 Disaster Recovery Procedures
In case of data loss:
- Immediately stop using affected device
- Do not attempt personal recovery
- Contact IT immediately: ext. 5555
- Preserve any error messages/logs
- Document actions taken before failure
- Follow IT instructions for recovery

---

# 14. Remote Desktop Access

## 14.1 Setting Up Remote Desktop
Accessing work computer remotely:
1. Enable Remote Desktop on work PC
2. Note computer name (found in System Properties)
3. Connect via VPN first
4. Use Remote Desktop Connection app
5. Enter: computername.company.com
6. Authenticate with domain credentials

## 14.2 Remote Access Troubleshooting
**Cannot connect via Remote Desktop:**
- Verify VPN connection active
- Confirm work computer powered on
- Check Remote Desktop enabled
- Verify firewall not blocking port 3389
- Try alternative: Remote Assistance
- Use web-based access: https://remote.company.com

## 14.3 Remote Access Security
- Always disconnect sessions when finished
- Never save passwords on personal devices
- Use complex passwords for remote access
- Enable network level authentication
- Report suspicious remote access activity
- Review access logs monthly

---

# 15. Browser Issues and Configuration

## 15.1 Supported Browsers
Company-approved browsers:
- Google Chrome (primary, latest version)
- Microsoft Edge (Chromium-based)
- Mozilla Firefox ESR
- Internet Explorer 11 (legacy apps only)

## 15.2 Browser Troubleshooting
**Websites not loading:**
- Clear cache and cookies: Ctrl+Shift+Delete
- Disable browser extensions
- Try incognito/private mode
- Check proxy settings: Auto-detect
- Reset browser to defaults
- Try different browser

**Performance issues:**
- Limit open tabs (recommend <10)
- Disable unnecessary extensions
- Clear browsing data regularly
- Update to latest browser version
- Check for conflicting security software
- Restart browser completely

## 15.3 Browser Security Settings
Required security configurations:
- Pop-up blocker enabled
- Do Not Track enabled
- Third-party cookies blocked
- Download file type restrictions
- Certificate warnings respected
- Auto-updates enabled

---

# 16. Operating System Updates

## 16.1 Windows Update Policy
Company Windows update requirements:
- Quality updates: install within 7 days
- Feature updates: install within 30 days
- Security updates: automatic installation
- Reboot windows: 6PM-6AM only
- Defer updates: maximum 14 days
- Manual check: Settings > Update & Security

## 16.2 macOS Update Policy
Mac system update guidelines:
- Minor updates: install within 14 days
- Major versions: test period before rollout
- Security Response updates: immediate
- Restart required: schedule off-hours
- Backup before major updates
- Report issues immediately

## 16.3 Update Troubleshooting
**Updates failing to install:**
- Check available disk space (minimum 20GB)
- Disable antivirus temporarily
- Download update manually from Microsoft/Apple
- Run Windows Update troubleshooter
- Check Windows Update service running
- Contact IT if repeatedly failing

---

# 17. Access Control and Permissions

## 17.1 File Share Permissions
Requesting folder access:
1. Submit access request via ServiceNow
2. Specify folder path and access level needed
3. Provide business justification
4. Manager approval required
5. Access granted within 24 hours
6. Review quarterly for continued need

## 17.2 Application Access
Requesting application permissions:
- New application: submit formal request
- Elevated privileges: manager + IT approval
- Admin rights: executive approval required
- Temporary access: specify duration
- Access logged and audited
- Violations result in account suspension

## 17.3 Access Review Process
Quarterly access reviews:
- IT sends access summary to managers
- Managers verify continued need
- Remove access no longer required
- Document any changes
- Complete within 10 business days
- Non-compliance escalated to executives

---

# 18. Active Directory Account Management

## 18.1 Account Provisioning
New employee account setup:
- Created within 24 hours of HR notification
- Username format: firstname.lastname
- Email: firstname.lastname@company.com
- Initial password: ChangeMe123!
- Must change on first login
- Added to default groups automatically

## 18.2 Account Modifications
Changing account attributes:
- Name changes: HR notification required
- Department moves: manager approval needed
- Title updates: HR system sync (automatic)
- Group membership: request via IT portal
- Email alias: maximum 3 per user
- Distribution list: created by IT only

## 18.3 Account Deactivation
Employee departure process:
- HR notifies IT on last day
- Account disabled end of business
- Email forwarding: 30 days to manager
- Files transferred to manager share
- Licenses reclaimed immediately
- Account deleted after 90 days

---

# 19. VoIP Phone System

## 19.1 Desk Phone Setup
Configuring VoIP phones:
- Phones auto-provision via DHCP
- Extension assigned by IT
- Voicemail PIN: last 4 of employee ID
- Forward to mobile: *72 + 10-digit number
- Conference bridge: dial 9 + extension
- Speed dial: up to 10 numbers

## 19.2 Voicemail Configuration
Setting up voicemail:
- Dial extension + # to access
- Default PIN must be changed
- Record personal greeting
- Email notification of new messages
- Visual voicemail via web portal
- Transcription available (English only)

## 19.3 Phone System Troubleshooting
**No dial tone:**
- Check network cable connection
- Verify PoE switch port active
- Restart phone (unplug 30 seconds)
- Check account provisioned correctly
- Test with different phone
- Submit ticket if hardware issue

**Poor call quality:**
- Check network bandwidth usage
- Use wired connection, not WiFi
- Close VPN during internal calls
- Update phone firmware
- Test different handset
- Report to telecom team

---

# 20. Collaboration Tools (Microsoft Teams)

## 20.1 Teams Configuration
Microsoft Teams setup:
- Desktop app required (not browser)
- Sign in: username@company.com
- Sync status: Available during work hours
- Notifications: priority only after hours
- File storage: SharePoint integration
- External chat: disabled by default

## 20.2 Teams Best Practices
Effective Teams usage:
- Use channels for topic-based discussions
- @mention for direct attention
- Schedule meetings don't interrupt with calls
- Share files via Teams not email attachments
- Use status indicators accurately
- Record important meetings (with permission)

## 20.3 Teams Troubleshooting
**Teams not loading:**
- Clear Teams cache: %appdata%\Microsoft\Teams
- Sign out and sign in again
- Check network connectivity
- Disable proxy settings
- Reinstall Teams application
- Try Teams web version temporarily

---

# 21. Disk Space Management

## 21.1 Checking Disk Space
Monitor storage usage:
- Windows: File Explorer > This PC
- Mac: About This Mac > Storage
- Critical threshold: <10% free space
- Warning threshold: <20% free space
- Regular cleanup: monthly recommended

## 21.2 Freeing Disk Space
Methods to recover storage:
- Delete temp files: Disk Cleanup utility
- Empty Recycle Bin/Trash
- Clear browser cache
- Remove old downloads
- Uninstall unused programs
- Move files to OneDrive
- Compress old files
- Delete duplicate files

## 21.3 Storage Quota Management
Company storage policies:
- Laptop/Desktop: 512GB standard
- OneDrive: 1TB per user
- Network share: 50GB per user
- Email mailbox: 50GB limit
- Archive to network if over quota
- Request increase via IT portal

---

# 22. SSL Certificate Errors

## 22.1 Understanding Certificate Errors
Common certificate warnings:
- **Expired certificate**: Contact site administrator
- **Self-signed certificate**: Internal sites only
- **Name mismatch**: Verify correct URL
- **Untrusted issuer**: May be legitimate internal cert
- Never proceed on external sites

## 22.2 Installing Company Certificates
Adding corporate certificates:
1. Download cert from https://pki.company.com
2. Double-click certificate file
3. Install to "Trusted Root Certification Authorities"
4. Restart browser
5. Verify no more warnings
6. Contact IT if issues persist

## 22.3 Certificate-Related Troubleshooting
**Persistent certificate errors:**
- Check system date/time (must be accurate)
- Clear browser SSL cache
- Remove and re-add certificates
- Check for expired company certificates
- Verify not behind filtering proxy
- Update root certificate bundle

---

# 23. Performance Optimization

## 23.1 System Performance Diagnostics
Checking system health:
- Task Manager: CPU, Memory, Disk usage
- Resource Monitor: detailed process view
- Performance Monitor: historical trends
- Event Viewer: system errors/warnings
- Disk defragmentation status
- SSD TRIM optimization

## 23.2 Improving Computer Performance
Performance enhancement steps:
- Close unnecessary startup programs
- Disable visual effects (Windows)
- Increase virtual memory/swap
- Upgrade RAM if consistently >80% usage
- Replace HDD with SSD
- Run disk cleanup and defragment
- Uninstall bloatware
- Scan for malware

## 23.3 When to Request Hardware Upgrade
Request new equipment if:
- Computer >4 years old
- RAM maxed out, still insufficient
- Boot time >5 minutes consistently
- Applications freeze regularly
- Unable to run required software
- Hardware errors in diagnostics
- Physical damage affecting performance

---

# 24. Encrypted Email Communication

## 24.1 Sending Encrypted Email
Sending secure messages:
1. Compose email normally
2. Click "Encrypt" button in Outlook
3. Select encryption type: OME
4. External recipients receive secure link
5. Internal emails auto-encrypted
6. Subject line not encrypted

## 24.2 Receiving Encrypted Email
Opening encrypted messages:
- Internal: opens normally in Outlook
- External: click link in notification
- Authenticate via Microsoft account
- Read message in web portal
- Reply stays encrypted
- Valid for 90 days

## 24.3 Encryption Requirements
When to use encryption:
- Customer personal information (PII)
- Financial data or account numbers
- Legal documents
- Confidential business information
- Employee personal data
- Anything marked "Confidential"

---

# 25. Wireless Keyboard and Mouse Issues

## 25.1 Bluetooth Pairing
Connecting Bluetooth devices:
1. Enable Bluetooth on computer
2. Put device in pairing mode
3. Select device from available list
4. Enter PIN if prompted (usually 0000)
5. Wait for successful connection
6. Test device functionality

## 25.2 Troubleshooting Wireless Peripherals
**Device not responding:**
- Check battery level/replace batteries
- Verify Bluetooth enabled
- Remove and re-pair device
- Check for interference (other Bluetooth devices)
- Update Bluetooth drivers
- Try USB dongle instead (if included)
- Test with wired device to isolate issue

## 25.3 Peripheral Best Practices
- Use company-approved devices only
- Keep spare batteries at desk
- Don't pair personal devices to work computer
- Report lost Bluetooth devices immediately
- Update device firmware when available
- Clean devices monthly

---

# 26. Screen Display Issues

## 26.1 Common Display Problems
**No display:**
- Check monitor power and cable connections
- Try different video cable/port
- Test monitor with different computer
- Check display settings: Win+P (Windows)
- Update graphics drivers
- Reset display to default settings

**Display quality issues:**
- Adjust resolution to native (typically 1920x1080)
- Change refresh rate to 60Hz or higher
- Calibrate color settings
- Clean monitor screen
- Check for dead pixels
- Replace old monitors (>5 years)

## 26.2 Multiple Monitor Setup
Configuring dual monitors:
1. Connect both monitors
2. Right-click desktop > Display settings
3. Detect displays if not shown
4. Arrange monitors to match physical layout
5. Set primary display
6. Choose extend mode (not duplicate)
7. Adjust individual resolutions

## 26.3 Docking Station Issues
**Monitors not working with dock:**
- Disconnect and reconnect dock
- Update dock firmware
- Update graphics drivers
- Try different USB-C/Thunderbolt port
- Check dock power supply
- Test monitors directly to laptop
- Replace dock if persistent issues

---

# 27. Keyboard Shortcuts for Productivity

## 27.1 Essential Windows Shortcuts
Common keyboard shortcuts:
- **Win+L**: Lock computer
- **Win+E**: Open File Explorer
- **Alt+Tab**: Switch between windows
- **Ctrl+Shift+Esc**: Task Manager
- **Win+V**: Clipboard history
- **Win+Shift+S**: Screenshot tool
- **Win+.**: Emoji picker

## 27.2 Essential Mac Shortcuts
macOS productivity shortcuts:
- **Cmd+Space**: Spotlight search
- **Cmd+Tab**: Switch applications
- **Cmd+Q**: Quit application
- **Cmd+Shift+3**: Screenshot
- **Cmd+,**: Application preferences
- **Cmd+Ctrl+Q**: Lock screen
- **Cmd+Shift+T**: Reopen closed tab

## 27.3 Application-Specific Shortcuts
**Outlook/Email:**
- Ctrl/Cmd+N: New email
- Ctrl/Cmd+R: Reply
- Ctrl/Cmd+Shift+R: Reply all
- Ctrl/Cmd+F: Forward
- Ctrl/Cmd+Enter: Send

**Browser:**
- Ctrl/Cmd+T: New tab
- Ctrl/Cmd+W: Close tab
- Ctrl/Cmd+Shift+T: Reopen closed tab
- Ctrl/Cmd+L: Address bar
- Ctrl/Cmd+D: Bookmark page

---

# 28. Software Licensing Compliance

## 28.1 License Types
Understanding software licenses:
- **Per-user**: assigned to specific person
- **Per-device**: assigned to specific computer
- **Concurrent**: shared pool, first-come first-served
- **Site license**: unlimited use within company
- **Subscription**: annual/monthly renewal

## 28.2 Compliance Requirements
License compliance obligations:
- Use software only as licensed
- Don't share login credentials
- Uninstall when no longer needed
- Report unused licenses for reassignment
- Don't install personal copies at work
- Annual audit participation mandatory

## 28.3 Audit Procedures
Software audit process:
- IT scans all devices quarterly
- Verify installed software matches licenses
- Identify unauthorized installations
- Remove or purchase licenses for violations
- Document exceptions with justification
- Report findings to management

---

# 29. Cloud Application Access

## 29.1 SSO (Single Sign-On) Portal
Accessing cloud applications:
- Navigate to https://portal.company.com
- Sign in with company credentials
- MFA verification required
- Click application tile to launch
- Automatic authentication to app
- Session timeout: 8 hours

## 29.2 Common Cloud Applications
Company-approved SaaS tools:
- Salesforce: CRM
- Workday: HR/Finance
- ServiceNow: IT ticketing
- Confluence: Documentation
- JIRA: Project management
- Box: File sharing
- DocuSign: Electronic signatures

## 29.3 Cloud Access Troubleshooting
**Cannot access cloud app:**
- Verify credentials not locked
- Check MFA device working
- Clear browser cookies for app
- Try different browser
- Verify license assigned
- Check if app experiencing outage
- Contact IT if app-specific issue

---

# 30. USB Device Policies

## 30.1 Approved USB Devices
Permitted USB devices:
- Company-issued USB drives (encrypted)
- Approved keyboards/mice
- Webcams (approved models)
- Charging cables only (no data)
- Company-issued mobile phones

## 30.2 Prohibited USB Devices
Not allowed to connect:
- Personal USB flash drives
- External hard drives (without approval)
- USB network adapters
- Unknown devices found on premises
- Devices from untrusted sources

## 30.3 USB Security Procedures
USB device safety:
- Scan all USB drives with antivirus before use
- Encrypt all company data on USB
- Report lost/stolen USB immediately
- Never pick up unknown USB devices
- Disable AutoRun/AutoPlay
- Request encrypted USB from IT

---

# 31. Audio and Microphone Issues

## 31.1 Audio Output Troubleshooting
**No sound:**
- Check volume level (not muted)
- Verify correct output device selected
- Test with headphones
- Update audio drivers
- Restart audio service
- Check physical connections
- Try different audio port

## 31.2 Microphone Troubleshooting
**Microphone not working:**
- Check app permissions (Windows Privacy)
- Verify mic not muted in system tray
- Test in different application
- Check mic as default recording device
- Update audio drivers
- Try different USB port
- Test with different microphone

## 31.3 Conference Call Audio
Optimizing meeting audio:
- Use headset instead of speakerphone
- Mute when not speaking
- Close applications using audio
- Position mic close to mouth
- Reduce background noise
- Test audio before important meetings
- Use wired headset if Bluetooth issues

---

# 32. Software Update Management

## 32.1 Critical Software Updates
Priority update schedule:
- Security patches: within 72 hours
- Browser updates: within 1 week
- Office suite: within 2 weeks
- Operating system: within 1 month
- Third-party apps: as recommended

## 32.2 Update Notification Handling
Responding to update prompts:
- Don't ignore security updates
- Save work before installing
- Schedule updates during downtime
- Restart when prompted
- Verify functionality after update
- Report issues immediately

## 32.3 Update Troubleshooting
**Update installation failures:**
- Retry update after restart
- Free up disk space (minimum 20GB)
- Disable antivirus temporarily
- Download update manually
- Check Windows Update service running
- Review error codes in Event Viewer
- Contact IT for persistent failures

---

# 33. Firewall and Network Security

## 33.1 Corporate Firewall
Understanding company firewall:
- Blocks unauthorized incoming connections
- Monitors outbound traffic
- Filters web content categories
- Prevents known malware downloads
- Cannot be disabled on company devices
- Centrally managed by IT

## 33.2 Personal Firewall Settings
Device firewall configuration:
- Windows Defender Firewall: always enabled
- Allow company applications through firewall
- Block all incoming unless needed
- Enable for all network types (domain, private, public)
- Don't create exceptions without IT approval

## 33.3 Firewall Issues
**Application blocked by firewall:**
- Verify application approved by IT
- Request firewall exception via IT portal
- Provide application name and publisher
- Specify required ports/protocols
- Business justification required
- IT creates rule within 24-48 hours

---

# 34. Data Loss Prevention (DLP)

## 34.1 DLP Policies
Company data protection rules:
- Cannot email customer data to personal accounts
- Cannot upload sensitive files to personal cloud
- Cannot copy financial data to USB drives
- Cannot screenshot proprietary information
- Print jobs with sensitive data flagged

## 34.2 DLP Violations
Handling DLP alerts:
- Alert sent to employee and manager
- Review what triggered alert
- Provide business justification if legitimate
- Complete security awareness training
- Multiple violations escalated
- Serious violations: account suspension

## 34.3 Complying with DLP
Avoiding DLP blocks:
- Use company approved sharing methods
- Encrypt sensitive data before transfer
- Use secure file transfer portal
- Request exceptions in advance
- Follow data classification guidelines
- Ask IT if unsure about transfer method

---

# 35. Webcam Configuration and Issues

## 35.1 Webcam Setup
Configuring video camera:
- Built-in cameras: no setup needed
- External USB cameras: plug and play
- Grant permission in application settings
- Verify default camera in app settings
- Adjust brightness/contrast as needed
- Position at eye level

## 35.2 Webcam Troubleshooting
**Camera not working:**
- Check privacy settings (camera access)
- Close other apps using camera
- Update webcam drivers
- Try different USB port
- Restart computer
- Test in Camera app (Windows/Mac)
- Replace if hardware failure

## 35.3 Video Conference Best Practices
Professional video meetings:
- Use virtual background or clean physical background
- Ensure adequate lighting (face forward)
- Position camera at eye level
- Test video before important meetings
- Mute when not speaking
- Look at camera when speaking
- Dress professionally even remote

---

# 36. System Restore and Recovery

## 36.1 Creating System Restore Points
Windows System Restore:
- Create before major changes
- Automatic creation weekly
- Restore points keep 30 days
- Access: Control Panel > Recovery
- Does not affect personal files
- Restores system files and settings

## 36.2 Using System Restore
Restoring system to previous state:
1. Search "System Restore"
2. Choose restore point (date before issue)
3. Review affected programs
4. Confirm and start restore
5. Computer will restart
6. Verify issue resolved
7. Contact IT if still experiencing problems

## 36.3 Recovery Options
Other recovery methods:
- **Reset PC**: keeps files, reinstalls Windows
- **Fresh Start**: clean Windows install
- **Recovery drive**: boot from USB
- **System Image**: complete backup restore
- Contact IT before using recovery options

---

# 37. Group Policy and Domain Issues

## 37.1 Group Policy Updates
Understanding domain policies:
- Applied at startup/login automatically
- Cannot be modified by user
- Updates pushed by IT centrally
- Some settings locked for security
- Affects all domain-joined computers

## 37.2 Common Policy Restrictions
Typical group policy limitations:
- Cannot install unapproved software
- Screen lock after 10 minutes
- Password complexity enforced
- USB device restrictions
- Control Panel access limited
- Registry editing disabled

## 37.3 Domain Connection Issues
**Computer not connecting to domain:**
- Verify network connectivity
- Check VPN if remote
- Trust relationship may be broken
- Restart computer to refresh policies
- Contact IT to reset computer account
- May need to rejoin domain

---

# 38. Ergonomics and Workspace Setup

## 38.1 Proper Desk Setup
Ergonomic workstation configuration:
- Monitor top at or below eye level
- Monitor arm's length away (20-26 inches)
- Keyboard and mouse at elbow height
- Feet flat on floor or footrest
- Chair with lumbar support
- Wrists straight when typing

## 38.2 Equipment Requests
Requesting ergonomic equipment:
- Submit request via HR portal
- Manager approval required
- Options: monitor arm, standing desk, ergonomic keyboard
- Doctor note needed for medical accommodations
- IT coordinates delivery and setup
- Training provided for new equipment

## 38.3 Preventing Repetitive Strain
Avoiding computer-related injuries:
- Take breaks every hour (5-10 minutes)
- Use correct posture
- Adjust chair height properly
- Keep frequently used items within reach
- Vary tasks throughout day
- Report discomfort early

---

# 39. BitLocker Disk Encryption

## 39.1 BitLocker Overview
Company encryption policy:
- All laptops encrypted with BitLocker
- Encryption automatic on domain join
- Recovery key stored in AD
- Cannot disable without admin password
- Performance impact minimal

## 39.2 BitLocker Recovery
**Locked out of computer:**
1. Note computer name/asset tag
2. Contact IT Help Desk immediately
3. Provide employee ID verification
4. IT retrieves recovery key from AD
5. Enter 48-digit recovery key
6. Computer unlocks and boots normally
7. Report incident for tracking

## 39.3 BitLocker Best Practices
Using encrypted drives safely:
- Don't share recovery keys
- Backup key when prompted
- Report hardware changes to IT
- Don't attempt to disable encryption
- Keep TPM chip enabled in BIOS
- Test recovery process annually

---

# 40. Application Performance Issues

## 40.1 Diagnosing Slow Applications
Troubleshooting app performance:
- Check CPU usage in Task Manager
- Monitor memory consumption
- Review network activity
- Check disk I/O performance
- Update application to latest version
- Clear application cache
- Reinstall if corrupted

## 40.2 Application Crashes
**Program keeps crashing:**
- Note error messages/codes
- Check Event Viewer for details
- Update to latest version
- Run application as administrator
- Check for conflicting software
- Repair installation
- Uninstall and reinstall cleanly

## 40.3 Compatibility Issues
Running older applications:
- Try compatibility mode (right-click > Properties)
- Run as administrator
- Disable DPI scaling
- Update graphics drivers
- Check vendor compatibility list
- Request virtualized version from IT
- Consider alternative modern software

---

# 41. Network Shared Drives

## 41.1 Mapping Network Drives
Connecting to shared folders:
1. Open File Explorer
2. Click "Map network drive"
3. Select drive letter
4. Enter path: \\server\share
5. Check "Reconnect at sign-in"
6. Click Finish
7. Access drive from This PC

## 41.2 Network Drive Issues
**Cannot access network drive:**
- Verify VPN connected if remote
- Check network connectivity
- Confirm permissions to folder
- Try accessing via UNC path
- Clear cached credentials
- Remove and remap drive
- Contact IT if persistent

## 41.3 Network Drive Best Practices
Using shared drives effectively:
- Don't store personal files on shared drives
- Respect folder structure and naming
- Don't move/delete others' files
- Use appropriate permissions
- Monitor quota usage
- Clean up old files regularly
- Report permission issues promptly

---

# 42. Spam and Phishing Protection

## 42.1 Identifying Phishing Emails
Warning signs of phishing:
- Sender address doesn't match company domain
- Generic greetings ("Dear user")
- Urgent action required
- Suspicious links (hover to preview)
- Requests for personal information
- Poor grammar/spelling
- Unexpected attachments

## 42.2 Reporting Phishing
When receiving suspicious email:
1. Don't click links or open attachments
2. Don't reply to sender
3. Click "Report Phishing" in Outlook
4. Forward to security@company.com
5. Delete from inbox
6. IT will investigate and take action

## 42.3 Spam Filtering
Managing email spam:
- Company spam filter auto-blocks most
- Check Junk folder for false positives
- Mark spam: right-click > Junk
- Never unsubscribe from obvious spam
- Create inbox rules for repeated spam
- Don't share work email on public sites
- Use alias for newsletter subscriptions

---

# 43. Time and Date Synchronization

## 43.1 Importance of Accurate Time
Why time sync matters:
- Required for authentication
- Necessary for MFA codes
- Certificate validation depends on time
- Log correlation for security
- Meeting scheduling accuracy
- File timestamps

## 43.2 Configuring Time Sync
Setting up time synchronization:
- **Windows**: automatically syncs with domain
- **Mac**: System Preferences > Date & Time
- Check "Set time automatically"
- Time server: time.company.com
- Time zone set correctly
- Daylight saving adjusts automatically

## 43.3 Time-Related Issues
**Wrong time on computer:**
- Sync now: Settings > Time & Language
- Replace CMOS battery (desktops)
- Check time zone setting
- Verify internet connection (for NTP)
- Rejoin domain to reset policies
- Contact IT if automatic sync fails

---

# 44. PDF Reader and Creation

## 44.1 Adobe Acrobat Configuration
Company PDF software:
- Adobe Acrobat DC (licensed)
- Adobe Reader (free viewing)
- Set as default PDF application
- Enable auto-updates
- Sign PDFs with digital certificate
- Use company email for Adobe ID

## 44.2 PDF Troubleshooting
**PDF won't open:**
- Update Adobe Reader/Acrobat
- Try different PDF reader (Chrome, Edge)
- Check if file corrupted (re-download)
- Repair Adobe installation
- Check file permissions
- Convert to different format if needed

## 44.3 Creating and Editing PDFs
Working with PDF files:
- Print to PDF from any application
- Edit with Acrobat DC (licensed users)
- Fill forms with Reader (free)
- Compress large PDFs before sending
- Use PDF/A for archival
- Protect sensitive PDFs with password
- OCR scanned documents for searchability

---

# 45. Registry Cleaning and Maintenance

## 45.1 Registry Overview
Windows Registry information:
- Database of system settings
- **DO NOT modify without IT guidance**
- Backup before any changes
- Incorrect changes can break Windows
- Use regedit with extreme caution
- Most users should never access

## 45.2 Safe Registry Practices
If registry edit required:
1. Create system restore point first
2. Export registry key before changing
3. Follow IT instructions exactly
4. Double-check path before modifying
5. Restart computer after changes
6. Restore if issues occur

## 45.3 Registry Cleaners
Warning about registry tools:
- DON'T use registry cleaning software
- These tools often cause more problems
- Can corrupt Windows installation
- Not needed for normal operation
- IT will handle registry issues
- Ignore ads for registry cleaners

---

# 46. Startup Programs Management

## 46.1 Viewing Startup Programs
Checking startup applications:
- **Windows**: Task Manager > Startup tab
- **Mac**: System Preferences > Users & Groups > Login Items
- Shows programs that auto-start
- Indicates startup impact (high/medium/low)
- Disable unnecessary programs

## 46.2 Optimizing Startup
Improving boot time:
- Disable non-essential startup programs
- Keep antivirus enabled
- Keep company management tools enabled
- Remove trial software auto-starts
- Delay startup of non-critical apps
- Use Task Scheduler for delayed start

## 46.3 Problematic Startup Programs
Managing startup issues:
- Too many programs slow boot
- Check for malware in startup
- Update programs causing delays
- Remove programs no longer used
- Some programs required by policy (can't disable)
- Contact IT if unsure about program

---

# 47. Clipboard and Copy-Paste Issues

## 47.1 Clipboard Troubleshooting
**Copy-paste not working:**
- Restart application
- Try keyboard shortcuts (Ctrl+C, Ctrl+V)
- Restart Windows Explorer (Task Manager)
- Clear clipboard: Win+V > Clear all
- Check if source allows copying
- Restart computer if persistent
- Try paste as plain text (Ctrl+Shift+V)

## 47.2 Clipboard History
Using Windows Clipboard History:
- Enable: Settings > System > Clipboard
- Access: Win+V
- Stores last 25 items
- Syncs across devices with Microsoft account
- Pin frequently used items
- Clear sensitive data after use

## 47.3 Clipboard Security
Safe clipboard practices:
- Don't copy passwords (use password manager)
- Clear clipboard after copying sensitive data
- Be aware of clipboard monitoring malware
- Don't use online clipboard services
- Disable cloud clipboard for sensitive work
- Check what's copied before pasting in emails

---

# 48. Screensaver and Lock Screen

## 48.1 Screen Lock Policy
Company lock screen requirements:
- Auto-lock after 10 minutes idle
- Manual lock: Win+L or Cmd+Ctrl+Q
- Screen saver not required (uses lock screen)
- Password required to unlock
- Cannot disable auto-lock (policy enforced)

## 48.2 Lock Screen Customization
Personalizing lock screen:
- Windows: Settings > Personalization > Lock screen
- Mac: System Preferences > Desktop & Screen Saver
- Use professional background image
- Show company logo option available
- Don't display sensitive information
- Limit notification details on lock screen

## 48.3 Lock Screen Troubleshooting
**Can't unlock computer:**
- Verify caps lock not on
- Check correct keyboard language
- Try logging in as different user
- Force restart if completely frozen
- Contact IT for password reset
- May need to rejoin domain

---

# 49. Font Installation and Management

## 49.1 Installing Fonts
Adding new fonts:
- **Windows**: Right-click font file > Install
- **Mac**: Double-click font > Install Font
- Install for all users (requires admin)
- Restart applications to see new fonts
- Company fonts available at: \\fonts\shared

## 49.2 Company Standard Fonts
Approved corporate fonts:
- Primary: Segoe UI, Calibri
- Presentations: Arial, Helvetica
- Brand materials: (company custom fonts)
- Request custom fonts via IT portal
- Don't install random internet fonts
- Use web-safe fonts for documents

## 49.3 Font Troubleshooting
**Font not appearing:**
- Verify font installed correctly
- Restart application
- Check font not corrupted
- Install for all users, not just current
- Clear font cache
- Reinstall problematic font
- Use similar alternative if font missing

---

# 50. Keyboard Language and Input Methods

## 50.1 Adding Input Languages
Setting up multiple keyboards:
- Settings > Time & Language > Language
- Add keyboard layout
- Switch: Win+Space or Alt+Shift
- Show language bar in taskbar
- Set default input language
- Remove unused layouts

## 50.2 Special Characters
Typing special characters:
- Windows Character Map: Win+R > charmap
- Mac Character Viewer: Ctrl+Cmd+Space
- Alt codes: hold Alt, type code on numpad
- Common codes: © (Alt+0169), ® (Alt+0174)
- Emoji: Win+. or Cmd+Ctrl+Space

## 50.3 Input Method Troubleshooting
**Wrong keyboard layout:**
- Check language indicator in taskbar
- Switch layout: Win+Space
- Remove incorrect layouts
- Set default input method
- Restart if layout stuck
- Verify keyboard hardware matches layout

---

# 51. Laptop Docking and Undocking

## 51.1 Proper Docking Procedures
Docking laptop correctly:
1. Align laptop with dock connector
2. Press firmly until seated
3. Verify power indicator on dock
4. Displays should auto-detect
5. External keyboard/mouse connects
6. Allow 30 seconds for full detection

## 51.2 Undocking Procedures
Safely removing laptop from dock:
1. Save all work
2. Close applications using external drives
3. Disconnect external storage safely
4. Lift laptop straight up from dock
5. Verify battery charging
6. Reconnect to WiFi if needed

## 51.3 Docking Issues
**Monitors not working when docked:**
- Disconnect and reconnect dock
- Update dock firmware
- Update display drivers
- Check cable connections to monitors
- Try different dock port
- Test monitors with direct connection
- Replace dock if faulty

---

# 52. Browser Extension Management

## 52.1 Approved Extensions
Company-permitted browser extensions:
- LastPass (password manager)
- Microsoft Editor
- Grammarly (with approval)
- Adobe Acrobat extension
- Zoom extension
- Company VPN extension

## 52.2 Extension Security
Browser extension safety:
- Only install from official stores
- Review permissions before installing
- Remove unused extensions
- Keep extensions updated
- Report suspicious extension behavior
- Don't install random extensions

## 52.3 Managing Extensions
**Extension causing issues:**
- Disable extension temporarily
- Clear extension data
- Reinstall extension
- Check for updates
- Test in incognito mode (extensions disabled)
- Remove if persistent problems
- Report to IT if company-required extension fails

---

# 53. IT Support Contact Information

## 53.1 Help Desk Contact Methods
Getting IT support:
- **Phone**: 555-5555 (M-F 8AM-6PM)
- **Email**: itsupport@company.com
- **Portal**: https://helpdesk.company.com
- **Chat**: Available in portal 24/7
- **Walk-in**: Building A, Floor 1
- **Emergency after hours**: 555-5556

## 53.2 Creating Support Tickets
Effective ticket submission:
- Use portal for non-urgent issues
- Include detailed problem description
- List troubleshooting steps already tried
- Attach screenshots of errors
- Specify urgency/business impact
- Provide contact preference
- Include asset tag/computer name

## 53.3 Service Level Agreements
Support response times:
- **Critical** (system down): 1 hour
- **High** (impacted work): 4 hours
- **Medium** (inconvenience): 1 business day
- **Low** (question/request): 3 business days
- Updates provided every 24 hours
- Escalate if SLA not met

---

# 54. Asset Management and Inventory

## 54.1 Company Asset Tracking
IT equipment accountability:
- All equipment tagged with asset number
- Annual inventory audit required
- Report missing/stolen equipment immediately
- Return equipment on last day of employment
- Transfer equipment with manager approval
- Don't remove asset tags

## 54.2 Equipment Checkout
Borrowing IT equipment:
1. Submit request via IT portal
2. Specify equipment type and duration
3. Manager approval required (>7 days)
4. Sign checkout form
5. Return by due date
6. Late returns: escalated to manager

## 54.3 Equipment Disposal
Retiring old equipment:
- Don't throw away company IT equipment
- Submit disposal request to IT
- IT securely wipes all data
- Equipment donated or recycled
- Certificate of destruction provided
- Never sell or gift company equipment

---

# 55. Remote Work Technology

## 55.1 Home Office Setup
Remote work IT requirements:
- Company laptop (don't use personal computer)
- Secure home WiFi (WPA2/WPA3)
- VPN always on when working
- Separate work and personal devices
- Ergonomic workspace setup
- Reliable internet (minimum 25 Mbps)

## 55.2 Remote Access Tools
Working from home technology:
- VPN: required for all company resources
- Remote Desktop: access office computer
- Teams: primary communication tool
- OneDrive: file access from anywhere
- Web apps: available via SSO portal
- Virtual desktop: for special applications

## 55.3 Remote Work Security
Protecting company data at home:
- Lock computer when away from desk
- Don't let family use work computer
- Secure home WiFi with strong password
- Use privacy screen in public places
- Report lost/stolen equipment immediately
- Keep work devices separate from personal
- Don't access company data on personal devices
