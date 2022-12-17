---
title: "Unterrichtsblog vom 15.12.2022"
date: 2022-12-17T14:24:18+01:00
type: post
author: Moritz
tags: ["Wiesenmüller", "CarRent"]
---

# Guten Mittag,

in diesem Blogbeitrag möchte ich mit euch die Aufgabe von Herrn Wiesenmüller mit euch teilen.

### Aufgabenstellung:
> „Erweitere dein Programm so, dass man ein Fahrzeug betanken kann.“

### Wie löse ich das?

In dieser Lösung, kann man noch nicht selbst bestimmen wie voll der Tank sein soll, sondern er wird immer voll getankt.

- Zuerst erstellen wir in unserer PKW-Klasse zwei Variablen vom Typ double, die das maximale Tankvolumen und das aktuelle Tankvolumen festlegen.
```java
class PKW {
	private double tankMax;
	private double tank;
}
```
- Danach erstellt ihr wie gewohnt Getter und Setter für die beiden Attribute. Außerdem ist es wichtig, dass ihr den Konstruktor der Klasse PKW aktualisiert!
- Es ist auch wichtig, dass ihr vor der Erstellung des PKWs in eurer Main-Methode mit dem Scanner abfragt, wie viel Liter der Tank maximal haben kann & wie viel er momentan hat.
```java
System.out.println("Maximales Tankvolumen: ");
int pkwMaxTankvolumen = Integer.parseInt(scanner.nextLine());

System.out.println("Aktuelles Tankvolumen: ");
int pkwTankvolumen = Integer.parseInt(scanner.nextLine());

PKW pkw = Pkw(String EureAttribute);
```
- Als nächstes fragt ihr ab, ob der Nutzer den PKW tanken will. Das funktioniert mit einem Boolean Scanner.

```java
System.out.println("Wollen Sie den PKW tanken?");
boolean input = Boolean.parseBoolean(scanner.nextLine());
```
- Als nächstes müsst ihr mithilfe einer if-Abfrage herausfinden, ob die Eingabe „true“ ist & dann das Attribut „tank“ auf den Wert vom Attribut „tankMax“ setzen.
```java
if (input == true) {
	pkw.setTank(pkw.getTankMax());
	System.out.println("Sie haben den PKW getankt.");
} else {
	//Anweisungen, was passiert wenn Eingabe „false“ ist
}
```
- Nun sollte dein Programm funktionieren & du kannst deinen PKW betanken.

### Aufgaben zum Knobeln
Falls du noch etwas üben möchtest, habe ich dir folgende Aufgaben herausgesucht:
- Implementiere diesen Code auch für den LKW.
- Implementiere eine Version des Programms, in der der Nutzer *selbst* entscheiden kann wie viel er tanken möchte.

Bei Fragen könnt ihr uns einfach anschreiben!

### Schlusswort

Ich hoffe euch hat dieser erste Blogbeitrag gefallen, falls ihr Wünsche oder Anregungen habt erzählt sie uns.

Beste Grüße,

Moritz