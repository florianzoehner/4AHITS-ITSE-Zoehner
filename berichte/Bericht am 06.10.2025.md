

---

# Arbeitsbericht – GitHub & VS Code unter Kali Linux

**Datum:** 06.10.2025
**Autor:** Florian Zöhner

Aufgabenstellung:
 
- Installiere Kali und Metasploitable (falls noch nicht geschehen)
- Stelle beide VMs auf Bridged ins Labor-Netz
- Installiere Visual Studio Code auf Kali Linux
- Klone das Github Projekt in Kali, nimm mit VS Code eine Änderung im Markdown vor, führe add, commit und push durch und prüfe ob die Änderungen in der generierten html Seite ankommen (kurze Wartezeit)
- Nimm nun über die GitHub Oberfläche eine Änderung vor und prüfe ob diese per git pull in den Klon auf Kali übernommen werden.
- Dokumentiere alles wesentliche in einem Arbeitsbericht.
 
Bei dieser Aufgabe habe ich unter Kali Linux Visual Studio Code installiert und anschließend das GitHub‑Repository **4AHITS‑ITSE‑Zoehner** per **SSH** geklont. 
Dafür habe ich mit dem Befehl `ssh-keygen` einen SSH‑Schlüssel erzeugt und den öffentlichen Schlüssel bei GitHub in den SSH‑Einstellungen hinterlegt. 
 
Das Repository wurde dann mit  `git clone git@github.com:florianzoehner/4AHITS-ITSE-Zoehner.git` auf mein System geholt. 
Mit `code .` habe ich das Projekt in VS Code geöffnet, die Datei `README.md` bearbeitet und meine Änderung gespeichert. 
Anschließend nutzte ich `git add .`, `git commit -m "Änderung in Markdown-Datei am 06.10.2025"` und `git push`, um die Änderung per SSH in das Remote‑Repository zu übertragen. 
Danach habe ich im Browser eine weitere Änderung direkt über die GitHub‑Weboberfläche an derselben Datei vorgenommen.
Um diese Änderung im lokalen Klon sichtbar zu machen, führte ich `git pull` aus, und die Änderung wurde erfolgreich übernommen und war lokal sichtbar. 




