# Physical-Computing

# LED - Lichtemittierende Diode
(*Light emitting diode*)
 &nbsp;
 
 ![LED Gehäuse](https://res.cloudinary.com/rsc/image/upload/b_rgb:FFFFFF,c_pad,dpr_1.0,f_auto,h_843,q_auto,w_1500/c_pad,h_843,w_1500/F2285988-01?pgw=1&pgwact=1)
 
---
### **1) Wofür brauche ich LEDs?**
---

- **Glühbirnen** (*Lightbulbs*) - z.B. im Haushalt

- **Flutlichter** (*Flooding lights*)  -  z.B. auf Baustellen, Sportanlagen etc.
- **LED Panels**  -  z.B. in Büros 
- **Scheinwerfer** (*Spotlights*)  -   z.B. für Film, Autos etc.
- **Leuchtreklame**  -  z.B. Schilder

---
### **2) Wie benutze ich LEDs?**
---
 &nbsp;
Um mit LED Birnen Licht zu erzeugen werden grundlegend die **LED-Birne**, ein **Strombegrenzungswiderstand** (*Resistor*) und natürlich eine **Energiequelle** gebraucht.

### Der Anschluss funktioniert wie folgt :


- Die LED wird an eine Energiequelle (z.B. Batterie) angeschlossen/gelötet

- LEDs benötigen eine bestimmte Durchlassungsspannung (*FV*) um zu leuchten
- Moderne LEDs sind unabhängig von ihrer Farbe alle mit einer *Durchlassspannung* von ca. *3,3 V* ausgestattet.
- Besitzt die Energiequelle eine höhere *Versorgungsspannung* als die LEDs benötigen (*Volt (V)*) :
-- schmort LED durch
- daher : Einbau von Widerstand (*Resistor*)
-- dieser lässt nur eine gewisse Zufuhr an Energie an die LED
-- z.B. von *12V* erreichen letztendlich *2V* die LED
- anhand der LED lässt sich erkennen was du verbinden musst, damit die Verbindung funktioniert:
-- Das Gehäuse ist auf einer Seite flach = *negative Seite*
-- Der Draht ist auf einer Seite länger = *positive Seite*
-- nun kann man die Drahtenden mit der richtigen Polarität an den Energieträger oder den *Strombegrenzungswiderstand* anschließen
- möglich : mehrere LEDs miteinander verknüpfen (*LED Strip*)
-- max. werden 3 LEDs aneinandergereiht
-- danach folgt das Widerstandselement
-- in dieser Abfolge lässt sich eine Kette bilden mit immer *3 LEDs und dem jeweiligen Strombegrenzungswiderstand* folgend

### So findet man den richtigen *Resistor* für die LEDs :
 &nbsp;
Wie bereits erwähnt, wird ein Strombegrenzungswiderstand benötigt, damit eine höhere Energiequelle nicht die LEDs durchschmort. Da es unterschiedliche Typen von LEDs auf dem Markt gibt, ist es essenziell herauszufinden, welchen Resistor für welche Art von LED verwendet werden muss, um eine erfolgreiche Energieweiterlung zu ermöglichen.
 &nbsp;

### Dazu kann man 2 Methoden verwenden :
##### - Die theoretische Methode mit Hilfe einer Berechnung
 &nbsp;
**R** = (Versorgungsspannung **VS** - LED-Durchlassspannung **VF**) / LED-Strom **I**
 &nbsp;
 - Hier ist R der fragliche Widerstand in Ohm

- Vs ist der Versorgungsspannungs-Eingang der LED
- VF ist die LED vorwärts, die tatsächlich die minimale Versorgungsspannung ist, die eine LED benötigt, um mit optimaler Helligkeit zu leuchten.
- LED-Strom oder I bezieht sich auf die Nennstromstärke der LED und kann je nach Spezifikation der ausgewählten LED zwischen 20 mA und 350 mA liegen. Dies muss in der Formel in Ampere umgerechnet werden, damit 20 mA zu 0,02 A, 350 mA zu 0,35 A usw. werden.

Hier wird dir die Berechnung abgenommen:
<https://leds-and-more.de/Widerstandsrechner>
 &nbsp;
##### - Die praktische Methode durch Erprobung
 &nbsp;
 Man braucht eine verstellbare/variable Energiequelle, verstellbarer/variabler Strombegrenzungswiderstand und natürlich LEDs :
 - zuerst stellt man das Energiegerät auf die Spannungszufuhr um, die man für seine Endenergiequelle nutzen möchte
 
- man schließt den *Resistor* an
- LED wird angeschlossen
- am Resitstor stellt oder erhöht man die Zufuhr, um zu erfahren, wann es ausschlägt und somit nicht tauglich für die LED ist 
 &nbsp;
---
### **3) Was ist mir unklar?**
---
 &nbsp;
- Die Methode zur Erprobung
- somit die Rollen/Unterschiede der verschiedenen Werte (Ampere, Ohm etc.)
 &nbsp;
 
 --- 
 &nbsp
 ---

