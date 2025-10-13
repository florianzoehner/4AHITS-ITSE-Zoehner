

---

# Arbeitsbericht – GitHub & VS Code unter Kali Linux

**Datum:** 06.10.2025
**Autor:** Florian Zöhner
<br>
<br>
<br>
Aufgabenstellung:<br>
 
- Installiere Kali und Metasploitable (falls noch nicht geschehen)
- Stelle beide VMs auf Bridged ins Labor-Netz
- Installiere Visual Studio Code auf Kali Linux
- Klone das Github Projekt in Kali, nimm mit VS Code eine Änderung im Markdown vor, führe add, commit und push durch und prüfe ob die Änderungen in der generierten html Seite ankommen (kurze Wartezeit)
- Nimm nun über die GitHub Oberfläche eine Änderung vor und prüfe ob diese per git pull in den Klon auf Kali übernommen werden.
- Dokumentiere alles wesentliche in einem Arbeitsbericht. <br>
<br>
<br>
<br>
Lösung: <br>
 <br>
Als erstes habe ich Kali Linux und Metasploitable als virtuelle Maschinen installiert. Beide VMs habe ich so eingestellt, dass sie im Bridged-Modus laufen, damit sie im Labor-Netzwerk jeweils eine eigene IP-Adresse erhalten und miteinander kommunizieren können. Anschließend habe ich mit den Befehlen ifconfig und ip addr überprüft, ob die Netzwerkkonfiguration stimmt. Dann habe ich per ping die Erreichbarkeit zwischen den zwei VMs bestätigt.<br>
 
Danach habe ich auf meinem Kali-System Visual Studio Code installiert. Dazu habe ich das offizielle Repository von Microsoft eingebunden, die Paketlisten aktualisiert und das Paket „code“ installiert. Mit dem Befehl code konnte ich anschließend überprüfen, dass die Installation erfolgreich war.<br>
  
Anschließend habe ich das GitHub‑Repository **4AHITS‑ITSE‑Zoehner** per **SSH** geklont. 
Dafür habe ich mit dem Befehl `ssh-keygen` einen SSH‑Schlüssel erzeugt und den öffentlichen Schlüssel bei GitHub in den SSH‑Einstellungen hinterlegt. <br>
 
Das Repository wurde dann mit  `git clone git@github.com:florianzoehner/4AHITS-ITSE-Zoehner.git` auf mein System geholt. 
Mit `code .` habe ich das Projekt in VS Code geöffnet, die Datei `README.md` bearbeitet und meine Änderung gespeichert. 
Anschließend nutzte ich `git add .`, `git commit -m "Änderung in Markdown-Datei am 06.10.2025"` und `git push`, um die Änderung per SSH in das Remote‑Repository zu übertragen. 
Um auch den anderen Weg zu testen, habe ich über die GitHub-Weboberfläche direkt eine weitere Änderung an derselben Datei vorgenommen. Diese Änderung habe ich anschließend mit git pull in mein lokales Repository auf Kali übernommen. Dadurch waren die online durchgeführten Anpassungen sofort auch in meiner lokalen Kopie sichtbar.




