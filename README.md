# WeatherAnalyze
Ett Pythonprojekt som låter användaren hämta väderdata från en av tre städer via ett API och analyserar insamlad data.

## Mål
Mitt mål är att göra en enkel väderapp där användaren genom en meny får välja en stad som den vill hämta väderinfo om. Därefter så ska sjudagarsprognos hämtas med hjälp av ett API-anrop och sedan sparas ner i JSON-format för att senare kunna bearbetas, analyseras och visualiseras.

Projektet tränar datainsamling och databearbetning som kan ingå i förberedelsen av data för AI-system och har därför en tydlig koppling till AI-utvecklarrollen.

## Metod
1. Låta användaren välja en stad att hämta väderinfo om samt välja om detaljerad information ska visas.
2. Hämta väderinfon från Open-Meteo API med hjälp av Python biblioteket `requests`.
3. Skapa väderobjekt med klasserna Weather och DetailedWeather.
4. Spara väderdata och metadata i JSON-format.
5. Beräkna lägsta, högsta och genomsnittliga värden som hämtats.
6. Visa prognosen i diagram med matplotlib.
7. Rensa och normalisera värden som förberedelse för eventuell framtida AI-användning.

## Resultat


## Analys


## Certifikat
PCEP certifierar grundläggande Pythonkunskaper. PCAP omfattar även objektorientering och filhantering. Båda kopplar till mitt projekt. Vid framtida utveckling i molnet kan certifieringar från AWS eller Azure bli relevanta.

## Reflektion

Det svåraste var att få ihop flödet mellan API-anropet, objekten och sparningen till JSON samt att förstå hur felhanteringen skulle byggas upp. Under projektets gång har jag fått en bättre förståelse för hur data hämtas från ett API och sedan kan bearbetas och sparas.

Nästa gång skulle jag vilja utveckla programmet så att användaren kan hämta prognoser för fler städer och välja fler typer av väderdata att analysera. 

Jag tänkte först spara flera prognoser men valde denna lösning nu för att förenkla programmet, därför kan en framtida förbättring bli att spara historiken.

Jag valde JSON eftersom väderdata och metadata kan sparas tillsammans i en tydlig struktur. 

Arv gör att DetailedWeather kan återanvända attribut från Weather och lägga till vindhastighet. Det minskar upprepning, men för en så liten lösning hade en enda klass med valbar vindinformation också varit möjlig.

## Användning av AI

Jag har använt AI som en studiehandledare och som stöd för syntax, felsökning och granskning av kod. I vissa delar har AI föreslagit kod som jag har gått igenom, anpassat och använt i projektet. Jag har framför allt fått hjälp med:

- API-anropet och de parametrar som används för att hämta väderdata.
- Syntax och felhantering vid sparning till JSON samt metadata.
- Syntax för diagram och normalisering av data.
- Granskning och felsökning av befintlig kod.
- Formulering och granskning av markdowntexter.

När jag inte har förstått kod eller förslag från AI har jag ställt följdfrågor och gått igenom koden för att förstå hur den fungerar.

## Github-länk
https://github.com/Jhoglund88/WeatherAnalyze

## Installation/körning

1. Öppna `WeatherAnalyze.ipynb` i Jupyter Notebook eller VS Code med stöd för notebooks.
2. Installera biblioteken med `pip install requests matplotlib`.
3. Kör alla celler uppifrån och ned och välj stad samt om vindinformation ska visas.

Python 3 och internetanslutning krävs. Modulerna `json` och `datetime` ingår i Pythons standardbibliotek och behöver inte installeras separat.