Integrated Project 2020

SAMENVATTING
voormalig “I was there” (app om een student in te loggen met handtekening)


2 DELEN

USER gedeelte
inbreng handtekening (enkel als de student in de lijst staat, opgesteld door de admin)
GEEN feedback van suspicion level; enkel handtekening zetten -> popup dat het is gelukt; de rest gebeurd achter de schermen


ADMIN gedeelte
- Mogelijkheid tot CRUD van studenten. lijst van student met relevante gegevens
	Enkel wanneer de student in de lijst staat, heeft deze de mogelijkheid om in te loggen met zijn handtekening
	Belangrijk dat de admin deze lijst makkelijk kan exporteren (via CSV of iets anders: XLXS/JSON?) 
- overzicht handtekeningen met naam, studentennr, datum en locatie (reverse address lookup)
- voorzien van zoek/filter mogelijkheden
- beschermd door pwd 
- Data wordt lokaal weggeschreven maar kan gesynchroniseerd worden in firebase via synchronisatie knop
- bonuspunten voor handtekening verificatie, liefst lokaal en onmiddellijk
	Dit gebeurd dan via een “suspicion level” (omdat het moeilijk te achterhalen is of een digitale handtekening EFFECTIEF niet door de juiste persoon is gezet)


Deadline 19/10:
- wireframes
- architectuur (nadenken over klassen Welke database om lokaal weg te schrijven)
- canvas technologie -> welke canvas wordt er gebruikt








POTENTIEEL RELEVANTE INFORMATIE:

Rahimi Halima
- dit is de link van hoe we die img kunnen vergelijken maar waar ik nog aantwijfel
https://www.c-sharpcorner.com/forums/how-to-match-two-image-signatures?fbclid=IwAR3ggT__GCHdrtJ1eHyn2OZ334v9HzLRpEwTEn6Z5Gg8-Mb3WmStrtm56iI

- de link van hoe je key points van 2 foto's kunt vergelijken en kijken of ze verschillend zijn
https://www.tutorialspoint.com/how-to-match-the-key-points-of-two-images-using-opencv-java-library?fbclid=IwAR2fkS-dW0VBkZ5rzCG4YrtIwvjOwowelTBOBPMH4oS4-iHXiqO_oYNQxs8

- dit is van android, kotlin waar ge die signatureSpi kunt gebruiken
https://developer.android.com/reference/kotlin/java/security/SignatureSpi

Volders Pieter

Klassen / Database structuur

Student:  id:Long - studentnr: String - name:String - list<Autograph>
Autograph: id:Long - image: BLOB - date: Date - suspicionLevel:Enm
suspicionLevel: notRelevant - low  - high


Inloggen van student / Admin:
mogelijkheid van integratie met LDAP authentication / Azure Active Directory




Adriaenssens Jonas






