<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CompTIA A+ 2025 ComCave</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #46178f;
            color: #fff;
            margin: 0;
            padding: 0;
            min-height: 100vh;
        }
        .quiz-container {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            min-height: 83vh;
        }
        .quiz-title {
            text-align: center;
            font-size: 2.3rem;
            font-weight: bold;
            margin-bottom: 28px;
            letter-spacing: 1px;
            margin-top: 16px;
        }
        #question {
            text-align: center;
            font-size: 1.45rem;
            margin-bottom: 32px;
            margin-top: 10px;
            max-width: 650px;
        }
        #options {
            display: flex;
            flex-direction: row;
            flex-wrap: wrap;
            align-items: center;
            justify-content: center;
            gap: 16px;
            margin-bottom: 24px;
        }
        .option {
            margin: 0;
            padding: 15px 30px;
            cursor: pointer;
            border-radius: 5px;
            font-size: 18px;
            transition: transform 0.2s;
            display: inline-block;
            min-width: 210px;
            text-align: center;
            box-sizing: border-box;
        }
        .option:hover {
            transform: scale(1.05);
        }
        .blue { background-color: #1368ce; }
        .red { background-color: #db2b2b; }
        .yellow { background-color: #f7c948; color: #222; }
        .green { background-color: #26890c; }
        #timer {
            font-size: 24px;
            margin-top: 15px;
            margin-bottom: 10px;
            text-align: center;
        }
        .review-correct {
            background: #26890c;
            color: #fff;
            padding: 6px 16px;
            border-radius: 7px;
        }
        .review-wrong {
            background: #db2b2b;
            color: #fff;
            padding: 6px 16px;
            border-radius: 7px;
        }
        .review-block {
            background: #fff;
            color: #222;
            border-radius: 8px;
            padding: 16px 20px;
            margin-bottom: 18px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.08);
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }
        .btn-row {
            display: flex;
            flex-direction: row;
            justify-content: center;
            align-items: center;
            gap: 20px;
            margin-top: 32px;
            margin-bottom: 24px;
        }
        button, .start-btn {
            background: #1368ce;
            color: #fff;
            border: none;
            border-radius: 8px;
            padding: 14px 36px;
            font-size: 22px;
            margin-top: 0;
            cursor: pointer;
            transition: background 0.2s;
            display: inline-block;
        }
        button:hover, .start-btn:hover {
            background: #26890c;
        }
        #result {
            max-width: 760px;
            margin: 0 auto 40px auto;
            margin-top: 32px;
            background: none;
            overflow-y: auto;
            max-height: 85vh;
            scrollbar-width: thin;
        }
        .start-screen {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            text-align: center;
        }
        .start-title {
            font-size: 2.7rem;
            font-weight: bold;
            margin-bottom: 14px;
            margin-top: 0;
        }
        .start-desc {
            font-size: 1.15rem;
            margin-bottom: 28px;
            color: #d7d4eb;
            max-width: 440px;
        }
        .info-link-box {
            position: fixed;
            right: 18px;
            bottom: 18px;
            font-size: 1.05rem;
            z-index: 10;
            opacity: 0.92;
            background: #fff;
            color: #3c2371;
            border-radius: 12px;
            padding: 12px 18px;
            box-shadow: 0 3px 15px rgba(60,30,110,.13);
        }
        .info-link-box a {
            color: #3c2371;
            text-decoration: underline;
            margin-right: 0.8em;
        }
        .creator {
            text-align: center;
            color: #d7d4eb;
            margin: 42px 0 18px 0;
            font-size: 1.06rem;
            letter-spacing: 1px;
            opacity: 0.82;
            font-style: italic;
        }
        @media (max-width: 800px) {
            .review-block, #result { max-width: 98vw; }
            .info-link-box { font-size: 0.95rem; right: 3vw; bottom: 3vw; padding: 10px 6vw; }
            #question { font-size: 1.1rem; max-width: 99vw; }
            .quiz-title { font-size: 1.35rem; }
            #options { flex-direction: column; gap: 10px; }
        }
    </style>
</head>
<body>
    <div id="startScreen" class="start-screen">
        <h1 class="start-title">CompTIA A+ 2025 Comcave</h1>
        <div class="start-desc">
            Teste dein Wissen mit typischen Fragen zur CompTIA A+ (Core 1 & 2 & ältere).<br>
            Du hast <b>30 Sekunden</b> pro Frage.<br>
            Am Ende siehst du deine Punkte und kannst alle Antworten mit Lösungen vergleichen.<br>
        </div>
        <button class="start-btn" onclick="startQuiz()">Starten</button>
    </div>
    <div class="quiz-title" style="display:none;" id="quizTitle">CompTIA A+ 2025 ComCave</div>
    <div class="quiz-container" style="display:none;">
        <h2 id="question"></h2>
        <div id="options"></div>
        <div id="timer"></div>
    </div>
    <div id="result"></div>
    <div class="info-link-box">
        Original-Fragen:
        <a href="https://www.comptia.org/training/resources/practice-tests/comptia-a-1201-practice-questions" target="_blank">A+ 220-1101</a> |
        <a href="https://www.comptia.org/training/resources/practice-tests/comptia-a-1202-practice-questions" target="_blank">A+ 220-1102</a> |
        <a href="https://www.comptia.org/training/resources/practice-tests/comptia-a-1101-practice-questions" target="_blank">A+ 220-1001</a> |
        <a href="https://www.comptia.org/training/resources/practice-tests/comptia-a-1102-practice-questions" target="_blank">A+ 220-1002</a>
    </div>
    <div class="creator">
        Erstellt von Lucas Pakutka
    </div>
    <script>
        const questions = [
  {
    q: "Welche Technologie eignet sich am besten, um ein Gerät drahtlos mit einem Lautsprecher zu verbinden?",
    opts: ["Wi-Fi", "NFC", "5G", "Bluetooth"],
    ans: "Bluetooth"
},
{
    q: "Welche RAM-Technologie sollte für einen leistungsstarken Gaming-PC gewählt werden?",
    opts: ["Non-ECC", "Single Channel", "Registered", "DDR5"],
    ans: "DDR5"
},
{
    q: "Welcher Kabeltyp wird verwendet, um einen Bildschirm anzuschließen?",
    opts: ["DVI", "RJ45", "SATA", "USB 1.1"],
    ans: "DVI"
},
{
    q: "Welches Bauteil erkennt Eingaben auf einem Touchscreen-Monitor?",
    opts: ["Inverter", "Digitizer", "OLED", "LCD"],
    ans: "Digitizer"
},
{
    q: "Welches Cloud-Modell sollte eine Finanzorganisation wählen, wenn sie eine exklusive Cloud-Instanz benötigt?",
    opts: ["Hybrid", "Community", "Private", "Public"],
    ans: "Private"
},
{
    q: "Was verursacht am ehesten falsche Zeitanzeigen auf einem PC, trotz wiederholter Korrektur?",
    opts: ["Unseated RAM", "Stromkabel", "CMOS-Batterie", "Grafikkarte"],
    ans: "CMOS-Batterie"
},
{
    q: "Welche Technologie nutzt ein Smartphone, um an einem Zahlungsterminal zu bezahlen?",
    opts: ["RFID", "NFC", "802.11", "Bluetooth"],
    ans: "NFC"
},
{
    q: "Was sollte ein Techniker tun, wenn das Handy eines Nutzers nicht lädt, nachdem der Ladeanschluss geprüft wurde?",
    opts: ["Telefon neustarten", "Werkseinstellungen wiederherstellen", "Ein funktionierendes Kabel ausprobieren", "Zum Händler schicken"],
    ans: "Ein funktionierendes Kabel ausprobieren"
},
{
    q: "Wie sollte ein Techniker vorgehen, wenn ein Nutzer langsames Internet, hohe CPU-Auslastung und häufige Pop-ups meldet?",
    opts: ["Netzwerkteam informieren", "Neueste Treiber herunterladen", "Anti-Malware aktualisieren und scannen", "Wireless-Einstellungen prüfen"],
    ans: "Anti-Malware aktualisieren und scannen"
},
{
    q: "Welches Bauteil sollte ein Techniker ersetzen, wenn ein Laptop trotz getesteten Adapters langsam lädt?",
    opts: ["Akku", "RAM", "TPM", "Motherboard"],
    ans: "Akku"
},
{
    q: "Ein Benutzer kann auf seinem neuen Arbeitsplatz nicht auf Unternehmensressourcen zugreifen, die vorher zugänglich waren. Was sollte ein Techniker tun?",
    opts: ["Benutzer Adminrechte geben", "Firewall deaktivieren", "Arbeitsplatz zur Firmendomäne hinzufügen", "Gesichtserkennung aktivieren"],
    ans: "Arbeitsplatz zur Firmendomäne hinzufügen"
},
{
    q: "Welcher Prozess hilft einem IT-Spezialisten, Auswirkungen einer kritischen Anwendungs-Migration während eines Wartungsfensters zu bewerten?",
    opts: ["Endnutzerakzeptanz", "Risikobewertung", "Managergenehmigung", "Kollegenprüfung"],
    ans: "Risikobewertung"
},
{
    q: "Welche Malware zeichnet Anmeldedaten und Eingaben des Benutzers auf?",
    opts: ["Keylogger", "Trojaner", "Ransomware", "Rootkit"],
    ans: "Keylogger"
},
{
    q: "Welchen Punkt sollte ein Team zuerst prüfen, wenn ein geteilter Präsentations-Link nicht funktioniert?",
    opts: ["Versionsverlauf", "Browserkompatibilität", "Anzeige- und Freigabeberechtigungen", "Lizenzverwaltung"],
    ans: "Anzeige- und Freigabeberechtigungen"
},
{
    q: "Ein Benutzer löscht absichtlich Unternehmensdaten. Welcher Angriffstyp trifft zu?",
    opts: ["Whaling", "On-path-Angriff", "Insider-Bedrohung", "Spoofing"],
    ans: "Insider-Bedrohung"
},
{
    q: "Was sollte ein Techniker tun, wenn schädliche Aktivitäten nachts stattfinden?",
    opts: ["Gastkonten deaktivieren", "Anmeldezeiten beschränken", "Kontolaufzeit setzen", "Bildschirmschoner aktivieren"],
    ans: "Anmeldezeiten beschränken"
},
{
    q: "Was passiert, wenn ein Betriebssystem das EOL-Datum erreicht?",
    opts: ["Benutzeranmeldung nicht möglich", "OS-Kauf nicht möglich", "Keine Sicherheitsupdates mehr", "Neue Treiber erforderlich"],
    ans: "Keine Sicherheitsupdates mehr"
},
{
    q: "Was sollte ein Techniker nach Austausch eines Laptop-Motherboards tun, bevor das defekte Bauteil zurückgeschickt wird?",
    opts: ["ESD-Armband erden", "Akku und Adapter entfernen", "Innenraum reinigen", "Komponente in Antistatik-Beutel legen"],
    ans: "Innenraum reinigen"
},
{
    q: "Wie sollte man reagieren, wenn ein IT-Projekt zwei Tage verspätet ist und der Abteilungsleiter unzufrieden ist?",
    opts: ["An Management eskalieren", "Fristverlängerung beantragen", "Entschuldigen und Lösung anbieten", "Schriftliche Anfrage verlangen"],
    ans: "Entschuldigen und Lösung anbieten"
},
{
    q: "Ein Mitarbeiter erhält Beschwerden über Phishing-Mails, seit er eine Drittanbieter-E-Mail-App installiert hat. Was ist sofort zu tun?",
    opts: ["Postausgang prüfen", "Ungeprüfte App deinstallieren", "Kontakte löschen", "Nachrichten als Junk markieren"],
    ans: "Ungeprüfte App deinstallieren"
},
{
    q: "Ein Techniker muss ein defektes Netzteil in einem Server ersetzen. Der Server verfügt nur über ein Netzteil. Er hat zwei Prozessoren, die jeweils 100 W benötigen, fünf Festplatten mit jeweils 9 W und eine GPU mit 200 W. Welches Netzteil sollte der Techniker verwenden?",
    opts: ["375 W", "425 W", "325 W", "500 W"],
    ans: "500 W"
},
{
    q: "Ein Techniker hilft einem Benutzer beim Einrichten eines neuen Mobiltelefons. Der Benutzer konnte mit seinem vorherigen Handy durch Berühren des Zahlungssystems Einkäufe bezahlen. Welche Funktion sollte der Techniker aktivieren, damit dies auch mit dem neuen Handy funktioniert?",
    opts: ["PAN", "RFID", "NFC", "Bluetooth"],
    ans: "NFC"
},
{
    q: "Welche der folgenden Technologien bietet die SCHNELLSTE Verbindungsgeschwindigkeit?",
    opts: ["Glasfaser", "Satellit", "DSL", "Kabel"],
    ans: "Glasfaser"
},
{
    q: "Ein PC im Konferenzraum soll für Videopräsentationen an einen Großbildfernseher angeschlossen werden. Welcher Videoanschluss ist in dieser Umgebung am wahrscheinlichsten geeignet?",
    opts: ["Video Graphics Array", "Thunderbolt", "Digital Visual Interface", "High-Definition Multimedia Interface"],
    ans: "High-Definition Multimedia Interface"
},
{
    q: "Ein Techniker soll Festplatten von Firmenlaptops ordnungsgemäß entsorgen. Die Unternehmensrichtlinie verlangt, dass zur Datenvernichtung ein Hochleistungsmagnet verwendet wird. Welche Methode zur Datenvernichtung sollte der Techniker wählen?",
    opts: ["Entmagnetisieren", "Bohren", "Verbrennen", "Schreddern"],
    ans: "Entmagnetisieren"
},
{
    q: "Ein Techniker installiert M.2-Geräte in mehreren Arbeitsstationen. Was wird beim Einbau dieser Geräte benötigt?",
    opts: ["Luftfilterung", "Hitzebeständige Handschuhe", "Ergonomische Bodenmatten", "Elektrostatische Entladungsarmbänder"],
    ans: "Elektrostatische Entladungsarmbänder"
},
{
    q: "Ein Benutzer ruft beim IT-Helpdesk an und berichtet, dass alle Daten auf seinem Computer verschlüsselt sind. Es erscheint eine Pop-up-Nachricht, die eine Zahlung in Bitcoins verlangt, um die Daten zu entsperren. Womit ist der Computer des Benutzers höchstwahrscheinlich infiziert?",
    opts: ["Botnet", "Spyware", "Ransomware", "Rootkit"],
    ans: "Ransomware"
},
{
    q: "Welches der folgenden Betriebssysteme für Arbeitsstationen verwendet NTFS als Standard-Dateisystem?",
    opts: ["macOS", "Windows", "Chrome OS", "Linux"],
    ans: "Windows"
},
{
    q: "Welcher der folgenden Linux-Befehle zeigt ein Verzeichnis der Dateien an?",
    opts: ["chown", "ls", "chmod", "cls"],
    ans: "ls"
},
{
    q: "Ein Techniker will einen Laptop von einer Diagnose-DVD booten. Auf diesem System ist MS-Windows 8.1 installiert. Er ändert dazu im UEFI-BIOS die Bootreihenfolge so, dass zuerst vom internen DVD-Laufwerk gebootet werden soll. Dennoch startet das System MS-Windows. Welche Einstellung muss vorgenommen werden, damit dieses System vom internen DVD-Laufwerk bootet?",
    opts: ["Virtualisierung", "TPM", "UEFI BIOS Passwort", "Secure Boot"],
    ans: "Secure Boot"
},
{
    q: "Sie möchten den Papierverbrauch bei einem Multifunktionsdrucker reduzieren. Welche Konfigurationseinstellung sollte vorgenommen werden um diese Aufgabe zu erfüllen?",
    opts: ["Tintendruck in Sparmodus", "Gruppierter Ausdruck", "Duplexdruck", "Orientation (Ausrichtung)"],
    ans: "Duplexdruck"
},
{
    q: "Ein Techniker ist gerade dabei Hyper-V zu installieren als er die Fehlermeldung erhält, dass dieses Paket nicht installiert werden kann. Welche CPU-Eigenschaft sollte er überprüfen?",
    opts: ["Virtualisierungsunterstützung", "Hyperthreading", "Cachegrösse", "Anzahl der Kerne"],
    ans: "Virtualisierungsunterstützung"
},
{
    q: "Welche Art von Speicher wird bei L1 Cache Memory verwendet?",
    opts: ["SRAM", "SDRAM", "DRAM", "RDRAM"],
    ans: "SRAM"
},
{
    q: "Mehrere Pixel auf Ihrem LCD-Bildschirm sind immer schwarz! Mit welcher Massnahme lassen sich diese Pixelfehler beheben?",
    opts: ["Installieren der neuesten Videotreiber", "Ersetzen des LCD-Monitor", "Ändern der Bildschirmauflösung", "Neustart des Rechners"],
    ans: "Ersetzen des LCD-Monitor"
},
{
    q: "Welcher Speichertyp kommt bei Laptops vorwiegend zum Einsatz?",
    opts: ["ECC", "DDR2", "SDRAM", "SODIMM"],
    ans: "SODIMM"
},
{
    q: "Welcher Stecker ist ein sogenannter Mini-DIN Stecker?",
    opts: ["RCA", "PS/2", "DB9", "BNC"],
    ans: "PS/2"
},
{
    q: "Welche dieser Protokolle hat direkten Bezug zur Funktion 'Dateiübertragung unter MS Windows'?",
    opts: ["FTP", "SFTP", "LDAP", "SMB/CIFS"],
    ans: "SMB/CIFS"
},
{
    q: "Welcher Port wird verwendet für eine gesicherte Browserverbindung zu einem Webshop?",
    opts: ["3389", "80", "110", "443", "23"],
    ans: "443"
},
{
    q: "Für welchen Printertyp ist ein Wartungskit gedacht, in welchem sich eine Fixiereinheit (Fuser), eine Ladewalze (Transfer Roller) und eine Einzugswalze (Pickup Roller) befinden?",
    opts: ["Impactdrucker", "Thermodrucker", "Laserdrucker", "Tintenstrahldrucker (Inkjet)"],
    ans: "Laserdrucker"
},
{
    q: "Welcher Befehl überprüft die Festplatte auf logische Fehler?",
    opts: ["bootrec /fixmbr", "format /f", "bootrec /fixboot", "diskpart /fs", "chkdsk /f"],
    ans: "chkdsk /f"
},
{
    q: "Ein Laptop wird mit einem HDMI-Kabel an einen Fernseher angeschlossen. Es wird aber nicht der vollständige Bildschirm am Fernseher angezeigt. Welche Einstellung sollte in diesem Fall angepasst werden?",
    opts: ["Trapezkorrektur (Keystone)", "Wiederholungsrate", "Blick-/Sichtschutz (Privacy Filter)", "Auflösung"],
    ans: "Auflösung"
},
{
    q: "Ein Techniker ersetzt eine 250GB Festplatte gegen eine 2TB Festplatte. Nach der Installation erkennt das System die neue 2TB Festplatte als 250GB Platte. Was sollte der Techniker unternehmen um dieses Problem zu lösen?",
    opts: ["Aktualisieren des Betriebssystems (OS)", "Aktualisieren des BIOS", "Aktualisieren des Treibers", "Neuinstallation der Festplatte"],
    ans: "Aktualisieren des BIOS"
},
{
    q: "Wie heisst die Komponente, welche benötigt wird um die LCD Fluoreszenz-Hintergrundbeleuchtung mit Strom zu versorgen?",
    opts: ["Converter", "Diode", "Modulator", "Inverter", "Transceiver"],
    ans: "Inverter"
},
{
    q: "Welcher Adapter konvertiert analoge Signale in digitale Signale?",
    opts: ["S-Video zu RCA", "DVI-D zu HDMI", "HDMI zu VGA", "VGA zu DVI-D"],
    ans: "VGA zu DVI-D"
},
{
    q: "Welche/r Schnittstelle/Adapter ist bei einem Laptop sehr verbreitet und somit häufig anzutreffen?",
    opts: ["MicroBus", "PCI-X", "Micro Express", "PCI Express", "Mini PCIe"],
    ans: "Mini PCIe"
},
{
    q: "Über welchen Port werden gewöhnlich verschlüsselte Daten übertragen?",
    opts: ["TCP/443", "TCP/110", "UDP/53", "TCP/23"],
    ans: "TCP/443"
},
{
    q: "Was muss bei der Installation eines Digitizers ausgeführt werden?",
    opts: ["Muss kalibriert werden", "Muss mit dem Internet verbunden sein", "Es müssen die neusten SW-Treiber installiert sein", "Muss gereinigt werden"],
    ans: "Muss kalibriert werden"
},
{
    q: "Welcher RAM-Typ ist in der Lage weiterzuarbeiten auch wenn korrupte Daten vorhanden sind?",
    opts: ["Dual Channel", "Buffered", "ECC", "Non-Parity"],
    ans: "ECC"
},
{
    q: "Welche der folgenden Speichermedien werden verwendet, um ein RAID-5-Array zu bauen?",
    opts: ["Dual-Layer-DVDs", "SATA-Festplatten", "Blu-ray-Discs", "Flash-Laufwerke"],
    ans: "SATA-Festplatten"
},
{
    q: "Welches ist die wahrscheinlichste Ursache bei einem Drucker wenn auf jeder Seite Schlieren/Streifen auftreten?",
    opts: ["Bildtrommel", "Tonerkassette", "Zuführungsrollen", "Duplexeinheit"],
    ans: "Bildtrommel"
},
{
    q: "Welche Software startet den Bootvorgang bei einem Rechner sobald Strom zur Verfügung steht?",
    opts: ["BIOS", "MBR", "NTLDR", "OS Kernel"],
    ans: "BIOS"
},
{
    q: "Welcher Anschluss bei iOS Geräten ist in der Lage gleichzeitig Strom und Daten zu übertragen?",
    opts: ["Thunderbolt", "Lightning", "NFC", "Bluetooth", "FireWire"],
    ans: "Lightning"
},
{
    q: "In einer kleinen Firma müssen mehrere farbige Kopien von Verträgen ausgedruckt werden, welche dann an verschiedene Abteilungen und Kunden weitergeleitet werden. Mit welchem Drucker lassen sich diesen am schnellsten Ausdrucken?",
    opts: ["3D Drucker", "Laserdrucker", "Thermodrucker", "Matrix-/Nadeldrucker"],
    ans: "Laserdrucker"
},
{
    q: 'Ein Benutzer benötigt einen Rechner, welcher "Single-Thread"-Operationen möglichst schnell ausführen kann. Welche CPU-Eigenschaft ist die wichtigste um diese Anforderung zu erfüllen?',
    opts: ["Taktfrequenz", "Geschwindigkeit des Lüfters", "Anzahl Kerne", "Hyperthreading"],
    ans: "Taktfrequenz"
},
{
    q: "Wie wird ein Game Pad in der Regel an ein Mobile Device angeschlossen?",
    opts: ["TRRS", "microUSB", "Ethernet", "802.11n", "Bluetooth"],
    ans: "Bluetooth"
},
{
    q: "Welche der aufgeführten Geräte ist eine Ausgabeeinheit?",
    opts: ["Smart Card Leser", "Barcodeleser", "Webcam", "Tastatur", "Lautsprecher"],
    ans: "Lautsprecher"
},
{
    q: "Welcher Stecker wird normalerweise bei Glasfaserverbindungen verwendet?",
    opts: ["F-Connector (F-Stecker)", "RJ 11 und RJ45", "ST und LC", "BNC"],
    ans: "ST und LC"
},
{
    q: "Welches Gerät muss nach erfolgter Installation noch kalibriert werden?",
    opts: ["Videokarte", "Touch Screen", "Maus", "Tastatur"],
    ans: "Touch Screen"
},
{
    q: "Welche Bildschirmtechnologie stellt die beste Leuchtdichte von Farben zur Verfügung?",
    opts: ["OLED", "CRT", "Plasma", "LCD"],
    ans: "OLED"
},
{
    q: "Welcher Stecker mit 15 Kontakten wird normalerweise zur Übertragung von Videosignalen verwendet?",
    opts: ["VGA", "RCA", "HDMI", "DVI"],
    ans: "VGA"
},
{
    q: "Ein Benutzer plant die Speicherkapazität seines PC erweitern mit dem Anschluss externer Geräte. Welche dieser Anschlüsse ermöglicht ihm diesen Plan umzusetzen?",
    opts: ["Toslink", "IDE", "SATA", "eSATA"],
    ans: "eSATA" 
},
{
    q: "Sie entscheiden sich 802.11n einzusetzen. Welche Frequenz benutzt der WLAN-Standard 802.11n?",
    opts: ["2.4 GHz und/oder 5 GHz", "2.4 GHz", "2.4 GHz oder 5 GHz", "5 GHz"],
    ans: "2.4 GHz und/oder 5 GHz"
},
{
    q: "Welche der folgenden Kabeltypen sollten höchstwahrscheinlich verwendet werden um eine externe Festplatte anzuschliessen?",
    opts: ["Molex", "CAT6e", "SATA", "HDMI", "USB 3.0"],
    ans: "USB 3.0" 
},
{
    q: "Welches dieser unterschiedlichen Internetverbindungstypen hat eine signifikant höhere Latenzzeit (Verzögerung) als alle anderen Verbindungstypen?",
    opts: ["Kabelanschluss", "Glasfaserverbindung", "DSL-Anschluss", "Satellitenverbindung"],
    ans: "Satellitenverbindung"
},
{
    q: "Unter normalen Umständen verfügt welcher der folgenden Wirelessstandards (WLAN) die geringste Übertragungsrate im 2,4 GHz Frequenzbereich.",
    opts: ["802.11g", "802.11n", "802.11b", "802.11a"],
    ans: "802.11b"
},
{
    q: "Eine Benutzerin möchte ihren PC aufrüsten. Sie möchte eine USB 3.0 Karte, eine neue Videokarte, eine Soundkarte und eine neue Netzwerkkarte (NIC) einbauen. Welche neue Komponente macht es höchstwahrscheinlich nötig auch das Netzteil zu erneuern?",
    opts: ["Videokarte", "USB 3.0 Karte", "Netzwerkkarte", "Soundkarte"],
    ans: "Videokarte"
},
{
    q: "Ein Techniker ist gerade dabei ein System aufzusetzen, welches als HTPC (Home Theater Personal Computer, auch Media Center PC) genutzt werden soll. Welchen Formfaktor sollte der Techniker hinsichtlich der Grösse/Abmessungen dieses Systems wählen?",
    opts: ["ATX", "AT", "Micro-ATX", "Mini-ITX"],
    ans: "Mini-ITX"
},
{
    q: "Welches serielle Interface ist in der Lage maximal 480 Mb/s zu übertragen?",
    opts: ["9 Pin RS-232", "USB 1.1", "USB 3.0", "Centronics Schnittstelle", "USB 2.0"],
    ans: "USB 2.0"
},
{
    q: "Welches Protokoll wird verwendet um Dateien zwischen Rechner mit MAC OS und Windows OS über das LAN auszutauschen?",
    opts: ["SSH", "IMAP", "RDP", "SMB"],
    ans: "SMB"
},
{
    q: "Sie möchten den Temperaturverlauf der internen Festplatte während 24 Stunden überwachen. Welche der angebotenen Möglichkeiten erlaubt Ihnen diese Aufgabe?",
    opts: ["USB-Monitor", "S.M.A.R.T.", "MS-Windows Performance-Monitor", "ACPI", "Integrierte BIOS Diagnosefunktionen"],
    ans: "S.M.A.R.T."
},
{
    q: "Welches dieser Anschlüsse ist typisch für ein NAS?",
    opts: ["FireWire", "Seriell", "USB", "Ethernet", "eSATA"],
    ans: "Ethernet"
},
{
    q: "Welcher Standard erlaubt das Speichern von Daten ausserhalb des Gerätegehäuses?",
    opts: ["SATA", "PCIe", "eSATA", "PCI"],
    ans: "eSATA"
},
{
    q: "Wie lautet die Bezeichnung, wenn ein Smart Phone einen Internetzugang (Internetrouter) zur Verfügung stellt?",
    opts: ["Tethering", "Switching", "Redirecting", "Convergence", "Encapsulating"],
    ans: "Tethering"
},
{
    q: "Ein Techniker schliesst einen zweiten Bildschirm an einen Arbeitsplatzrechner an. Dieser neue Bildschirm steht rechts vom bestehenden Monitor. Welche Bildschirmeinstellung muss angepasst werden, damit der Mauszeiger wie gewohnt von links nach rechts vom ersten zum zweiten (neuen) Monitor bewegt werden kann?",
    opts: ["Position", "Rotation", "Bildschirmauflösung", "Bilschirmgrösse"],
    ans: "Position"
},
{
    q: "Die Abmessungen eines Laptop sind in der Regel zu gering so dass bei einer solchen Tastatur der separate Ziffernblock fehlt. Mit welcher speziellen Taste auf der Laptoptastatur lassen sich diese fehlenden Tasten und Funktionen dennoch wählen?",
    opts: ["Fn", "Alt Gr (Sys)", "Control (Ctrl)", "Alt"],
    ans: "Fn"
},
{
    q: "Der IT-Leiter möchte die Sicherheit beim Webauftritt der Firma erhöhen um sogenannten \"Man-in-the-Middle\"-Attacken vorzubeugen. Welches Internetprotokoll sollte implementiert werden um diese Anforderung zu erfüllen?",
    opts: ["Telnet", "SMTP", "IMAP", "HTTPS"],
    ans: "HTTPS"
},
{
    q: "Welcher digitale Übertragungsdienst kann über bestehende (alte) Kupferleitungen betrieben werden und ist der Vorgänger der xDSL-Übertragungsdienste?",
    opts: ["Ethernet", "ISDN", "Analoge Telefone", "Kabel TV"],
    ans: "ISDN"
}



];

let currentQuestion = 0, score = 0, timerInterval;
let userAnswers = [];

function startQuiz() {
    document.getElementById('startScreen').style.display = 'none';
    document.getElementById('quizTitle').style.display = '';
    document.querySelector('.quiz-container').style.display = '';
    document.getElementById('result').innerHTML = '';
    currentQuestion = 0;
    score = 0;
    userAnswers = [];
    loadQuestion();
    window.scrollTo(0,0);
}

function loadQuestion() {
    clearInterval(timerInterval);
    let timeLeft = 30;
    document.getElementById('timer').textContent = `Zeit: ${timeLeft}`;
    window.scrollTo(0, 0);

    timerInterval = setInterval(() => {
        timeLeft--;
        document.getElementById('timer').textContent = `Zeit: ${timeLeft}`;
        if(timeLeft <= 0) {
            userAnswers.push(null);
            nextQuestion();
        }
    }, 1000);

    const q = questions[currentQuestion];
    document.getElementById('question').textContent = q.q;
    document.getElementById('options').innerHTML = q.opts.map((opt, idx) =>
        `<div class="option ${['red', 'blue', 'yellow', 'green'][idx % 4]}" onclick="checkAnswer('${opt}')">${opt}</div>`
    ).join('');
}

function checkAnswer(opt) {
    userAnswers.push(opt);
    if(opt === questions[currentQuestion].ans) score++;
    nextQuestion();
}

function nextQuestion() {
    currentQuestion++;
    if(currentQuestion < questions.length) loadQuestion();
    else showResult();
}

function showResult() {
    clearInterval(timerInterval);
    document.querySelector('.quiz-container').style.display = 'none';
    document.getElementById('quizTitle').style.display = 'none';
    document.getElementById('result').innerHTML = `
        <h2 style="text-align:center;">Quiz beendet! Punkte: ${score}/${questions.length}</h2>
        <div class="btn-row">
            <button onclick="showReview()">Lösungen anzeigen</button>
            <button onclick="startQuiz()">Nochmal spielen</button>
        </div>
        <div id="exportArea"></div>
    `;
    renderExportBlock();

    // Animation, falls alles richtig:
    if (score === questions.length) {
        let confettiCanvas = document.createElement("canvas");
        confettiCanvas.id = "confetti";
        confettiCanvas.style.position = "fixed";
        confettiCanvas.style.top = 0;
        confettiCanvas.style.left = 0;
        confettiCanvas.style.width = "100vw";
        confettiCanvas.style.height = "100vh";
        confettiCanvas.style.pointerEvents = "none";
        confettiCanvas.style.zIndex = 1000;
        document.body.appendChild(confettiCanvas);

        let congrats = document.createElement("div");
        congrats.textContent = "Glückwunsch! Alle Fragen richtig!";
        congrats.style.position = "fixed";
        congrats.style.top = "35%";
        congrats.style.left = "50%";
        congrats.style.transform = "translate(-50%,-50%)";
        congrats.style.background = "rgba(255,255,255,0.97)";
        congrats.style.color = "#46178f";
        congrats.style.fontSize = "2.2rem";
        congrats.style.fontWeight = "bold";
        congrats.style.padding = "24px 36px";
        congrats.style.borderRadius = "18px";
        congrats.style.zIndex = 1001;
        congrats.style.boxShadow = "0 6px 48px #0002";
        document.body.appendChild(congrats);

        let ctx = confettiCanvas.getContext("2d");
        confettiCanvas.width = window.innerWidth;
        confettiCanvas.height = window.innerHeight;
        let confetti = [];
        let colors = ["#f7c948","#db2b2b","#1368ce","#26890c","#fff85a","#f76a1a","#a57aff"];
        for(let i=0; i<120; i++) {
            confetti.push({
                x: Math.random()*window.innerWidth,
                y: Math.random()*window.innerHeight-400,
                r: 7+Math.random()*12,
                d: 2+Math.random()*6,
                c: colors[Math.floor(Math.random()*colors.length)],
                tilt: Math.random()*10-10
            });
        }
        let angle = 0;
        function drawConfetti() {
            ctx.clearRect(0,0,confettiCanvas.width,confettiCanvas.height);
            for(let i=0;i<confetti.length;i++) {
                let p = confetti[i];
                ctx.beginPath();
                ctx.ellipse(p.x, p.y, p.r, p.r/2, p.tilt, 0, 2*Math.PI);
                ctx.fillStyle = p.c;
                ctx.fill();
            }
            updateConfetti();
        }
        function updateConfetti() {
            angle += 0.01;
            for(let i=0;i<confetti.length;i++) {
                let p = confetti[i];
                p.y += p.d + Math.cos(angle + i);
                p.x += Math.sin(angle) * 2;
                p.tilt += Math.random()*0.6-0.3;
                if(p.y > window.innerHeight+20) {
                    p.y = -10;
                    p.x = Math.random()*window.innerWidth;
                }
            }
        }
        let confettiInterval = setInterval(drawConfetti, 16);

        setTimeout(()=>{
            clearInterval(confettiInterval);
            if(confettiCanvas) confettiCanvas.remove();
            if(congrats) congrats.remove();
        }, 5000);
    }

    window.scrollTo(0,0);
}

// Exportbereich als eigener Block, damit auch nach showReview() sichtbar
function renderExportBlock() {
    document.getElementById("exportArea").innerHTML = `
        <div style="display:flex;flex-direction:column;align-items:center;margin:40px 0 30px 0;">
            <input id="exportName" type="text" placeholder="Dein Name (optional)" style="padding:10px 18px;font-size:1.2rem;border-radius:7px;border:none;margin-bottom:15px;width:270px;max-width:90%;">
            <button onclick="exportResultsHTML()" style="font-size:1.05rem;">Ergebnisse exportieren</button>
        </div>
    `;
}

// Der Export als HTML-Design wie die Lösungsausgabe
function exportResultsHTML() {
    let userName = document.getElementById("exportName").value.trim();
    let html = `
<!DOCTYPE html>
<html lang="de">
<head>
<meta charset="UTF-8">
<title>CompTIA A+ Quiz Ergebnisse</title>
<style>
body{background:#faf8ff;font-family:Poppins,sans-serif;color:#2b254a;padding:30px;}
h2{text-align:center;}
.result-summary{background:#fff3;margin:0 auto 35px auto;border-radius:9px;padding:18px 24px;max-width:520px;font-size:1.25em;}
.review-block{background:#fff;color:#222;border-radius:8px;padding:16px 20px;margin-bottom:18px;box-shadow:0 2px 10px #3c237119;max-width:700px;margin-left:auto;margin-right:auto;}
.review-correct{background:#26890c;color:#fff;padding:6px 16px;border-radius:7px;}
.review-wrong{background:#db2b2b;color:#fff;padding:6px 16px;border-radius:7px;}
</style>
</head>
<body>
    <h2>CompTIA A+ Quiz Ergebnisse</h2>
    <div class="result-summary">
        ${userName ? `Name: <b>${escapeHTML(userName)}</b><br>` : ""}
        Gesamtpunktzahl: <b>${score} / ${questions.length}</b>
    </div>
`;
    for(let i = 0; i < questions.length; i++) {
        let correct = questions[i].ans;
        let user = userAnswers[i] === null ? "<i>Keine Antwort</i>" : escapeHTML(userAnswers[i]);
        let block = `<div class="review-block">
            <b>Frage ${i+1}:</b><br>${escapeHTML(questions[i].q)}<br><br>
            <b>Deine Antwort:</b> `;
        if(userAnswers[i] === correct) {
            block += `<span class="review-correct">${user}</span>`;
        } else {
            block += `<span class="review-wrong">${user}</span> <br><b>Korrekt wäre:</b> <span class="review-correct">${escapeHTML(correct)}</span>`;
        }
        block += "</div>";
        html += block;
    }
    html += "</body></html>";

    // Dateiname festlegen
    let filename = "comptia-a-plus-quiz-ergebnisse";
    if(userName) {
        let clean = userName.trim()
            .replace(/\s+/g,"_")           // Leerzeichen zu _
            .replace(/[^a-zA-Z0-9_-]/g,"") // alles außer Buchstaben, Ziffern, _ und - entfernen
            .substring(0,32);              // Max 32 Zeichen für Lesbarkeit
        if(clean.length > 0) filename += "_" + clean;
    }
    filename += ".html";

    let blob = new Blob([html], {type: "text/html"});
    let a = document.createElement("a");
    a.href = URL.createObjectURL(blob);
    a.download = filename;
    document.body.appendChild(a);
    a.click();
    document.body.removeChild(a);
}

// Hilfsfunktion zur HTML-Escaping für Nutzereingaben und Fragen/Texte
function escapeHTML(str) {
    return (str+"")
      .replace(/&/g,"&amp;")
      .replace(/</g,"&lt;")
      .replace(/>/g,"&gt;")
      .replace(/"/g,"&quot;")
      .replace(/'/g,"&#039;");
}

function showReview() {
    let html = "<h2 style='text-align:center;'>Deine Lösungen:</h2>";
    for(let i = 0; i < questions.length; i++) {
        let correct = questions[i].ans;
        let user = userAnswers[i] === null ? "<i>Keine Antwort</i>" : userAnswers[i];
        let block = `<div class="review-block">
            <b>Frage ${i+1}:</b><br>${questions[i].q}<br><br>
            <b>Deine Antwort:</b> `;
        if(userAnswers[i] === correct) {
            block += `<span class="review-correct">${user}</span>`;
        } else {
            block += `<span class="review-wrong">${user}</span> <br><b>Korrekt wäre:</b> <span class="review-correct">${correct}</span>`;
        }
        block += "</div>";
        html += block;
    }
    html += `<div class="btn-row">
        <button onclick="startQuiz()">Nochmal spielen</button>
    </div>
    <div id="exportArea"></div>
    `;
    document.getElementById('result').innerHTML = html;
    renderExportBlock();
    window.scrollTo(0,0);
}
</script>
</body>
</html>
