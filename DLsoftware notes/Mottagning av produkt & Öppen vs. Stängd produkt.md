Fråga till chatGPT:

Okay, tack för hjälpen. en annan fråga. i DLsoftware, så finns något som heter 'mottagning av produkt'. När dom fått en faktura med produkter som ska betalas så antar jag att det är här där jag registrerar att dom har mottagits med hjälp av ett order nummer, stämmer det? sen undrar jag också vad som menas med 'öppen mottagning' och 'stängd mottagning'?

Yes, du tänker helt rätt 👍  
Det här är klassisk **inköp / lager-logik**, och DLsoftware följer i stort sett samma tänk som många affärssystem.

Jag tar det steg för steg och kopplar det till verkliga flödet, inte bara systemtermer.

---
## Vad betyder **”mottagning av produkt”** i DLsoftware?

**Ja** – det är exakt där du registrerar att varorna **fysiskt har kommit in**, normalt kopplat till ett **inköpsordernummer**.

Det typiska flödet är:

1. **Inköpsorder skapas**
    
    - Du beställer produkter från leverantör
        
    - Systemet genererar ett **ordernummer**
        
2. **Varorna levereras**
    
    - Kartonger/produkter kommer till lagret
        
    - (Fakturan kan komma före, samtidigt eller efter – det är separat)
        
3. **Mottagning av produkt**
    
    - Du går till _Mottagning av produkt_
        
    - Väljer rätt **inköpsorder**
        
    - Registrerar:
        
        - vad som faktiskt kom
            
        - antal
            
        - ev. serienummer / batch
            
    - **Lagret uppdateras**
        

Det är alltså **mottagningen** som gör att produkterna blir “i lager” i systemet – inte fakturan.

---
## Viktigt: faktura ≠ mottagning

En vanlig missuppfattning är att:

> “När fakturan registreras så finns varorna”

Men i de flesta affärssystem (inkl. DLsoftware):

- **Faktura = ekonomi**
    
- **Mottagning = lager**
    

De är kopplade – men inte samma sak.

---
## Vad är **öppen mottagning**?

En **öppen mottagning** betyder i praktiken:

- Mottagningen är **påbörjad men inte färdig**
    
- Inköpsordern är fortfarande **öppen**
    
- Du kan:
    
    - ändra antal
        
    - lägga till fler mottagna rader
        
    - göra fler delmottagningar senare
        

Vanliga scenarion:

- Du har beställt 10 st → bara 6 st kommer
    
- Resten kommer senare
    
- Du registrerar 6 st nu → mottagningen är **öppen**
    

Systemet förväntar sig fler leveranser kopplat till samma order.

--------
## Vad är **stängd mottagning**?

En **stängd mottagning** innebär:

- Mottagningen är **klar**
    
- Inköpsordern avslutas
    
- Systemet antar:
    
    - inget mer ska komma
        
    - lagersaldot är definitivt
        
- Du kan oftast **inte ändra** mottagningen utan korrigering
    

Vanliga scenarion:

- Alla beställda produkter har kommit
    
- Du vet att resterande inte kommer levereras
    
- Du vill “låsa” ordern
    
 En stängd mottagning är alltså ett slags _“klart, färdigt, bokfört”_ för lagret.

----
## Sammanfattning i tabellform

|Begrepp|Vad betyder det?|
|---|---|
|Mottagning av produkt|Registrering av att varor fysiskt kommit in|
|Inköpsorder|Beställningen till leverantören|
|Faktura|Ekonomisk händelse (betalning/moms)|
|Öppen mottagning|Delvis mottagen, fler leveranser kan komma|
|Stängd mottagning|Färdig mottagen, inget mer förväntas|

------
## Hur detta hänger ihop i praktiken

Ett “rent” arbetssätt brukar vara:

1. Skapa inköpsorder
    
2. Ta emot varor → **mottagning**
    
3. Stäng mottagning när klart
    
4. Registrera leverantörsfaktura
    
5. Matcha faktura mot order/mottagning    

Detta gör att:

- lagret stämmer
    
- fakturor kan kontrolleras mot faktiskt mottagna varor
    
- avvikelser (fel antal, restorder) syns tydligt

----
## Flödesschema: Inköp → Mottagning → Faktura

[ Start ]
    |
    v
[ Skapa inköpsorder ]
    |
    |  (ordernummer skapas)
    v
[ Leverantör skickar varor ]
    |
    v
[ Mottagning av produkt ]
    |
    |---> Är alla varor mottagna?
    |          |
    |          |-- NEJ --> [ Öppen mottagning ]
    |          |             |
    |          |             | (restorder / fler leveranser)
    |          |             v
    |          |        [ Ny mottagning senare ]
    |          |             |
    |          |-------------+
    |
    |-- JA --> [ Stäng mottagning ]
                    |
                    v
           [ Varor finns i lager ]
                    |
                    v
        [ Leverantörsfaktura anländer ]
                    |
                    v
      [ Registrera & matcha faktura ]
                    |
                    v
               [ Betalning ]
                    |
                    v
                 [ Slut ]

-----------
## Så kan du “läsa” schemat

- **Inköpsorder**  
    → Det administrativa startskottet (vad du förväntar dig få).
    
- **Mottagning av produkt**  
    → Bekräftar vad som faktiskt kom in fysiskt.
    
- **Öppen mottagning**  
    → Används vid del-leveranser eller osäkerhet.
    
- **Stäng mottagning**  
    → Markerar att inget mer ska komma på ordern.
    
- **Faktura**  
    → Hanteras separat, men bör stämma mot mottagningen.


----------
## DLsoftware-annoterat flöde

**Inköp → Mottagning → Lager → Faktura**

[ Start ]
    |
    v
[ Inköpsorder ]
( Inköp → Inköpsorder )
    |
    |  • Leverantör
    |  • Artiklar
    |  • Antal
    |  • Pris
    |  → Inköpsordernummer skapas
    v
[ Order skickas till leverantör ]
    |
    v
[ Mottagning av produkt ]
( Lager → Mottagning av produkt )
    |
    |  • Välj inköpsordernummer
    |  • Kontrollera levererade artiklar
    |  • Ange mottaget antal
    |
    |---> Är allt mottaget?
    |          |
    |          |-- NEJ --------------------------+
    |          |                                 |
    |          v                                 |
    |   [ Öppen mottagning ]                     |
    |   • Delmottagning                          |
    |   • Resterande antal kvar på ordern       |
    |                                           |
    |<------------------------------------------+
    |
    |-- JA --> [ Stäng mottagning ]
                    |
                    |  • Ordern markeras som klar
                    |  • Inget mer kan tas emot
                    v
           [ Lager uppdateras ]
           ( Artiklar → Lager )
                    |
                    v
[ Leverantörsfaktura ]
( Ekonomi → Leverantörsfakturor )
                    |
                    |  • Registrera faktura
                    |  • Koppla till inköpsorder
                    |  • Kontrollera:
                    |      – pris
                    |      – antal
                    |      – moms
                    v
              [ Bokföring ]
                    |
                    v
              [ Betalning ]

