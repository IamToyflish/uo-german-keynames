How to: Ultima Online Makros auf das Numpad legen
===

!!! ACHTUNG: DIESE ANLEITUNG FUNKTIONIERT NUR MIT DEM DEV CLIENT !!!

Der Standardclient patcht bei jedem Start über den Launcher, ersetzt also bei jedem Start die keynames.txt. Der Dev-Client tut das nicht. Die keynames.txt wird also JEDES MAL ersetzt, wenn ihr den Standard-Patch-Branch benutzt. Da komm ich später noch mal drauf :)

BUT WHY!?
---

Ich mag die F-Tasten nicht, die sind so weit auseinander und ich muss meine Hand so viel bewegen, das ist ja ekelhaft. Wir sind hier ja nicht beim Sport! 

BUT HOW!?
---

Schritt 1: Numlock deaktivieren
Wenn ihr das nicht tut werdet ihr als Makro-Taste einfach die "1" bekommen, also auch über die Ziffernreihe abrufbar. Man deaktiviert Num durch den Druck auf die Num-Taste.

Schritt 2: Testmakro anlegen

Legt euch ein Makro mit irgendwas ein. Bei mir war es:
1 (ZEHNERTASTATUR)
Say Lucian beschte

Ihr werdet dieses Makro nie drücken müssen, von daher ist es zum testen egal was für eines es ist.

Wichtig ist dass im Tastaturkürzel-Feld nicht nur die "1" steht, sondern "1 (ZEH). An den Klammern dahinter erkennt man, dass er tatsächlich die Numpad-Taste nimmt und nicht die Taste "1".

Schritt 3: Makrofile überprüfen 

!!! Wer das Phänomen Nummerntasten in UO Makros NICHT nachvollziehen, sondern es einfach nur lösen will kann diesen Schritt überspringen !!!!

Das Makrofile findet man auf Windows unter:
%USERPROFIL%\Dokumente\Alathair\Einstellungen\Profile\{Accountname}\Alathair\{Charname}\macros2d.txt

Solltet ihr das Makro oben angelegt haben (und sonst keines), wird die Datei folgenden Inhalt enthalten:

    1 (ZEHNERTASTATUR) 0 0 0
    +S a y   * h u s t e t * 
    ########
    
Hier können wir in der ersten Zeile herausnehmen wie die Taste vom Client benannt wird.


Schritt 4: Tastennamen in keynames.txt übernehmen

Die keynames.txt ist dafür zuständig, dass UO weiß wie die Tasten auf eurer Tastatur heißen. Nur wenn die Namen in der keynames.txt mit den Namen in der macros2d.txt überein stimmen erkennt UO die korrekten Makros.

Wenn das nicht der Fall ist "bereinigt" UO die falschen Makros sobald ihr euren Client schließt, wirft also alles weg bei dem die Tasten nicht übereinstimmen.

Die keynames.txt findet ihr unter:
{Alathair Ordner}\keynames.txt

Ein wenig nach unten gescrollt sehen wir folgende Einträge (hier auszugsweise dargestellt):

    ...
    Num 1
    Num 2
    Num 3
    Num 0
    ...

... und der geneigte Leser von Schritt 3 wird merken: Das stimmt nicht überein!

Damit ihr euch nicht die Mühe machen müsst jedes Makro auszuprobieren um den Namen dann in die keynames.txt zu übertragen, habe ich hier den Num-Abschnitt meiner keynames.txt zusammengefasst:

    Scroll Lock
    7 (ZEHNERTASTATUR)
    8 (ZEHNERTASTATUR)
    9 (ZEHNERTASTATUR)
    - (ZEHNERTASTATUR)
    4 (ZEHNERTASTATUR)
    5 (ZEHNERTASTATUR)
    6 (ZEHNERTASTATUR)
    + (ZEHNERTASTATUR)
    1 (ZEHNERTASTATUR)
    2 (ZEHNERTASTATUR)
    3 (ZEHNERTASTATUR)

Den Block könnt ihr einfach kopieren und den Teil eurer Datei ersetzen, wenn ihr wollt. Für "/" und "*" gibt es leider keinen Ersatz. Da wird in die Makro Datei immer nur " (Zehnertastatur)" für beide Tasten geschrieben. Wer da was rausfindet.. immer her :)

Das Ersetzen der keynames.txt müsst ihr bis jetzt leider nach JEDEM Patchen über den Standard-Zweig des Launchers wiederholen.

Schritt 4: Profit!
Nachdem ihr eure keynames.txt angepasst habt könnt ihr nun 
