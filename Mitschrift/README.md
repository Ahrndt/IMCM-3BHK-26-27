# IMCM-3BHK

## Einleitung

### Markdown

*Markdown* ist eine Auszeichnungssprache (_Markup Language_)
Mit Auszeichnungssprachen wird text strukturiert. Einige Markup- Languages sind z.B.:

- HTML (*Hypertext Markup Language*)
- XML    (*Extensible Markup Language*)
- MD (*Markdown*)
- YAML(*YAML Ain´t Markup Language* bzw *yet another markup language*)

Markdown ist heutzutage eine der beliebtesten Auszeichnungssprachen. 
Es wird vor allem für die Erstellung von Dokumentationen, Blogs und Readme-Dateien verwendet, da es einfach zu lernen und zu verwenden ist. 

Um ein Git-Repository zu erstellen und Markdown-Dateien zu verwenden, können Sie die folgenden Schritte ausführen:

- im gewünschten Verzeichnis im Terminal(bzw CLI-_Command Line Interface_) den Befehl `git init` ausführen, um ein neues Git-Repository zu erstellen.

>**Einschub zur Installation von Git**

>Falls bei der Eingabe von `git init` eine Fehlermeldung erscheint, ist Git möglicherweise nicht installiert. In diesem Fall können Sie Git von der offiziellen Website [git-scm.com](https://git-scm.com/) herunterladen und installieren. 
Bei der Installation wird der Befehl in den Umgebungsvariable **PATH** hinzugefügt. Darin sind die Bezeichnungen aller Programme ethalten, die im Terminal aufgerufen werden können.

- dann in Github-Desktop das erstellte Repository öffnen und mit dem lokalen Repository synchronisieren.(File > Add Local Repository)

-nun kann über die schaltfläche **Commit to master** ein Commit erstellt werden.
- danach kann das Commit auf das entfernte Repository (z.B. auf GitHub) gepusht werden, indem die Schaltfläche **Push origin** verwendet wird.






## Statische und dynamische Websites


Wenn wir eine Anfrage stellen, stellt unser Computer die Anfrage an den DNS Server. 

DNS-Request wird an den DNS-Server gesendet, der die Anfrage verarbeitet und die entsprechende IP-Adresse zurückliefert(DNS-Response).

 HTTP-Request wird an den Webserver gesendet, der die Anfrage verarbeitet und die entsprechende Antwort zurückliefert(HTTP-Response).

In den 1990er Jahren waren die meisten Websites statisch. Das bedeutet, dass der in Inhalt in eine html-Datei geschrieben wurde und sich nicht dynamisch änderte. Jede Anfrage an den Webserver lieferte die gleiche HTML-Datei zurück. Die Inhalte waren also immer gleich, die abgefragt worden sind.

![funktionsweise von statischen Websites](image.png)
*Abbildung: Ablauf einer DNS- und HTTP-Anfrage*
^
Die Abbildung zeigt die Funktionsweise von statischen Websites. Zuerst muss der Domain-Name über das Domain Name System (DNS) in die IP-Adresse des Webservers aufgelöst werden (Schritt 1 und 2 in der Abbildung). Danach schickt der Client eine http-Anfrage an den entsprechenden Webserver und erhält von diesem eine http-Antwort, die überlicherweise zuerst die index.htmlenthält (Schritt 3 und 4).

Ab den 2000er Jahren setzten sich zunehmend dynamische Websites durch. Im Gegensatz zu statischen Websites werden die Inhalte hier nicht fest in HTML-Dateien gespeichert, sondern bei jeder Anfrage dynamisch vom Webserver generiert. Dies ermöglicht personalisierte Inhalte und interaktive Funktionen.

![alt text](image-1.png)

Der Ablauf der Seitenerstellung ist in der folgenden Grafik dargestellt. Die URL-Auflösung mittels DNS erfolgt wie bei statischen Websites(in der Grafik lila dargestellt). Der Webserver braucht bei dynamischen Websites aber unterstützung durch eine serverseitige Programmiersprache.(PHP, Python, Ruby, etc.) Wenn der Webbrowser bzw. Webclient bei einem Restaurantbesuch als Gast gesehen wird, dann ist der Webserver der Kellner, der die Bestellung aufnimmt und sie an den Koch weitergibt. Die Köchin ist dann in diesem Fall die serverseitige Programmiersprache. Sie greift daraufhin auf die Zutaten in der Vorratskammer (Datenbank) und bereitet das Gericht nach einem Rezept (HTML-Template bzw. Vorlage) zu. Das fertige Gericht (HTML-File) wird dann vom Kellner (Webserver) an den Gast (Webbrowser) serviert.

