## Scheduling Algorithms for Multiprogramming in a Hard-Real-Time Enviroment 

### Abstrakt
Detta är en sammanfattning av artikeln "Scheduling Algorithms for Multiprogramming in a Hard-Real-Time Enviroment" som är skriven av C. L. Liu och James W. Layland 1973. Artikeln diskuterar problematiken med att schemalägga multikörningsprogram (engelska multitasking) på en dator med en ensam processor, framförallt där processer är beroende av att köras inom en viss tidsgräns. Artikeln visar på att en låst prioritesordning oftast leder till en så pass låg processoreffiktivetet som 70%. 

En alternativ metod där varje uppgift poänsätts via sin aktuella tidsdrist. Denna poäng används sedan för att sätta upp prioriteringsordningen som möjligör full processor effiktivitet. En kombination av dessa två metoder diskuteras även.  

### Keywords 

realtids multikörning av program, schemaläggare, multiprograms shemaläggare, dynamisk schemaläggare, tidsfrists baserad schemaläggare, prioritetsbaserad schemaläggning.

### Introduktion 

Datorer används i stor utsträckning till att övervaka och kontrollera industriprocesser. Dessa datorer har oftast program som är tids-kritiska processer så som kontroll och övervakning men även rena batch processor (processer som datorn utför helt självständigt utan inblandning av användare eller avbrott). Men det finns även system där dessa icke tids-kritiska processer saknas och alla uppgifter i arbetskön är beroende av att ske inom en viss tidsgräns. När det inte finns några jobb som kan ges en lägre prioritet så kan man endast nå en säker och effektiv hantering genom att schemalägga arbeten väldigt noga. Den senare gruppen, ren processtyrning, används som bakgrund till den kombinerade metod som kommer att presenteras.

Två algoritmer för schemaläggning för denna typ av processer studeras i artikeln. Båda dessa algoritmer bygger på prioritet och baseras på "preemtion" (det aktuella arbetet kan avbrytas för att köra ett annat arbete som har högre prioritet). 
I kombination med preemtion så använder sig den första metoden av en fixerad prioritets tilldelning, den kommer alltså inte att ändras innan den har körts. Denna metod leder till en effektiv användning av processorn till på ca 70%. Det andra alternativet gör det möjligt att till fullo använda processorn genom att använda sig av en flexibel tilldelning av prioritet, där prioriten kan omvärderas beroende på den aktuella tidsfristen.      

Ett datorsystem för att hantera ett processflöde utför en eller flera funktioner för att kontrollera och övervaka processen. Varje funktion baseras på en eller flera uppgifter.  En del av dessa uppgifter är baserade på avbrott eller svar från andra delar av systemet, resten baseras på information eller som svar på data som andra funktioner eller uppgifter lämnar. Ingen av dessa uppgifter kan utföras innan en funktion kräver detta. Dessa uppgofter måste ske inom en viss tidsram - en del är strikt beronde av att de uförs inom en exakt tidsrymd (dessa kategoriserar vi som "hard-real-time", dess motsatt "soft-real-time"). En bra metafor skulle kunna vara en hjärtsimulator, där det är viktigt att varje slag slår på exakt utsatt tid. Det hjälper inte att det i snitt sker på rätt tid. En pacemaker skulle alltså här visas arbeta i "hard-real-time". 

### Metod 
Författarnas antaganden görs genom beräkningar på ett par givna antaganden och krav. Exempelvis så ställer antar man att alla förfrågningar för uppgifter som har hårda deadlines är periodiska och har en konstant intevall mellan förfrågningarna. Vidrare så antas att varje uppgift måste slutföras innan nästa förfrågan kan hanteras. Uppgifterna som ligger i eller kommer in i kön är helt oberoende av andra uppgifters start eller slutförande. Exekvieringstiden för en uppgiftär konstant för den uppgiften och kommer inte att variera mellan olika körningar. Uppgifter som är icke-periodisk skiljer sig från andra uppgifter och hanterar initiering eller felhantering. De har högre prioritet än periodiska uppgifter när de körs men har inte hårda deadlines. 

### Resultat


### Diskussion 
