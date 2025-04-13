# SQL_Note

## 📁 **Default Location of SQL Server 2022 Installation Media**

The default path is:

```
C:\Program Files (x86)\Microsoft SQL Server\160\Setup Bootstrap\SQLServer2022\
```

### 🔍 Contents in that folder:
- `Setup.exe` → this is what you use to run installation or removal
- `Logs\` → installation and uninstall logs
- Supporting files for setup and configuration

---

## ✅ How to Use It to Remove Instances

1. Open **Command Prompt as Administrator**
2. Navigate to the setup folder:
   ```bash
   cd "C:\Program Files (x86)\Microsoft SQL Server\160\Setup Bootstrap\SQLServer2022"
   ```

3. Run this to uninstall an instance:
   ```bash
   Setup.exe /Action=Uninstall /INSTANCENAME=MSSQLSERVER02
   ```
   Then repeat for:
   ```bash
   Setup.exe /Action=Uninstall /INSTANCENAME=MSSQLSERVER03
   ```

---

## 🛠 If That Folder Doesn't Exist

If it’s missing or was cleaned up, you’ll need to **re-download the SQL Server 2022 installer (ISO or EXE)**:

### 🔗 Official Download Link:
- [Download SQL Server 2022 Developer Edition (Free)](https://www.microsoft.com/en-us/sql-server/sql-server-downloads)

Choose **Developer** or **Express**, and you'll get a small installer (`SQL2022-SSEI-Dev.exe` or similar). When it runs, choose:

- **Download Media** → to get the full ISO
- Or **Basic Install** just to reinstall/remove

---

Need help navigating the installer options or mounting the ISO? Let me know — I can walk you through that too.
