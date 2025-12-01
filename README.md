🔑 Product Key Reader
Ein leichtgewichtiges, portables Windows-Tool zum schnellen Auslesen von Microsoft Windows- und Office-Produktschlüsseln. Ursprünglich als PowerShell-Skript gestartet, 
wurde dieses Projekt für bessere Performance und Stabilität

<img width="1002" height="601" alt="2025-12-01 13_58_16-C# – Datei-Explorer" src="https://github.com/user-attachments/assets/cd1b62f8-6a41-40cf-a1d3-124ae1fa3943" />

**✨ Funktionen**
🔍 Windows-Erkennung: Liest den Produktschlüssel direkt aus der Registry (DigitalProductId).

🚀 Windows 11 Support: Erkennt Windows 11 korrekt anhand der Build-Nummer (auch wenn die Registry "Windows 10" meldet).

📦 Office-Unterstützung: Scannt nach installierten Office-Versionen (inkl. Click-to-Run & WOW6432Node).

**📄 PDF & HTML Export:**

Exportiert die Liste sauber formatiert als HTML.

**PDF-Export: Nutzt wkhtmltopdf über direkte Speicher-Pipe (Stdin) für fehlerfreie Erstellung ohne temporäre Dateien.**

📋 Sicheres Kopieren: Kopiert Schlüssel in die Zwischenablage und löscht diese automatisch nach 30 Sekunden (visueller Timer).

**🛠 Portabel: Keine Installation notwendig. Läuft direkt als .exe.**

**⚙️ Voraussetzungen**
Betriebssystem: Windows 10 oder Windows 11

Laufzeitumgebung: .NET Framework 4.7.2 (oder höher)

Rechte: Erfordert Administrator-Rechte (zum Lesen der Registry-Schlüssel).

Optional (für PDF): wkhtmltopdf muss installiert sein oder im Ordner liegen.

**🚀 Installation & Nutzung**
Lade die neueste ProductKeyReader.zip aus den Releases herunter.

(Optional) Lege wkhtmltopdf.exe in denselben Ordner, um die PDF-Funktion portabel zu nutzen.

Starte das Programm (Bestätige die Admin-Abfrage).

Klicke auf Scannen.

**🐛 Troubleshooting**
PDF wird nicht erstellt:

Stelle sicher, dass wkhtmltopdf installiert ist.

Falls installiert: Zeige dem Programm den Pfad zur wkhtmltopdf.exe, wenn du danach gefragt wirst.

Es fehlen eventuell die Visual C++ Redistributables auf deinem System (benötigt von wkhtmltopdf).

📝 Lizenz & Credits
Entwickelt von Malte Speck © 2025.
