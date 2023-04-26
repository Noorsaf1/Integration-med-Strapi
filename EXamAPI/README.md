För att använda Postman behöver du först installera programmet på din dator.

När du har startat Postman klickar du på "New" knappen och väljer sedan "HTTP Request".

Därifrån kan du välja vilken metod du vill använda, till exempel GET, och sedan ange URL:en för den information du vill hämta.

Till exempel, om du vill ha information om TV-apparater, skulle du använda URL:en http://localhost:3000/Computers.

Om du vill ha information om ljud, mobiler eller datorer kan du ersätta "televisions" med den lämpliga termen.

Detta gäller också för metoderna POST, PUT och DELETE. Om du vill använda en mer avancerad text, följ instruktionerna nedan:

Använda POST, PUT och DELETE i Postman
Välj den metod du vill använda i rullgardinsmenyn bredvid URL-fältet (GET, POST, PUT eller DELETE).

Ange URL:en för resursen du vill interagera med, till exempel http://localhost:3000/Computers för att skapa, uppdatera eller ta bort en TV-apparat.

Om du behöver autentisera dig, klicka på "Authorization" fliken och välj "Bearer Token" från typmenyn. Klistra in din JWT i fältet "Token".

För POST och PUT-förfrågningar, klicka på "Body" fliken och välj "raw" och "JSON" format. Skriv in nycklar och värden för de fält du vill skicka i förfrågans kropp, till exempel:

json
Copy code
{
    "name": "Example Computers",
    "description": "A great Computers",
    "manufacturer": "Example Corp",
    "price": 1200,
    "screen_size": 55
}
Klicka på "Send" knappen för att skicka förfrågan. Svaret visas i "Response" avsnittet nedan.

