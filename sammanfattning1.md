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
prioritet och baseras på **preemtion** (det aktuella arbetet kan avbrytas för att köra ett annat högre prioriterat 
arbete). Den första metoden använder sig av fixerad tilldelning av prioritet, den andra använder sig av en flexibel 
tilldelning av prioritet. Genom att kombinera de båda algoritmerna så kan man {} vilket även kommer att diskuteras. 


### Metod 


### Resultat


### Diskussion 
