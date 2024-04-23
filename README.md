![Oi, Equilíbrio!](https://github.com/morrismuehl/CapoeiraEquilibrioLiederbuch/blob/main/equilibrio.png?raw=true) 

# PDF vom Liederbuch

+ Auf main.pdf klicken →  Downloadbutton ist oben rechts
    + Lieder im Inhaltsverzeichnis sind in der .pdf verlinkt, also einfach auf ein Lied klicken!
+ Sollte das zukünftig nicht klappen kann ich die Datei auch auf Dropbox o.ä. hochladen
+ Wenn ihr wollt/könnt geht natürlich auch das repo clonen und die TeX Datei selbst kompilieren



<!-- Wer diesen Link hier entdeckt hat, hat eindeutig zu wenig zu tun! https://drive.google.com/file/d/12-0kGGJtOUCfqC{5}G2pe8LlUzrcaDV8oy/view?usp=sharing -->


# TO-DO 

+ [ ] Metaphorische Bedeutungen der Lieder in 1-2 kurzen Sätzen nennen.
- [ ] Römische Zahlen zu arabischen Zahlen
    - [ ] Evtl. sogar mit "richtiger" musikalischer Notation?
- [ ] Lieder automatisch in alphabetischer Reihenfolge auflisten
- [ ] Irgendwie Berimbaus in den Hintergrund/Rand/Mitte/überall
- [ ] **Mehr Lieder!**


# Wozu der ganze Scheiß hier?

+ Hier kann ich sehr easy Veränderungen sehen und ggf. unterschiedliche Versionen erstellen
+ Ihr könnt mir natürlich auch einfach privat schreiben wenn ihr das Liederbuch haben wollt oder Ideen habt! 


# Vorschläge/Ideen/Neue Lieder

## Einfach

+ Auf Issues gehen →  Lied oder Anmerkung reinschreiben →  weiteren Anweisungen folgen
+ Wenn das nicht geht kontaktiert mich ruhig auf anderen Wegen

## Komplizierter

+ in [main.tex ](https://github.com/morrismuehl/CapoeiraEquilibrioLiederbuch/blob/main/main.tex) reingucken, die Liederstruktur ist gar nicht so kompliziert  
+ Den Song zwischen ``\begin{song} und \end{song}``
    + Verse zwischen ``\begin{verse*} und \end{verse*}``
        + Ohne `*` werden die Strophen nummeriert
        + Gleiches geht prinzipiell auch mit ``\begin{chorus*} und \end{chorus*}``, braucht man aber meist nicht (finde ich)
    + Um Symbole über Teile von Wörtern zu setzen ``\chord*{Symbol}Wo rt`` so erscheint es über dem "Wo" (Das Leerzeichen ist wichtig!)
    + *kursiv* geht mit `\textit{kursive Sachen}`

### Beispiel für ein Lied

```
\begin{song}{title={Dificuldade no nó do atabaque eu vou fazer}}
        \begin{verse*}
            \chord*{{3}, {5}}Difi \chord*{{4}}cul dade no nó do atabaque eu vou fazer\\
            \chord*{{3}}Ba lança pra la\\
            \chord*{{3}}Ba lança pra ca\\
            \chord*{{3}}pra \ tu aprender\\
            \textit{Dificuldade no nó do atabaque eu vou fazer}\\
            \textit{Balança pra la}\\
            \textit{balança pra ca}\\
            \textit{pra tu aprender}\\
            \chord*{{3}}Tem \ dendê no atabaque\\
            \chord*{{3}}\textit{No} \textit{atabaque tem dendê}\\
            \chord*{{3}}a tabaque tem dendê\\
            \chord*{{3}}\textit{Tem} \ \textit{dendê no atabaque}\\
        \end{verse*}
\end{song}
```


