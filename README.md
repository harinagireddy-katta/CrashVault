# 🚀 CrashVault – Data Recovery System for Lost Files

**CrashVault** is a forensic data recovery system designed to retrieve **accidentally lost files** from **hard drives and USB devices** using **Kali Linux and Python**. This tool provides an efficient data recovery process with **60-70% accuracy**, supporting critical file formats: **PDFs, PPTs, Excel sheets, and Word documents**.

---

## 🛠️ Features
- **Forensic Data Recovery**: Recovers deleted/lost files from USB drives and hard disks.
- **Deep File System Scanning**: Ensures thorough recovery of lost data.
- **Metadata Analysis**: Enhances recovery accuracy by analyzing file signatures.
- **Selective File Type Recovery**: Supports **PDF, PPT, Excel, and Word documents**.
- **User-Friendly Interface**: Simple command-line based tool with clear recovery steps.

---

## 📋 Supported File Types
- **Documents**: DOC, XLS, PPT, PDF

---

## ⚙️ Requirements
- Kali Linux Operating System
- Python 3.7 or higher
- Administrator privileges
- Minimum 4GB RAM
- Available disk space for recovered files

---

## 🔽 Installation & Setup

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/yourusername/CrashVault.git
cd CrashVault
```

### **2️⃣ Install Dependencies**
Ensure you are running **Kali Linux** and install the required forensic tools:
```bash
sudo apt update
sudo apt install scalpel foremost testdisk -y
```

### **3️⃣ Run the Recovery Script**
```bash
python recovery_tool.py --drive /dev/sdX --output recovered_files/
```
🔹 Replace `/dev/sdX` with the correct drive (e.g., `/dev/sdb`).  
🔹 The recovered files will be stored in `recovered_files/`.  

---

## 🚦 Usage Instructions
1. **Identify the lost partition**:
   ```bash
   sudo fdisk -l
   ```
2. **Run the CrashVault recovery tool** with the specified drive.
3. **Extract recovered files** from the output directory.

---

## 💡 Tips for Best Results
1. **Stop Using the Drive**:
   - Immediately stop using the drive when data loss occurs.
   - Don't save new files to the drive.

2. **Choose Appropriate Scan**:
   - Quick Scan: For recently deleted files.
   - Deep Scan: For formatted drives or older deletions.

3. **Save Location**:
   - Always save recovered files to a different drive.
   - Ensure enough free space at the destination.

---

## 📝 Logging
- Logs are saved in `recovery.log`
- Contains detailed operation information
- Useful for troubleshooting

---

## 🤝 Contributing
We welcome contributions! Follow these steps:
1. **Fork this repo**
2. **Create a new branch** (`git checkout -b feature-name`)
3. **Commit your changes** (`git commit -m "Added feature"`)
4. **Push the changes** (`git push origin feature-name`)
5. **Create a pull request** 🚀

---

## ⚖️ Disclaimer
**CrashVault is for forensic and ethical recovery purposes only.** Ensure you have permission before scanning any storage device. The authors are not responsible for any data loss or damage.
