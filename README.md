# wbackup
Windows Backup Scripts for sending Alert Mails via Powershell

# PowerShell Backup Reporting Script

This PowerShell script generates reports on the status of Windows backups and sends them via email.

## Usage

1. **Requirements:**

   - SMTP Server
   - PowerShell
   - Windows Server Backup module
   - Task Scheduler

2. **Configuration:**

   - Edit the file `yourScript.ps1`:

     - Adjust the SMTP server:
       ```powershell
       $smtpServer = "yourSMTPServer"
       ```

     - Customize the sender address, recipient address, and other email settings:
       ```powershell
       $msg.From = "your@Mail"
       $msg.ReplyTo = "your@Mail"
       $msg.To.Add("your@Mail")
       ```
       
3. **Running the Script:**

   - Run the script:
     ```powershell
     .\yourScript.ps1
     ```

   - The script generates a report on the backup status and sends it via email.
  
4. **Task Scheduler Configuration:**

   - To automate the script, set up tasks in Task Scheduler to trigger on the desired event IDs.


