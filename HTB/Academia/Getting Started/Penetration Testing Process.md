---
id: Getting Started
aliases: []
tags:
  - theme/cybersecurity/htb/academy
  - type/academy-note
  - topic/academy/gettingStarted
created: 2025-04-14T05:56
lead: +++ Lead paragraph goes here +++
modified: 2025-04-15T05:28
status: TODO
template-version: "2"
template_type: Course Note
uuid: C3D3C304-DDC4-4AAD-8074-4E6686477042
---
# Penetration Testing Process

> [!Summary]
> `= this.lead` 

## Infosec Overview
<!-- Overview Of What Will Be covered in This Course -->

##  
<!--- Header For Each Page Your READ With The following

Brief walkthrough notes from the page/article/video.

### Key Concepts
- 🔑 Point 1
- 🔍 Point 2

### Visual / Diagram
![Screenshot]()  
-->
---
## Service Scanning
A service is an application running on a computer that performs some useful function for other users or computers.

### Nmap
Most basic scan
![](attachments/Screenshot%202025-04-15%20at%205.08.00%20AM.png)
 
 port 3389 is the default port for Remote Desktop Services and is an excellent indication that the target is a Windows machine. Port 22 (SSH) indicates that the target is running Linux/Unix, but this service can also be configured on Windows. 

We can use the -sC parameter to specify that Nmap scripts should be used to try and obtain more detailed information. The -sV parameter instructs Nmap to perform a version scan. Finally, -p- tells Nmap that we want to scan all 65,535 TCP ports

![](attachments/Penetration%20Testing%20Process-20250415.png)

### SMB
SMB allows users and administrators to share folders and make them accessible remotely by other users. smbclient can interact with SMB shares. The -L flag retrieves a list of available shares on the remote host while -N suppresses the password prompt

![](attachments/Penetration%20Testing%20Process-20250415-1.png)

---

## **Practice Questions**
<!-- Flashcard style - Can be parsed by Obsidian plugins like Obsidian CardBoard or Obsidian Recall -->

**Q**:  What is the version of the service on port 8080? 
**A**: Apache Tomcat!
![](attachments/Screenshot%202025-04-15%20at%204.24.30%20AM.png)

**Q**: Non-default port the telnet service is running on
**A**: 2323


**Q**: List SMB shares on target host. Connect to share as bob user. Once connected, access the folder called ‘flag’ and submit contents of the flag.txt file
**A**: ![](attachments/Screenshot%202025-04-15%20at%204.56.56%20AM.png)

**Q**:
**A**:


**Q**:
**A**:

**Q**:
**A**:

**Q**:
**A**:

**Q**:
**A**:

**Q**:
**A**:

**Q**:
**A**:


---

## **External Resources**
- [Getting started writeup](https://medium.com/@joshthedev/step-5-getting-started-a586c57af17d)

---

---

## ✅ Tasks
- [ ] Create Flashcards

---
