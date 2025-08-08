# 🛡️ Basic Vulnerability Scan on PC  

## 📖 Introduction  
Vulnerability scanning is a security process used to identify weaknesses, misconfigurations, and outdated software in a computer system or network. These weaknesses, known as **vulnerabilities**, can be exploited by attackers to gain unauthorized access, steal data, or disrupt services.  

By using automated tools like **OpenVAS** or **Nessus Essentials**, security analysts can detect and prioritize vulnerabilities based on their severity. Performing regular vulnerability scans is a critical part of maintaining strong cybersecurity hygiene and protecting systems from evolving threats.  

## 📌 Objective  
Perform a basic vulnerability scan on your computer using **OpenVAS** or **Nessus Essentials** to identify common security risks and understand their severity.  

## 🛠 Tools Used  
- **Nessus Essentials** *(Free vulnerability scanner)*  
- **Operating System:** Ubuntu  
- **Network Type:** Localhost / LAN  

## 📋 Steps Performed  

1. **Installed Vulnerability Scanner**  
   - Downloaded and installed **Nessus Essentials** from the official Tenable website.  
   - Registered for a free activation code.  
   - *![Screenshot - Nessus Installation](screenshots/1_installation.png)*  

2. **Configured Scan Target**  
   - Set target as **local machine IP** (`127.0.0.1` or system’s local IP).  
   - *![Screenshot - Target Configuration](screenshots/2_target.png)*  

3. **Performed Full Scan**  
   - Selected **Full Scan** template in Nessus.  
   - Started the scan and waited for completion (~30–60 mins).  
   - *![Screenshot - Scan Running](screenshots/3_scan_running.png)*  

4. **Reviewed Results**  
   - Checked vulnerabilities listed with severity ratings (Critical, High, Medium, Low).  
   - Noted **CVE IDs** and CVSS scores for each vulnerability.  
   - *![Screenshot - Scan Results](screenshots/4_results.png)*  

5. **Researched Fixes**  
   - Looked up vendor patches and configuration changes to mitigate issues.  
   - *![Screenshot - Research Fixes](screenshots/5_research.png)*  

## 📊 Findings Summary  

| Severity   | Count | Example Vulnerabilities |
|------------|-------|------------------------|
| Critical   | 3     | Remote Code Execution in SMBv1 (CVE-2017-0144) |
| High       | 5     | TLS/SSL Weak Cipher Suites, Outdated OpenSSL |
| Medium     | 8     | Outdated Browser Plugins, Insecure HTTP Headers |
| Low        | 4     | Missing HTTP Security Headers, Open Ports with No Service |

## 🔐 Key Learnings  
- **Vulnerability Scanning** helps identify potential security gaps before attackers exploit them.  
- **CVSS Scores** provide a standard way to measure severity.  
- Regular scans help in proactive security maintenance.  

## 💡 Best Practices for Vulnerability Management  
1. **Run scans regularly** — at least once a month.  
2. **Patch critical vulnerabilities immediately** to prevent exploitation.  
3. **Disable unused services/ports** to reduce attack surface.  
4. **Use strong encryption protocols** and disable weak ciphers.  
5. **Enable automatic updates** for OS and software.  
6. **Review scan reports** and maintain a vulnerability log.  
7. **Combine scanning with penetration testing** for deeper security assessment.  

## ✅ Conclusion  
This task provided hands-on experience in identifying system vulnerabilities using a professional security tool. The scan results highlighted several potential risks, ranging from outdated software to weak configurations. Understanding and mitigating these vulnerabilities is essential for improving system security and reducing the attack surface. Regular scanning combined with timely patching ensures a safer computing environment.  
