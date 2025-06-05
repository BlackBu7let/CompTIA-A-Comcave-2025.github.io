<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CompTIA A+ 2025 Quiz</title>
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
            width: 100%;
        }
        .export-row {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 8px;
            margin-bottom: 24px;
            width: 100%;
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
        input[type="text"] {
            padding: 10px;
            font-size: 1.05rem;
            border-radius: 6px;
            border: none;
            outline: none;
            margin: 0 0 2px 0;
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
        .creator-fixed {
            position: fixed;
            left: 20px;
            bottom: 16px;
            color: #d7d4eb;
            font-size: 1.06rem;
            letter-spacing: 1px;
            opacity: 0.88;
            font-style: italic;
            z-index: 100;
            background: none;
        }
        #musicCtrl {
            position: fixed;
            top: 24px;
            right: 24px;
            z-index: 2222;
            background: rgba(70,23,143,0.75);
            padding: 10px 18px;
            border-radius: 12px;
            box-shadow: 0 3px 10px rgba(0,0,0,0.3);
            cursor: pointer;
            font-size: 1.2rem;
            display: flex;
            align-items: center;
            gap: 8px;
            user-select: none;
        }
        @media (max-width: 800px) {
            .review-block, #result { max-width: 98vw; }
            .info-link-box { font-size: 0.95rem; right: 3vw; bottom: 3vw; padding: 10px 6vw; }
            #question { font-size: 1.1rem; max-width: 99vw; }
            .quiz-title { font-size: 1.35rem; }
            #options { flex-direction: column; gap: 10px; }
            .creator-fixed { font-size: 0.95rem; left: 2vw; bottom: 2vw; }
        }
    </style>
</head>
<body>
    <!-- Hintergrundmusik: Quiz Show Background Music Loop by Alexander Blu -->
    <audio id="bgmusic" loop preload="auto">
      <source src="https://www.orangefreesounds.com/wp-content/uploads/2021/12/Quiz-show-background-music-loop.mp3" type="audio/mpeg">
      Dein Browser unterstützt kein HTML5-Audio.
    </audio>
    <div id="musicCtrl">
      <span id="musicIcon" style="font-size:1.3em;">🎵</span>
      <span id="musicStatus">Musik: Aus</span>
    </div>
    <script>
      const audio = document.getElementById('bgmusic');
      const ctrl = document.getElementById('musicCtrl');
      const status = document.getElementById('musicStatus');
      let playing = false;

      audio.onerror = function() {
        status.textContent = "Musik: Fehler";
        ctrl.style.opacity = 0.7;
      };

      ctrl.onclick = function() {
        if (playing) {
          audio.pause();
          status.textContent = "Musik: Aus";
        } else {
          audio.play().then(() => {
            status.textContent = "Musik: An";
          }).catch(e => {
            status.textContent = "Musik nicht erlaubt";
          });
        }
        playing = !playing;
      };

      // Wird in startQuiz() aufgerufen, um bei Quizstart Musik abzuspielen
      function playMusicOnce() {
        if (!playing) {
          audio.play().then(() => {
            status.textContent = "Musik: An";
            playing = true;
          }).catch(e => {
            status.textContent = "Musik nicht erlaubt";
          });
        }
      }
    </script>

    <div id="startScreen" class="start-screen">
        <h1 class="start-title">CompTIA A+ 2025 Quiz</h1>
        <div class="start-desc">
            Teste dein Wissen mit typischen Fragen zur CompTIA A+ (Core 1 & 2 & ältere).<br>
            Du hast <b>30 Sekunden</b> pro Frage.<br>
            Am Ende siehst du deine Punkte und kannst alle Antworten mit Lösungen vergleichen.<br>
        </div>
        <button class="start-btn" onclick="startQuiz()">Starten</button>
    </div>
    <div class="quiz-title" style="display:none;" id="quizTitle">CompTIA A+ 2025 Quiz</div>
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
    <div class="creator-fixed">
        Erstellt von Lucas Pakutka
    </div>
    <script>
        function shuffleArray(array) {
            for (let i = array.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [array[i], array[j]] = [array[j], array[i]];
            }
        }

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
    q: "Welches Medium verfügt über die höchste Speicherkapazität?",
    opts: ["ADVD-DL", "BCD-RW", "CCD-R", "DDVD-R"],
    ans: "DDVD-R"
},
{
    q: "Blu-ray-Discs haben folgende Kapazität:",
    opts: ["4,7 GB", "9 GB", "25 GB", "85 GB"],
    ans: "25 GB"
},
{
    q: "Welches der folgenden Medien wird auch mit Solid State bezeichnet?",
    opts: ["Bandlaufwerk", "DVD", "Flash-Card", "LS-120"],
    ans: "Flash-Card"
},
{
    q: "Was wird als optisches Medium bezeichnet?",
    opts: ["Floppy", "Blu-ray", "SSD", "Bandlaufwerk"],
    ans: "Blu-ray"
},
{
    q: "Sie möchten eine SSD in Ihr Notebook einbauen, aber der SATA-Steckplatz ist bereits belegt. Was kann allenfalls alternativ noch vorhanden sein für Ihr Anliegen?",
    opts: ["Interner USB-Anschluss", "Ein RAID-Anschluss", "Eine .M2-Schnittstelle", "Nichts, Sie können keine SSD mehr einbauen"],
    ans: "Eine .M2-Schnittstelle"
},
{
    q: "Welches der folgenden Speichermedien bietet die höchste Stoßfestigkeit?",
    opts: ["NAS-HDD", "Flash Card", "SATA-HDD", "SSD"],
    ans: "SSD"
},
{
    q: "Welches der folgenden Speichermedien hat eine Kapazität von 8,5 GB?",
    opts: ["CD-RW", "DL DVD", "Blu-ray", "DVD"],
    ans: "DL DVD"
},
{
    q: "Was überbietet eine 15.000-rpm-SAS-Festplatte in Sachen Lesegeschwindigkeit am ehesten?",
    opts: ["Compact Flash", "SSD", "Tape", "SD"],
    ans: "SSD"
},
{
    q: "Welcher Anschluss wird durch einen männlichen 9- oder 25-Pin-Stecker an der Rückseite eines Notebooks beschrieben?",
    opts: ["Parallele Schnittstelle", "Serielle Schnittstelle", "IEEE 1394-Schnittstelle", "USB 3.0-Anschluss"],
    ans: "Serielle Schnittstelle"
},
{
    q: "Was ist die empfohlene Maximallänge eines internen SATA-Kabels?",
    opts: ["45 cm", "60 cm", "100 cm", "300 cm"],
    ans: "100 cm"
},
{
    q: "Welche Schnittstelle unterstützt nur ein (1) Gerät pro Anschluss?",
    opts: ["RS-232", "USB 1.1", "SAS", "SATA 3,0 Gbit/s"],
    ans: "SATA 3,0 Gbit/s"
},
{
    q: "Welcher Standard wird verwendet, um die Anzahl Ladegeräte und -anschlüsse für mobile Geräte deutlich zu reduzieren?",
    opts: ["RS-232", "USB-C", "SATA", "Thunderbolt 4"],
    ans: "USB-C"
},
{
    q: "Sie möchten eine neue externe Disk an Ihr System anschließen. Dafür verwenden Sie einen USB 3.2 Gen 2x2-Anschluss. Welche maximalen Datenraten erlaubt dies?",
    opts: ["20 Gbps", "10 Gbps", "5 Gbps", "1 Gbps"],
    ans: "20 Gbps"
},
{
    q: "Ein Mainboard verfügt über einen AM4-Sockel. Welcher Prozessor passt in diesen Sockel?",
    opts: ["AMD Phenom", "AMD Ryzen", "Intel Xeon", "Intel Core i7"],
    ans: "AMD Ryzen"
},
{
    q: "Auf welcher Form der Datenübertragung basiert PCI-Express?",
    opts: ["Parallele Datenübertragung", "USB 2.0", "Serielle Punkt-zu-Punkt-Verbindung", "Interner PCI-Bus"],
    ans: "Serielle Punkt-zu-Punkt-Verbindung"
},
{
    q: "Welche Funktion macht die Installation einer CPU einfacher?",
    opts: ["Plug and Play", "Niedrigere Latenzen", "Zero Insertion Force", "Kühlkörper"],
    ans: "Zero Insertion Force"
},
{
    q: "Welches der folgenden RAM-Module weist 260 Pins auf?",
    opts: ["DDR1-SDRAM", "SO-DIMM", "DDR3-SDRAM", "SDR-DRAM"],
    ans: "SO-DIMM"
},
{
    q: "Die maximale Datenübertragungsrate von PCI 4.0 beträgt",
    opts: ["1324 GB/s", "8 GB/s", "15,76 GB/s", "31,51 GB/s"],
    ans: "31,51 GB/s"
},
{
    q: "Welcher RAM-Typ kann die Spezifikation PC3-10500 aufweisen?",
    opts: ["DDR2", "RDRAM", "SDRAM3", "DDR3"],
    ans: "DDR3"
},
{
    q: "Welcher Display-Typ benötigt zur Darstellung eine Hintergrundbeleuchtung?",
    opts: ["LCD", "LED", "CRT", "Plasma"],
    ans: "LCD"
},
{
    q: "Welche Schnittstellen werden normalerweise von einem KVM-Switch unterstützt?",
    opts: ["PS/2, VGA, USB", "DB25, DB9, PS/2", "PS/2, DB9, USB", "PS/2, VGA, DB25"],
    ans: "PS/2, VGA, USB"
},
{
    q: "Welche der folgenden Methoden nutzen Sie für gewöhnlich zur biometrischen Authentifikation?",
    opts: ["Passwort", "Verschlüsseltes Passwort", "RFID-SmartCard", "Fingerabdrucklesegerät"],
    ans: "Fingerabdrucklesegerät"
},
{
    q: "Welche Methode zum Eingeben von Daten erfordert die Authentifizierung des Benutzers mit einem Körperteil?",
    opts: ["Biologie", "Biometrie", "Autopsie", "Autometrie"],
    ans: "Biometrie"
},
{
    q: "Welches Gerät kann ein PAL-Signal einer externen Quelle decodieren?",
    opts: ["TV-Tuner-Karte", "Grafikkarte", "Videoschnittkarte", "Soundkarte"],
    ans: "TV-Tuner-Karte"
},
{
    q: "Welche Komponente muss bei intervallmäßigen Wartungsarbeiten an einem Laserdrucker ersetzt werden?",
    opts: ["Laderolle", "Scannerspiegel", "Trommeleinheit", "Tintenrestbehälter"],
    ans: "Trommeleinheit"
},
{
    q: "Welchen Druckertyp werden Sie für den Einsatz von mehrteiligen Formularen mit Durchschlag einsetzen?",
    opts: ["Einen Nadeldrucker", "Einen Thermoprinter", "Einen Tintenstrahldrucker", "Einen Laserdrucker"],
    ans: "Einen Nadeldrucker"
},
{
    q: "Wenn Sie einen Laserdrucker wegen eines Papierstaus öffnen, was trifft in diesem Moment zu?",
    opts: ["Der Laser ist heiß.", "Der Druckerspooler verliert alle Aufträge.", "Die Fixiereinheit ist heiß.", "Die Tonerkassette kann verrutschen."],
    ans: "Die Fixiereinheit ist heiß."
},
{
    q: "Ein Kunde meldet sich beim Techniker, weil sein Tintenstrahldrucker nicht mehr so klar wie bisher druckt. Wie kann der Techniker als Erstes versuchen, das Problem zu lösen?",
    opts: ["Tintenpatronen ersetzen", "Drucker kalibrieren", "Anderes Papier benutzen", "USB-Kabel ersetzen"],
    ans: "Drucker kalibrieren"
},
{
    q: "Wie wird bei einem Laserdrucker der Prozess des Fixierens von Toner auf das Papier genannt?",
    opts: ["Bonding", "Transferring", "Duplexing", "Fusing"],
    ans: "Fusing"
},
{
    q: "Welches Bauteil eines Laserdruckers bringt mithilfe von Hitze den Toner auf das Papier auf?",
    opts: ["Fixiereinheit", "Aufnahmerollen", "Papiertransferwalze", "Bildtrommel"],
    ans: "Fixiereinheit"
},
{
    q: "Was ist der hauptsächliche Grund dafür, dass Drucker von Zeit zu Zeit automatisch gereinigt werden?",
    opts: ["Längere Lebenszeit der Toner", "Entfernung von Tonerrückstanden", "Längere Lebenszeit des Druckers", "Schnellerer Druck"],
    ans: "Entfernung von Tonerrückstanden"
},
{
    q: "Wozu ist der 110/220-V-Umschalter an der Geräterückseite zuständig?",
    opts: ["Übertaktung für Spiele", "Lüftergeschwindigkeit", "Länderanpassung", "Computersperre"],
    ans: "Länderanpassung"
},
{
    q: "Ein Techniker nimmt einen Umbau in einem Computer vor, hat jedoch kein ESD-Armband zur Verfügung. Wie kann er sich am besten vor statischer Aufladung schützen?",
    opts: ["Das Metallgehäuse des Computers halten", "Das Stromkabel halten", "Die Schuhe ausziehen", "Den PC vom Strom nehmen"],
    ans: "Das Metallgehäuse des Computers halten"
},
{
    q: "Sie möchten die Datensicherheit auf Ihrem System erhöhen und konfigurieren darum die zwei vorhandenen Disks mit RAID. Welchen RAID-Level werden Sie unter diesen Anforderungen wählen?",
    opts: ["Level 0", "Level 1", "Level 5", "Level 10"],
    ans: "Level 1"
},
{
    q: "Sie möchten in Ihrem System mehr Arbeitsspeicher einsetzen. Auf dem bisherigen Speicher steht DDR4-3200. Welchen Speicherriegel nehmen Sie zur Aufrüstung?",
    opts: ["DDR4-3200", "DDR3-4800", "PC3-6400", "PC4-25600"],
    ans: "DDR4-3200"
},
{
    q: "Was kann in einem Notebook normalerweise nicht aufgerüstet werden?",
    opts: ["Grafikkarte", "Festplatte", "Arbeitsspeicher", "Wireless-Karte"],
    ans: "Grafikkarte"
},
{
    q: "Der Akku eines Laptops wird bei angeschlossenem Ladekabel nicht aufgeladen. Was ist vermutlich defekt?",
    opts: ["DC-in-Stecker", "Festplatte", "Kühlsystem", "Batterie"],
    ans: "Batterie"
},
{
    q: "Ein Benutzer möchte einen Paralleldrucker für sein Notebook nutzen. Was benötigt er dazu, wenn das Notebook keinen solchen Anschluss mehr hat?",
    opts: ["Splitter", "Portreplikator", "Wireless-Router", "Parallel-USB-Kabel"],
    ans: "Parallel-USB-Kabel"
},
{
    q: "Was kann in einem Laptop nur im ausgeschalteten Zustand, und wenn alle Stromquellen getrennt sind, installiert werden?",
    opts: ["PCMCIA-Geräte", "Express Card 54-Geräte", "SODIMM-Chip", "USB-Hub"],
    ans: "SODIMM-Chip"
},
{
    q: "Was verspricht einem Laptopbenutzer einen schnellen Systemstart?",
    opts: ["Viel Arbeitsspeicher", "Akku mit hoher Kapazität", "eSATA-Festplatte", "Solid State Drive"],
    ans: "Solid State Drive"
},
{
    q: "Welchen Druckertyp werden Sie für den Druck von Ersatzteilen auswählen?",
    opts: ["Einen 3D-Drucker", "Einen Thermoprinter", "Einen Tintenstrahldrucker", "Einen Laserdrucker"],
    ans: "Einen 3D-Drucker"
},
{
    q: "Wenn Sie einen Laserdrucker wegen eines Papierstaus öffnen, werden Sie welches Bauteil nicht berühren?",
    opts: ["Den Papiereinzug", "Die Fixiereinheit", "Die Tonerkassette", "Die Trommeleinheit"],
    ans: "Die Fixiereinheit"
},
{
    q: "Was für einen Anschluss suchen Sie in der Systemsteuerung, wenn Sie bei einem Drucker den Netzwerkanschluss überprüfen möchten?",
    opts: ["USBDot001", "LPT002", "File-Port", "WSD-Port"],
    ans: "WSD-Port"
},
{
    q: "Ein Kunde meldet sich beim Techniker, weil sein Tintenstrahldrucker nicht mehr druckt. Die Meldung lautet »Replace Waste-Tank«. Was tut er?",
    opts: ["Tintenrestbehälter austauschen", "Tintentanks ersetzen", "Intensivreinigung durchführen", "Den Drucker ersetzen"],
    ans: "Tintenrestbehälter austauschen"
},
{
    q: "Ihr Laserdrucker zieht einen feinen Streifen über das Papier, der schwarz ist. Was können Sie tun?",
    opts: ["Toner wechseln", "Coronadraht reinigen", "Papier muss anders beschaffen sein", "Trommeleinheit ersetzen"],
    ans: "Coronadraht reinigen"
},
{
    q: "Sie benötigen Ersatzmaterial für Ihren 3D-Drucker. Das bisherige Material haben Sie in Flaschen eingekauft. Welches Filament haben Sie benutzt?",
    opts: ["ABS", "PLA", "Resin", "3D-Tinte"],
    ans: "Resin"
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
            playMusicOnce();
            document.getElementById('startScreen').style.display = 'none';
            document.getElementById('quizTitle').style.display = '';
            document.querySelector('.quiz-container').style.display = '';
            document.getElementById('result').innerHTML = '';
            currentQuestion = 0;
            score = 0;
            userAnswers = [];
            shuffleArray(questions);
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
                if (timeLeft <= 0) {
                    userAnswers.push(null);
                    nextQuestion();
                }
            }, 1000);

            const q = questions[currentQuestion];
            let shuffledOpts = [...q.opts];
            shuffleArray(shuffledOpts);

            document.getElementById('question').innerHTML = 
                `<span style="font-size:1rem;opacity:.8;">Frage ${currentQuestion+1} von ${questions.length}</span><br><br>${q.q}`;
            document.getElementById('options').innerHTML = shuffledOpts.map((opt, idx) =>
                `<div class="option ${['red','blue','yellow','green'][idx % 4]}" onclick="checkAnswer('${opt}')">${opt}</div>`
            ).join('');
        }

        function checkAnswer(opt) {
            userAnswers.push(opt);
            if (opt === questions[currentQuestion].ans) score++;
            nextQuestion();
        }

        function nextQuestion() {
            currentQuestion++;
            if (currentQuestion < questions.length) loadQuestion();
            else showResult();
        }

        function showResult() {
            clearInterval(timerInterval);
            document.querySelector('.quiz-container').style.display = 'none';
            document.getElementById('quizTitle').style.display = 'none';
            document.getElementById('result').innerHTML = `
                <h2 style="text-align:center;">Quiz beendet! Punkte: ${score}/${questions.length}</h2>
                <div style="width:100%;display:flex;justify-content:center;">
                    <div class="btn-row">
                        <button onclick="showReview()">Lösungen anzeigen</button>
                        <button onclick="startQuiz()">Nochmal spielen</button>
                    </div>
                </div>
                <div style="width:100%;display:flex;justify-content:center;">
                    <div class="export-row">
                        <input type="text" id="userName" placeholder="Dein Name (optional)" maxlength="40">
                        <button onclick="exportResults()">Ergebnis exportieren</button>
                    </div>
                </div>
            `;

            // Konfetti-Animation, wenn alle Fragen richtig
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
                congrats.style.top = "20px";
                congrats.style.left = "50%";
                congrats.style.transform = "translate(-50%,0)";
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
                for (let i = 0; i < 120; i++) {
                    confetti.push({
                        x: Math.random() * window.innerWidth,
                        y: Math.random() * window.innerHeight - 400,
                        r: 7 + Math.random() * 12,
                        d: 2 + Math.random() * 6,
                        c: colors[Math.floor(Math.random() * colors.length)],
                        tilt: Math.random() * 10 - 10
                    });
                }
                let angle = 0;
                function drawConfetti() {
                    ctx.clearRect(0,0,confettiCanvas.width,confettiCanvas.height);
                    for (let i = 0; i < confetti.length; i++) {
                        let p = confetti[i];
                        ctx.beginPath();
                        ctx.ellipse(p.x, p.y, p.r, p.r/2, p.tilt, 0, 2 * Math.PI);
                        ctx.fillStyle = p.c;
                        ctx.fill();
                    }
                    updateConfetti();
                }
                function updateConfetti() {
                    angle += 0.01;
                    for (let i = 0; i < confetti.length; i++) {
                        let p = confetti[i];
                        p.y += p.d + Math.cos(angle + i);
                        p.x += Math.sin(angle) * 2;
                        p.tilt += Math.random() * 0.6 - 0.3;
                        if (p.y > window.innerHeight + 20) {
                            p.y = -10;
                            p.x = Math.random() * window.innerWidth;
                        }
                    }
                }
                let confettiInterval = setInterval(drawConfetti, 16);
                setTimeout(() => {
                    clearInterval(confettiInterval);
                    if (confettiCanvas) confettiCanvas.remove();
                    if (congrats) congrats.remove();
                }, 5000);
            }
            window.scrollTo(0,0);
        }

        function showReview() {
            let html = "<h2 style='text-align:center;'>Deine Lösungen:</h2>";
            for (let i = 0; i < questions.length; i++) {
                let correct = questions[i].ans;
                let user = userAnswers[i] === null ? "<i>Keine Antwort</i>" : userAnswers[i];
                let block = `<div class="review-block">
                    <b>Frage ${i+1}:</b><br>${questions[i].q}<br><br>
                    <b>Deine Antwort:</b> `;
                if (userAnswers[i] === correct) {
                    block += `<span class="review-correct">${user}</span>`;
                } else {
                    block += `<span class="review-wrong">${user}</span><br><b>Korrekt wäre:</b> <span class="review-correct">${correct}</span>`;
                }
                block += "</div>";
                html += block;
            }
            html += `
                <div style="width:100%;display:flex;justify-content:center;">
                    <div class="btn-row">
                        <button onclick="startQuiz()">Nochmal spielen</button>
                    </div>
                </div>
                <div style="width:100%;display:flex;justify-content:center;">
                    <div class="export-row">
                        <input type="text" id="userName" placeholder="Dein Name (optional)" maxlength="40">
                        <button onclick="exportResults()">Ergebnis exportieren</button>
                    </div>
                </div>
            `;
            document.getElementById('result').innerHTML = html;
            window.scrollTo(0,0);
        }

        function exportResults() {
            let name = document.getElementById('userName') ? document.getElementById('userName').value.trim() : '';
            let html = `<h2 style='text-align:center;'>CompTIA A+ 2025 Quiz Ergebnisse${name ? " von " + name : ""}</h2>`;
            html += `<p style='text-align:center;'><b>Punkte:</b> ${score} / ${questions.length}</p>`;
            for (let i = 0; i < questions.length; i++) {
                let correct = questions[i].ans;
                let user = userAnswers[i] === null ? "<i>Keine Antwort</i>" : userAnswers[i];
                let block = `<div style="background:#fff;color:#222;border-radius:8px;padding:16px 20px;margin-bottom:18px;box-shadow:0 2px 10px rgba(0,0,0,0.08);max-width:700px;margin-left:auto;margin-right:auto;">
                    <b>Frage ${i+1}:</b><br>${questions[i].q}<br><br>
                    <b>Deine Antwort:</b> `;
                if (userAnswers[i] === correct) {
                    block += `<span style="background:#26890c;color:#fff;padding:6px 16px;border-radius:7px;">${user}</span>`;
                } else {
                    block += `<span style="background:#db2b2b;color:#fff;padding:6px 16px;border-radius:7px;">${user}</span><br><b>Korrekt wäre:</b> <span style="background:#26890c;color:#fff;padding:6px 16px;border-radius:7px;">${correct}</span>`;
                }
                block += "</div>";
                html += block;
            }
            let blob = new Blob([`<html><head><meta charset="utf-8"><title>Quiz Ergebnisse</title></head><body style="font-family:sans-serif;background:#f8f8fa;padding:16px;">${html}</body></html>`], { type: "text/html" });
            let filename = `Quiz_Ergebnis${name ? "_" + name.replace(/[^a-z0-9äöüÄÖÜß]/gi, "_") : ""}.html`;
            let link = document.createElement("a");
            link.href = URL.createObjectURL(blob);
            link.download = filename;
            document.body.appendChild(link);
            link.click();
            setTimeout(() => { document.body.removeChild(link); }, 500);
        }
    </script>
</body>
</html>
