Victor Furustubbe
Klass: FED24
Företag: Initiam
Handledare: Lennart Svanberg
LIA-period: 8/1 — 22/5 2026

---
### Innehållsförteckning

1. Introduktion
2. Bakgrund
3. Genomförande & Resultat
4. Kopplingen till Kursplanen
5. Reflektion gällande förbättringsområden
6. Slutsats

---
### Introduktion

Denna rapport kommer att handla om det arbete jag i samverkan med mina klasskamrater Andrew Kalumba och Priyadharshini Seetha Ram har utfört under ledning av våran mentor och handledare Lennart Svanberg. Vi har under dessa 20 veckor jobbat med att utveckla ett nytt affärssystem vid namn BikeMeNow åt våran klient AVA MC AB i syfte att ersätta deras nuvarande system. Det har varit händelserika veckor fyllda av allt från intervjuer och tester till kodande.

### Bakgrund

AVA är en återförsäljare av motorcyklar beläget ute i Gustavsberg. Dom etablerades år 1975 och har lång erfarenhet av att ta hand om och förbättra motorcyklar. Verksamheten drivs av Gunnar som tillsammans med Toni sköter försäljning och kundkontakt.  

Deras Serviceavdelning sköter Service och underhåll vilket innebär allt från inköp av reservdelar, oljebyten och fullständiga genomgångar samt utförande av service, garanti och försäkringsärenden.

Mekanikerna reparerar, småjusterar och erbjuder däckservice till den som behöver det.

Till sist har vi Monica som är den administrativa spindeln i nätet. Hon har överblick över hela verksamheten och sköter allt från inköp och lagerhållning till fakturor och bokföring.

### Genomförande & Resultat

Vi inledde vår LIA med ett första möte ute hos AVA torsdagen den 8:e januari. Där bekantade vi oss med kunden och deras verksamhet. Gunnar visade oss deras affärssystem vid namn 'DLSoftware' och berättade om den upplevda problematiken av att använda det systemet.

Efter det mötet så ägnade vi ungefär en och en halv månad åt att intervjua personalen på AVA för en närmare inblick i deras arbetssätt, hur dom arbetar med det befintliga systemet, dokumentation över hur verksamheten fungerar och hur dom olika avdelningarna skiljer sig åt.

![[Pasted image 20260519202540.png]]

Vi bestämde oss tidigt för att fokusera på Säljavdelningen och resan från det första mötet med kunden till att motorcykeln blivit såld. Det resulterade i en 'Customer journey map' där:
1. Kunden visar intresse av att köpa en motorcykel genom att komma in till affären eller att gå in på deras hemsida (eller blocket som deras hemsida även är kopplad till).
2. Om ett fortsatt intresse finns så skapas en 'Offert' med all kundinformation samt kostnaden för motorcykeln och övrigt utrustning.
3. När en 'Offert' är accepterad så skapas ett 'Köpesavtal'. I ett köpesavtal ingår allt från namn & motorcykel till kostnader, försäkringar och betalningar samt finansiering genom eventuella lån.
4. Nu när båda parter har skrivit på köpesavtalet och motorcykeln är redo att antingen levereras om den finns i lager eller att beställas om så inte är fallet.

Det ovanstående är en kortfattad beskrivning över hur en försäljningsprocess går till eftersom det i verkligheten är väldigt komplicerat och innefattar delar av dom andra avdelningarna också. Därför valde vi att dela upp försäljningsprocessen mellan oss där jag (Victor) tog allt från kundkontakten till offert medans Andrew tog delen gällande köpesavtal och försäljning. Priya fokuserade på allt inom lagerhållningen.

Detta resulterade i en 'Pipeline' där dom säljansvariga kunde se kundens resa från anmält intresse till avslutad affär.

![[Pasted image 20260519225847.png]]

I början av april så fick jag ett sidouppdrag av Lennart där han ville att jag skulle bygga en bokningsapplikation för testkörningar av motorcyklar. Bakgrunden till detta handlar om att AVA erbjuder den potentiella köparen att testköra motorcykeln innan affären är i hamn och är då skyldig att fylla i ett 'Provkörningskort' med sin kundinformation, vilket sker manuellt och skrivs in i systemet för hand. 

Därför valde jag att utveckla en lösning där kunden skannar av en QR-kod och själv verifierar sin identitet med BankID kopplat till ett excelark där all testkörningsdata samlas. 

![[Pasted image 20260519225941.png]]

![[Screenshot_20260519_225905_DuckDuckGo.jpg]]

![[Screenshot_20260519_225917_DuckDuckGo.jpg]]

![[Screenshot_20260519_230014_DuckDuckGo.jpg]]

![[Screenshot_20260519_230049_DuckDuckGo.jpg]]

![[Screenshot_20260519_230105_DuckDuckGo.jpg]]

![[Screenshot_20260519_230123_DuckDuckGo.jpg]]

![[Pasted image 20260519231013.png]]

### Kopplingen till Kursplanen

Under praktikens gång har vi haft fria tyglar att använda oss av den tech stack som har passat vårt projekt. Vi använde Next.js + TypeScript & Tailwind CSS. All databashantering gick via Supabase och PostgresQL. Claude.ai skötte all kodgenerering. Allt detta är kunskaper vi har lärt oss under våra två år på Futuregames.

### Reflektion gällande förbättringsområden

Vårt projekt startade som ett blankt ark utan någon som helst struktur och även fast det har varit kul och lärorikt så känns det som att ens brister förstärks eftersom man själv står som ansvarig i slutändan.

Kommunikationen med våran klient är något jag har värdesatt. Att se saker och ting från användarens perspektiv är fundamentalt viktigt att träna på för att kunna utveckla rätt lösningar för deras verksamhet.

Till sist så hade jag önskat mig en projektledare som kunde tygla projektet och en senior utvecklare att bolla tekniska frågor med.

### Slutsats

I slutändan är jag väldigt stolt över det arbete vi genomfört. Vi startade från ingenting och slutade med någonting. Vi tvingades axla roller vi inte var bekväma i och gjorde det bästa av situationen. Vi hade full kreativ frihet att testa idéer och implementera 'features'. Jag är en rikare person idag än vad jag var igår, tack för det!