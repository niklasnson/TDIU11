## Scheduling Algorithms for Multiprogramming in a Hard-Real-Time Enviroment 

### Abstrakt
Detta är en sammanfattning av artikeln "Scheduling Algorithms for Multiprogramming in a Hard-Real-Time Enviroment" som 
är skriven av C. L. Liu och James W. Layland 1973. Artikeln diskuterar problematiken med att schemalägga 
multikörningsprogram (engelska multitasking) på en dator med en ensam processor, framförallt där processer är beroende 
av en garanterad körning. Artikeln visar att låst prioritesordning oftast leder till en så pass låg 
processoreffiktivetet som 70%. En alternativ metod baserad på aktuell tidsfrist visas som möjligör full processor 
effiktivitet. En kombination av dessa två metoder diskuteras även. 

### Keywords 

realtids multikörning av program, schemaläggare, multiprograms shemaläggare, dynamisk schemaläggare, tidsfrists baserad
schemaläggare, prioritetsbaserad schemaläggning.


### Introduktion 

Datorer används i stor utsträckning till att övervaka och kontrollera industriprocesser. Dessa datorer har oftast 
program som är tids-kritiska processer så som kontroll och övervakning men även rena batch processor (processer som 
datorn utför helt självständigt utan inblandning av användare eller avbrott). Men det finns även system där 
icke tids-kritiska processer existerar där alltså alla processer är tids-kritiska då krävs noga schemaläggning av 
aktiviteterna för att systemet skall kunna arbeta effektivt och säkert. Den senare av dessa exmpel är den som används 
för att lägga fram den kombinerade metoden. 

Två algoritmer för schemaläggning för denna typ av processer studeras i artikeln. Båda dessa algoritmer bygger på 
prioritet och baseras på "preemtion" (det aktuella arbetet kan avbrytas för att köra ett annat högre prioriterat 
arbete). Den första metoden använder sig av fixerad tilldelning av prioritet, den andra använder sig av en flexibel 
tilldelning av prioritet. Genom att kombinera de båda algoritmerna så kan man {} vilket även kommer att diskuteras. 

Ett datorsystem för att hantera ett processflöde utför en eller flera funktioner för att kontrollera och övervaka
processen. Varje funktion baseras på en eller flera uppgifter.  En del av dessa uppgifter är baserade på avbrott eller 
svar från andra delar av systemet, resten baseras på information eller som svar på data som andra funktioner eller 
uppgifter lämnar. Ingen av dessa uppgifter kan utföras innan en funktion kräver detta. Dessa uppgofter måste ske inom 
en viss tidsram - en del är strikt beronde av att de uförs inom en exakt tidsrymd (dessa kategoriserar vi som 
"hard-real-time", dess motsatt "soft-real-time"). En bra metafor skulle kunna vara en hjärtsimulator, där det är viktigt 
att varje slag slår på exakt utsatt tid. Det hjälper inte att det i snitt sker på rätt tid. En pacemaker skulle alltså 
här visas arbeta i "hard-real-time". 


### Metod 

* (A1) 
    Alla förfrågningar för uppgifter som har hårda deadlines är periodiska, med en konstant intervall mellan förfrågningar.

* (A2) 
    Varje uppgift måste slutföras innan nästa förfrågan kan hanteras.  

* (A3)
    Uppgiften är oberoende av start eller slutförande av förfrågningar av andra uppgifter. 

* (A4) 
    Exekveringstid för varje uppgift är konstant för den uppgiften och kommer inte variera mellan olika körningar. 

* (A5)
    Icke-periodiska uppgifter är speciella dessa hanterar initiering eller felhantering. De flyttar periodiska uppgifter 
    när de körs och har inte hårda deadlines.  
    

### Resultat


### Diskussion 
