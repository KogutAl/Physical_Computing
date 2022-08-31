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
 
  ![Bild zeigt einen Resistor](https://protosupplies.com/wp-content/uploads/2017/11/Resistor-10-Ohm-5-Closeup-CC.jpg)

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
- Die Methode zur Erprobung
- somit die Rollen/Unterschiede der verschiedenen Werte (Ampere, Ohm etc.)
 &nbsp;
 
 --- 
 ---

# Mystery Component
#### (*Auflösung: Potentiometer*)
 &nbsp;
![Bild zeigt ein Potentiometer](https://upload.wikimedia.org/wikipedia/commons/thumb/b/b5/Potentiometer.jpg/220px-Potentiometer.jpg)
 &nbsp;
---
### **Was ist ein Potentiometer?**
---
- Ein Widerstand ist ein grundlegendes elektrisches Element mit zwei Anschlüssen, das dem elektrischen Stromfluss widersteht, wenn eine Spannung zwischen den beiden Anschlüssen angelegt wird. Durch Hinzufügen eines beweglichen dritten Anschlusses wird der Widerstand in ein Potentiometer umgewandelt. Daher kann ein Potentiometer als ein Widerstand mit drei Anschlüssen mit einem variablen oder beweglichen Kontakt definiert werden, der eine Spannung in zwei Teile teilt.
 &nbsp;
---
### **Der Aufbau**
---

Unterschieden werden kann zwischen linearen und rotierenden Potentiometer. Beide bestehen sowohl aus vier Hauptkomponenten:

-  zwei festen Klemmen
-  einer beweglichen Klemme (Wischer genannt)
-  einem Widerstandsstreifen oder einer Widerstandsspur
-  Gehäuse

Der einzige Unterschied zwischen den beiden Arten von Potentiometern besteht darin, dass bei einem linearen Potentiometer der Widerstandsstreifen auf einer geraden Spur angeordnet ist, während bei einem Drehpotentiometer der Widerstandsstreifen auf einer Kreisbahn angeordnet ist.

 &nbsp;
 
 ---
### **Handhabung mit einem Arduinoboard**
---
Ein Potentiometer ist ein einfacher Regler, der einen variablen Widerstand liefert, den wir als Analogwert in das Arduino-Board einlesen können.

- kann als Analogwert in Arduino-Board eingelesen werden
- dieser Wert steuert hier die Rate bzw. Geschwindigkeit mit der eine LED blinkt

Um dies zu erreichen werden drei Drähte mit dem Board verbunden

- Der erste Draht geht von einem der äußeren Stifte des Potentiometers auf Masse (GND)
- Der zweite geht von 5 Volt zum anderen äußeren Stift des Potentiometers
- Der dritte Draht geht vom analogen Eingang 2 zum mittleren Pin des Potentiometers
 &nbsp;
![Anschluss des Potentiometers an Arduino-Board](https://www.exp-tech.de/media/image/39/a4/5b/xpotentiometer5c4f09d4098a5.jpg.pagespeed.ic.45UiUsDwnW.webp)
 &nbsp;
- Durch Drehen der Welle des Potentiometers wird der Widerstandswert auf beiden Seiten des Wischers geändert
- Dadurch wird die relative "Nähe" dieses Pins auf 5 Volt und Masse geändert
- nun haben wir einen analogen Eingang
- Wenn die Welle ganz in eine Richtung gedreht wird, gehen 0 Volt zum Stift
- wir lesen 0
- Wenn die Welle ganz in die andere Richtung gedreht wird, gehen 5 Volt zum Stift
- wir lesen 1023
- Dazwischen gibt analogRead () eine Zahl zwischen 0 und 1023 zurück, die proportional zu der an den Pin angelegten Spannung ist.

![Schaltplan](https://www.roboter-bausatz.de/media/image/b1/7b/12/Potentiometer_Steckplatine.jpg)

 &nbsp;
[Verlinkung zum Arduino Code](https://www.roboter-bausatz.de/projekte/arduino-potentiometer-beispiel-mit-led)

 &nbsp;
---

#### Quellen:

- <https://www.exp-tech.de/blog/arduino-tutorial-potentiometer>
- <https://funduino.de/nr-7-potentiometer>
- <https://www.roboter-bausatz.de/projekte/arduino-potentiometer-beispiel-mit-led>
