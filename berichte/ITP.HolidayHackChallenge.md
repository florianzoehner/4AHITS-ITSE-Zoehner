# ITP Arbeitsbericht

Klasse: 4AHITS  
Team: Florian Zöhner, Alexander Hauser  
Fach: ITP2  
Datum: 05.12.2025

## Holiday Hack Challenge
 
### Augabe 1
 A
#### Lösung
Ins Terminal klicken ond "answer" eingeben.

![](../berichte/bilder/challange1.png)

### Aufgabe 2

#### Lösung
Teil 1:
Domain: \b(?:[a-zA-Z0-9-]+\.)+[a-zA-Z]{2,}\b
IP-Address: \d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3}
URL: [a-zA-Z0-9-]{0,61}[a-zA-Z0-9])?\.)+[A-Za-z]{2,}(?::\d{1,5})?(?:\/[^\s]*)?
Email: \b[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}\b
 
Teil 2:
Custom SED Command: s/\@/[@]/g; s/\./[.]/g; s/\:///[://]/g; s/\HTTP/[HXXP]/g;
