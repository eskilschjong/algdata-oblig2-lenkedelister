# Obligatorisk oppgave 2 i Algoritmer og Datastrukturer

Denne oppgaven er en innlevering i Algoritmer og Datastrukturer. 
Oppgaven er levert av følgende studenter:
* Eskil Ekaas Schjong, s364722, s364722@oslomet.no
* Oliver Dragland, s364702, s364702@oslomet.no

# Arbeidsfordeling

I oppgaven har vi hatt følgende arbeidsfordeling:
* Vi har i fellesskap løst alle oppgavene.

# Oppgavebeskrivelse

I oppgave 1 så lagde vi først metoden antall for å sjekke antall verdier i listen,
og metoden tom for som returnerer en boolean basert på om listen er tom eller ikke.
Vi lagde en konstuktør som lager en dobbeltlenket liste fra en tabell.

I oppgave 2 så lagde vi en toString metode som returnerer en tegnstreng med den dobbeltlenkede listens verdier.
Vi lagde også en metode som gjør det samme i omvendt rekkefølge.
Vi lagde også metoden leggInn, som legger in en node med en ny verdi bakerst i listen.

I oppgave 3 lagde vi en metode som skal returnere noden med en gitt indeks.
Vi lagde også en metode som kan endre verdien til en node med gitt indeks.
Vi lagde også en metode som returnerer en ny liste fra intervallet mellom to gitte indekser.

I oppgave 4 traversjerer vi gjennom listen i forsøk om å finne matchende verdi. 
Derfra lagrer vi indexen til matchende verdi og returner første tilfelle.
Hvis den ikke fant en matchende verdi, blir ikke index oppdatert fra -1 og vil dermed returnere -1 (fant ikke verdien i liste.)
I metoden inneholder bruker vi indeksTil for å sjekke om verdien finnes i listen.
Dersom indeksTil returnerer -1, finnes ikke verdien.

I oppgave 5 skiller vi mellom om den skal legge inn fremst, bakerst eller et annet sted. Her blir ny node opprettet,
og pekere blir endret slik at nodene ved siden av indeksen vil peke på den nye noden. 
Dermed vil alle noder sin indeks bak den nye noden bli forhøyet med en.

I oppgave 6 måtte vi som i oppgave 5 skille mellom om vi skal fjerne fremste, bakerste eller en annen node.
Dersom noden enten er bakerst, eller fremst endrer vi bare hale/hode pekerne. 
Dersom noden ligger et annet sted, bruker vi metoden finnNode for å finne noden til indeksen, og bytter om nodenaboenes pekere.
I fjern(verdi) bruker vi samme fremgangsmåte som over, bare at vi finner ut om noden er fremst eller bakerst på en litt annen måte.
Dersom noden ligger et annet sted, traverserer vi gjennom listen og matcher verdien til nodene med inputverdi.
Derfra finner vi riktig node, og bytter om naboens pekere.

I oppgave 7 så valgte vi å benytte oss av metode 1 ettersom dette er av en laverer kompleksitet.
Her traversjerer vi gjennom listen og setter hver node til null,
og avslutter med å sette hode = null og antall = 0.

I oppgave 8 sjekker vi om tabellen er tom ved hjelp av metoden hasNext(), dersom hasNext=false, er tabellen tom.
B fulgte vi oppgaveinstruksen. Da vi lagde konstruktøren til iterator interfacet, kopierte vi den ferdigskrevde metoden,
og bytte ut startnoden (denne) fra hode til noden som tilhører input indeksen via metoden finnNode(indeks).
I D brukte vi først indekskontroll på indeks, også returnerte vi en instans av DobbeltLenketListeIterator(indeks).
