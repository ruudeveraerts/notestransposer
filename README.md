README.md by Ruud Everaerts, about his Notestransposer

Written 21 Sept 2012

Hello everybody who is reading this. I am writing this
because I'm trying to figure out how git and github.com
are working. Some time ago I wrote some code in JavaScript
to transpose musical notes, and published it on my website.

Looking for some code to publish on my github-account, I found
this code, and decided to provide it. I needed some selfwritten
JavaScript code anyway, to get to know github better, and I think 
this, maybe trivial piece of code, needed to be available as open 
source code anyway.

In this README.htm I provide the dutch Handleiding (=tutorial)
(see bottom of the page) that can also be found in the
original html-document that contains the JavaScript code (see
folder Document, file transposer.htm).

But first: here's the tranlation of this Handleiding in English.

Tutorial

Some time ago I was working with Lilypond, this
great program for writing musical notes (also
providing output in MIDI-format). But mostly
known for transforming notes in ascii-style
into pretty PDF sheets of music. A great tool
for writing professional sheet music, or, learning
to read notes / sightreading/ prima vista reading.
Lilypond is a tool that plays the music you
entered in ascii-style, or more correctly, creates
the MIDI-file you can play to hear what you have
written. A great way to teach yourself.

I learned that this program has to possibility
to transpose notes. 
A song in C can be played in E, just tell Lilypond
to do so. But I found out, sometimes, according to
your needs, Lilypond is doing too much. What if you
want to see how the notes in Ascii-format change
to other notes in Ascii-format, when you tell a program
to transpose the given notes?

Up till now, I haven't found a way how to accomplish
this in Lilypond. But since we are talking a about
ascii plain text here, I thought I might be possible
to write something in JavaScript that can do this
for you.

===
How to use the HTML-page with JavaScript?

It's easy. Select the melody-part from your
Lilypond file. And copy it to the
text area on the left of the page.
Just put the notes. c4 d8 g,4 a'2 are
examples of notes in ascii-lilypond-style.
Make sure every note has a space before it.
If the note is at the first position of a line,
make sure you put a space in front of it.

On the left, you'll see an option-box. Labeled
"Bron" (Dutch for "Source"). Select the
note the song is in. (Select a Major Key.
Musicians know, when the song is in Minor, what
the Mayor equivalent is: Am -> C , Bm -> D 
Dm -> F, C#m -> F and so on)

On the right, you'll see an option-box. Labeled
"Doel" (Dutch for "Target"). Select the note
you want the song to be in. Again, select the
Mayor equivalent, if the song is in Minor.

Then, click the button between the left and
the right text area. A transposed version
of the notes will appear in the right text
area box.

===<hr>


Handleiding

Laatst was ik bezig met Lilypond, het geweldige 
notenschrijfprogramma (compleet met midi-output) 
dat noten die je ingeeft prachtig op papier zet. 
Ideaal voor het professioneel vervaardigen van 
bladmuziek, of, waar ik het voor gebruikte, om 
noten te leren lezen. Leuk als je door de 
midi-output meteen kan terughoren hoe je zelf had 
moet bedenken hoe het zou moeten klinken.

Ik ontdekte dat het programma je ook helpt bij 
het transponeren van muziek. Staat het stuk in c, 
maar wil je het in e zingen, dan kan dat. Bij 
Lilypond is het zelfs zo gemakkelijk gemaakt, dat 
je dan alleen maar ervóór hoeft aan te geven in 
welke hoogte je het uitgeprint wil hebben!



Ideaal. Het past ook wel bij mijn filosofie dat 
de kern van muziek eigenlijk een geraamte is, dat 
door arrangeurs en instrumentalisten verder 
ingekleurd wordt.

Maar hier ging Lilypond me eigenlijk te snel. 
Stel dat ik de notenpartij zelf wil transponeren 
naar een bepaalde hoogte. Dus niet de output in 
midi of in pdf, maar de onderliggende partij. Het 
lijkt me eigenlijk wel ideaal om alle muziek in c 
te hebben, en dan zelf per geval te exporteren 
naar de hoogte die op dat moment nodig is. Ook 
leuk voor vergelijkend muziekonderzoek, bedenk ik 
me nu...

Het kan bijna niet anders of Lilypond heeft daar 
ergens een module voor, maar ik vond hem niet. Ik 
besloot zelf wat in JavaScript in elkaar te 
zetten.

Een muziekkenner zal er wel van gruwen. Snap nog 
steeds niet de zin van een beses = enharmonisch 
gelijk aan een a, of het verschil tussen een fis 
en een ges. Wat enharmonisch gelijk is, is in 
mijn systeem gewoon helemaal gelijk. En ik 
vertaal naar de namen die ik het meeste tegenkom. 
Dus liever een bes dan een ais, liever een cis 
dan een des, liever een es dan een dis, bij gis 
en as kies ik voor as, al weet ik niet waarom.

Hoe gebruik je deze pagina?
De handleiding is eenvoudig: selecteer het 
melodiestukje uit de lilypond-file (bijvoorbeeld 
voorbeeld.ly). Alleen de nootjes, niet het 
relative of key gedoe vooraf. Kopieer dat in het 
vakje hierboven. (Bij het starten staat daar het 
notenfragment van het volksliedje "Berend Botje", 
als voorbeeld. Vervang die tekst dus). O, en hou 
in de gaten: een noot wordt voorafgegaan door een 
spatie. Dus begin iedere regel met een spatie.

Geef linksboven (bij Bron) aan in welke hoogte 
dit bronbestand staat. (Berend Botje staat in f). 
Geef daarnaast (bij Doel) aan naar welke hoogte 
het liedje getransponeerd moet worden.

Dan klikken op de toets met het pijltje, en 
voila. Wellicht dat het scriptje iemand tot nut 
zal zijn.

UPDATE
Nou, nog niet helemaal perfect, maar toch een 
verbetering: als de doelhoogte g d a e b of fis 
is, worden zwarte toetsen genoteerd met een 
kruis, als de doelhoogte f, bes, es, as, des of 
ges is, worden zwarte toetsen genoteerd met een 
mol.
