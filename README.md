# Webb-mom-5

Inlämningsuppgift moment 5
My Favourites
Förutsättningar:
 Använd Responsive Web mall exempelkod från Moment 1.
 Utgå från underlag i Classroom särskilt exempelkoden, lärarens lektion och länkar i detta
dokument.
 favouritesgrund.html och favourites.html ligger i ”c. Exempelkod” i1 Moment 5.
Uppgift
Du ska göra ett nytt formulär där användaren kan lägga in sina favoritländer som hen skulle vilja
besöka.
Uppgiften består av två delar en enklare och en svårare som bygger vidare på den enklare uppgiften.
Del 1 Skapa en lista med favoriter

Användaren ska kunna ange en id och ett land. När användaren trycker på knappen ska rubriken ”My
favourite list:” ändras till att innehålla användarens id och landet hen valde. Användaren ska kunna
välja flera länder men bara en åt gången och lägga till på listan.

Skapa en funktion som:
a) Använd favouritesgrund.html som finns i exempelkoden.
b) Spara undan formuläret i en variabel. Använd HTMLcollection.
c) Om det är en ny användare skriv ut en ny rubrik som innehåller det nya id:et. Använd
HTMLcollection item för att hämta id:et. Tänk på att du måste ta bort den gamla listan.

Sida 2 av 4
d) Skapa ett element att lägga listan i. Till exempel en div med document.createElement(”div”).
Lägg sedan innehållet i diven med egenskapen innerHTML.
e) Innehållet redigerar du så att det innehåller ordningsnummer, land och lämpliga element (till
exempel &lt;b&gt; för att de ska likna bilden ovan. Varje nytt land läggs till med metoden
appendChild().
f) Du ska skriva ett index på sidan för att hålla reda på ordningsnumret på landet. Listan ska
börja på 1.
g) Tänk på att det kan vara nödvändigt att rensa alla variabler varje gång användaren skapar en
ny lista.
h) Ni kan även integrera din nya sida i Responsiv mall med fungerande meny-system.
Här finns länkar med instruktioner förutom exempelkoden hur du kan använda ovanstående verktyg:
 Arbeta med HTMLcollection:
o https://developer.mozilla.org/en-US/docs/Web/API/HTMLCollection
o https://developer.mozilla.org/en-US/docs/Web/API/Document/forms
o https://www.w3schools.com/jsref/dom_obj_htmlcollection.asp
 Arbeta med element i HTMLcollection:
o https://www.w3schools.com/jsref/met_htmlcollection_item.asp
 createElement och appendChild:
o https://www.w3schools.com/jsref/met_document_createelement.asp
 innerHTML:
o https://www.w3schools.com/jsref/prop_html_innerhtml.asp

Del 2 Skapa en lista med favoriter som går att spara och hämta
Nu ska du skapa en ny sida utifrån första delen av uppgiften. Det ska gå att skapa en lista för varje
användare som du sedan ska kunna hämta med användar-id:et.
Som i del 1 ska användaren kunna ange en id och ett land. När användaren trycker på knappen ska
rubriken ”My favourite list:” ändras till att innehålla användarens id och landet hen valde.
Användaren ska kunna välja flera länder men en åt gången och lägga till på listan.

Nu ska det även gå att hämta listorna genom att ange användar-id:et och trycka på knappen ”Pick a
List”

Sida 3 av 4

Lägg till i den tidigare funktionen:
a. Varje gång du lagt in ett nytt land spara undan raden som du skrev på sidan i en array
b. Skriv in arrayen i en cookie med användar-id:et som identifikation. Använd funktionen
setCookie();
Skapa en ny funktion för att hämta sparade listor:
a) Använd favourites.html som finns i exempelkoden.
b) Spara undan formuläret i en variabel. Använd HTMLcollection.
c) Hämta id:et som vi ska använda för att söka cookien
d) Om det är en ny användare skriv ut en ny rubrik som innehåller det nya id:et. Använd
HTMLcollection item för att hämta id:et och hämta cookien med funktionen getCookie().
Tänk på att du måste ta bort den gamla listan.
e) Innehållet i cookien är en sträng. Omvandla den till en array med sträng-metoden split. Varje
land i strängen ska ha ett komma-tecken som avskiljare.
i) Loopa igenom arrayen med en for eller en for of loop. För varje land skapa ett element att
lägga listan i. Till exempel en div med document.createElement(”div”). Lägg sedan innehållet
i diven med egenskapen innerHTML. Samma som i första uppgiften punkt d. Varje nytt land
läggs till med metoden appendChild() som förut.
Förutom tidigare länkar behöver du även följande:
 Cookies:
o https://www.w3schools.com/js/js_cookies.asp
 Sträng-metoder split:
o https://www.w3schools.com/jsref/jsref_split.asp
 Loopar for och for in:
o https://www.w3schools.com/js/js_loop_for.asp
o https://www.w3schools.com/js/js_loop_forof.asp
