Soft Computing - Platforma za izradu kolokvijuma

1.  Platforma

Za izradu zadataka koristiti Python 3.14. Sama platforma “trči” na Python 3.14.10.

Studentima je dostupan kompletan skup podataka. Na pomenutom skupu podataka će se i
evaluirati rešenja.

Prilikom submit-a Python skripte sa rešenjem, platforma izvršava skriptu pomoću sledeće
komande:

python <ime_skripte>.py  <dataset_folder>
Npr.: python moja_skripta.py data/

Lokaciji skupa podataka se može pristupiti pomoću argumenata komandne linije (sys.argv).

Neophodno je da skripta kao rezultat izvršavanja na kraju ispiše samo broj koji predstavlja
rezultat, bez ikakvog pratećeg teksta:

●  Nepravilno: Dobijena vrednost je 10.23
●  Pravilno: 10.23

Takođe, potrebno je zakomentarisati sva iscrtavanja (plot-ove) i suvišne ispise (print-ove)
kako bi se skripta uspešno izvršila na platformi.

Svaki student može najviše tri puta submit-ovati svoje rešenje za svaki kolokvijum
bez gubljenja bodova. Svakim dodatnim submit-om se gubi po 1 bod.

Platforma će asistentima uvek prikazati studentsko rešenje sa najboljim rezultatom.
Ako studenti žele da im se gleda neki drugi submit, potrebno je da isto napišu svom
predmetnom asistentu putem email-a.

Skripte se na platformi izvršavaju asinhrono, a vreme izvršavanja će biti posebno
definisano za svaki kolokvijum. Ako se taj period prekorači, pokušaj će se računati kao
neuspešan. Platforma “trči” na serveru koji ima Intel Xeon procesor (4 x 2.4 GHz), 16 GB
RAM memorije i Debian operativni sistem.

Nakon što se skripta izvrši, ukoliko je sve prošlo bez problema, u desnom delu prozora (My
Submissions) će biti prikazan ostvareni rezultat sa zelenom bojom kao pozadinom. Ukoliko
nema rezultata, već samo crvena boja kao pozadina - pogledajte sekciju 3.

U meniju Rate Me! studenti mogu prijaviti greške i dati predloge za unapređenje platforme.

2.  Biblioteke

Na platformi su instalirane biblioteke koje su ostavljene u okruzenja folderu na GitHub
repozitorijumu predmeta.

Prilikom submit-a rešenja na platformu, studenti mogu da koriste sve core pakete
Python-a 3.14 i gorenavedene biblioteke. Prilikom analize problema, analize skupa
podataka, vizualizacije podataka studenti mogu da koriste biblioteke po izboru, ali je
neophodno da njihovi import-i i upotreba u submit skripti budu zakomentarisani, kako bi se
ona bez problema izvršila na platformi.

3.  Najčešće greške

Ukoliko nakon submit-a skripte u desnom delu prozora ne dobijete rešenje, već samo crvenu
boju pozadine, na stranici submit-a možete videti poruku greške (Error message). Značenja
nekih poruka greške:

Invalid output format - poslednji red ispisa nije broj koji predstavlja rezultat
●
●  Execution time exceeded the limit - skripta se izvršavala duže od definisanog

vremena izvršavanja za kolokvijum

●  No output - skripta se nije uspešno izvršila. Uzrok može biti sintaksna greška,

korišćenje biblioteke koja nije instalirana na platformi, plot koji nije zakomentarisan…

Pored gorenavedenih, moguća je i poruka koja predstavlja exception koji je skripta “bacila”.

Da bi se sprečile greške, a samim tim izgubili i dragoceni pokušaji za kolokvijum,
preporučuje se da pre submit-a proverite sledeće stvari:
●  Da li koristite odgovarajuću verziju Python-a;
●  Da li se skripta može izvršiti putem komande:

python <ime_skripte>.py  <dataset_folder>
npr.: python python moja_skripta.py data/

●  Da li se kao rezultat izvršavanja vraća samo broj koji predstavlja rešenje, bez

pratećeg teksta i suvišnih iscrtavanja i ispisa;

●  Da li su zakomentarisani import-i i upotreba biblioteka koje nisu instalirane na

platformi za taj zadatak;

●  Da li izvršavanje skripte na vašoj mašini traje kraće od vremenskog roka za

kolokvijum.

Ukoliko i pored svega navedenog ne uspete da utvrdite problem, pošaljite asistentu
email.


