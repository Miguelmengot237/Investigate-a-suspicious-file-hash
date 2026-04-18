# Investigate-a-suspicious-file-hash
Using investigative tools like VirusTotal to investigate a suspicious file hash

I am a level one security operations center (SOC) analyst at a financial services company. I received an alert about a suspicious file being downloaded on an employee's computer. 

I investigate this alert and discover that the employee received an email containing an attachment. The attachment was a password-protected spreadsheet file. The spreadsheet's password was provided in the email. The employee downloaded the file, then entered the password to open it. When the employee opened the file, a malicious payload was then executed on their computer. 

I retrieved the malicious file and created a SHA256 hash of the file. With the file hash, I used VirusTotal to uncover additional IoCs that are associated with the file.

SHA256 file hash: 54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b

Here is a timeline of the events leading up to this alert:

1:11 p.m.: An employee receives an email containing a file attachment.
1:13 p.m.: The employee successfully downloads and opens the file.
1:15 p.m.: Multiple unauthorized executable files are created on the employee's computer.
1:20 p.m.: An intrusion detection system detects the executable files and sends out an alert to the SOC.
