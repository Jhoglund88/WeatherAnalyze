# WeatherAnalyze
Ett Pythonprojekt som låter användaren hämta väderdata från en av tre städer via ett API och analyserar och sparar insamlad data.

## Mål
Jag vill skapa en väderapp som hämtar en vald stads sjudagarsprognos via API och sparar den i JSON för planering och analys. Projektet visar datainsamling och förberedelse av data inför eventuell AI-användning.

## Metod
1. Låta användaren välja en stad att hämta väderinfo om samt välja om detaljerad information ska visas.
2. Hämta väderinfon från Open-Meteo API med hjälp av Python biblioteket `requests`.
3. Skapa väderobjekt med klasserna Weather och DetailedWeather.
4. Spara väderdata och metadata i JSON-format.
5. Beräkna lägsta, högsta och genomsnittliga värden som hämtats.
6. Visa prognosen i diagram med matplotlib.
7. Rensa och normalisera värden som förberedelse för eventuell framtida AI-användning.

## Resultat
Programmet hämtade och sparade en sjudagarsprognos för 2-8 oktober (temperatur/vind) i Stockholm i en JSON-fil den 2 Oktober 2026.

Resultat för temperatur:
Lägsta: 7,6 °C
Högsta: 18,1 °C
Medel: 12,7 °C

Resultat för vind:

Lägsta: 1,0 km/h
Högsta: 25,5 km/h
Medel: 13,9 km/h

## Analys
I veckoprognosen varierar temperaturen i Stockholm mellan 7 och 18 °C och sjunker under natten. Vinden varierar mellan 1 och 25 km/h utan ett lika tydligt mönster. Eftersom prognosen bara gäller en stad och en vecka går det inte att dra långsiktiga slutsatser.

## Certifikat
PCEP certifierar grundläggande Pythonkunskaper. PCAP omfattar även objektorientering och filhantering. Båda är relevanta för mitt projekt. Vid framtida utveckling i molnet kan certifieringar från AWS eller Azure bli relevanta.

## Reflektion

Det gick bra att skapa funktioner, klasser och datarensning. Det svåraste var att koppla ihop API, objekt, JSON och felhantering, men det gav mig bättre förståelse för dataflödet. Jag valde JSON för att samla prognos och metadata. Arv minskar upprepning, även om en klass hade räckt för projektets storlek. Nästa steg är fler städer, vädervariabler och sparad historik.

## Användning av AI

Jag har använt AI som stöd för syntax vid API-anrop, felhantering, JSON, diagram. Har låtit Ai göra felsökning. Jag har granskat och anpassat AI-förslag samt ställt följdfrågor när jag behövt förstå koden bättre.

## Github-länk
https://github.com/Jhoglund88/WeatherAnalyze

## Installation/körning

1. Öppna `WeatherAnalyze.ipynb` i Jupyter Notebook eller VS Code med stöd för notebooks.
2. Installera biblioteken med `pip install requests matplotlib`.
3. Kör alla celler uppifrån och ned och välj stad samt om vindinformation ska visas.

Python 3 och internetanslutning krävs. Modulerna `json` och `datetime` ingår i Pythons standardbibliotek och behöver inte installeras separat.