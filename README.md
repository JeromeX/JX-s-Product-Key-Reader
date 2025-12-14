# 🔑 Product Key Reader

A lightweight, portable Windows tool designed to quickly retrieve Microsoft Windows and Office product keys. Originally started as a PowerShell script, this project has been rewritten in C# for improved performance and stability.

> [!NOTE]
> The application interface is currently available in **German only**.

<div align="center">
  <img width="80%" src="https://github.com/user-attachments/assets/b2f75790-c7f6-4166-a31b-5ce2224e41d4" alt="Product Key Reader Screenshot" />
</div>

---

## 💻 Built With

* **C#** (Core Application)
* **HTML** (Report Formatting & Export)

## ✨ Features

* **🔍 Windows Recovery:** Reads the product key directly from the Registry (`DigitalProductId`).
* **🚀 Windows 11 Support:** Correctly detects Windows 11 based on the Build Number (even if the Registry reports "Windows 10").
* **📦 Office Support:** Scans for installed Office versions (including Click-to-Run & `WOW6432Node`).
* **📄 PDF & HTML Export:**
    * Exports the list as a cleanly formatted HTML file.
    * **PDF Export:** Utilizes `wkhtmltopdf` via a direct memory pipe (Stdin) for error-free generation without creating temporary files.
* **📋 Secure Copy:** Copies keys to the clipboard and automatically clears them after **30 seconds** (visual timer included).
* **🛠 Portable:** No installation required. Runs directly as an `.exe`.

## ⚙️ Requirements

* **OS:** Windows 10 or Windows 11
* **Runtime:** .NET Framework 4.7.2 (or newer)
* **Permissions:** Requires **Administrator privileges** (to read restricted Registry keys).
* **Optional (for PDF):** `wkhtmltopdf` must be installed or located in the application folder.

## 🚀 Installation & Usage

1.  Download the latest `ProductKeyReader.zip` from the **[Releases](../../releases)** page.
2.  **(Optional)** Place `wkhtmltopdf.exe` in the same folder to use the PDF function in portable mode.
3.  Start the program (Confirm the Admin/UAC prompt).
4.  Click on **Scan**.

## 🐛 Troubleshooting

**PDF is not being created:**
* Ensure that `wkhtmltopdf` is installed or the executable is in the app folder.
* **If installed:** Point the program to the correct path of `wkhtmltopdf.exe` if prompted.
* Your system might be missing the **Visual C++ Redistributables** (which are required by `wkhtmltopdf`).

## 📝 License & Credits

Developed by Malte Speck © 2025.
