<h1>Three Foxes Lounge</h1>

<h2>Testovací plán</h2>

<h2>Debug Divas</h2>

<h2>Hackathon 2024</h2>

Obsah

[1 Úvod 3](#1-úvod)

[1.1 Obecné informace o projektu 3](#11-obecné-informace-o-projektu)

[1.2 Cíle testovacího plánu 4](#12-cíle-testovacího-plánu)

[2 Rozsah projektu 4](#2-rozsah-projektu)

[2.1 User stories – funkce aplikace 4](#21-user-stories--funkce-aplikace)

[2.2 User stories – statické prvky aplikace 6](#22-user-stories--statické-prvky-aplikace)

[3 Horizonty vývoje a testování aplikace 6](#3-horizonty-vývoje-a-testování-aplikace)

[3.1 Krátkodobý plán projektu – Hackathon 7](#31-krátkodobý-horizont-projektu--hackathon)

[3.1.1 Týmová příprava 7](#311-týmová-příprava)

[3.1.2 Stanovení cílů a rozsahu testování 9](#312-stanovení-cílů-a-rozsahu-testování)

[3.1.3 Identifikace testovacích nástrojů a prostředí 10](#313-identifikace-testovacích-nástrojů-a-prostředí)

[3.1.4 Seznam prohlížečů a zařízení pro testování 10](#314-seznam-prohlížečů-a-zařízení-pro-testování)

[3.1.5 Testovací postup 11](#315-testovací-postup)

[3.2 Dlouhodobý plán projektu 12](#32-dlouhodobý-plán-projektu)

[3.2.1 Kontinuální zlepšování 12](#321-kontinuální-zlepšování)

[3.2.2 Strategické plánování pro budoucí verze a aktualizace aplikace 12](#322-strategické-plánování-pro-budoucí-verze-a-aktualizace-aplikace)

[3.2.3 Potenciální rizika testovacího procesu 13](#323-potenciální-rizika-testovacího-procesu)

# 1 Úvod

## 1.1 Obecné informace o projektu

Významný klient v oblasti hoteliérství zadal vytvoření aplikace pro nové ubytovací zařízení v malebném prostředí anglických lesů. Aplikace musí být připravena k online spuštění do 14 dnů od zadání, protože blížící se lovecká sezóna přiláká do regionu lovce z celého světa. To je ideální příležitost pro zviditelnění nového ubytovacího zařízení, Three Foxes Lounge.

Úspěšné a včasné dodání aplikace je zásadní, protože zpoždění či nedodání by mohlo způsobit klientovi výrazné finanční ztráty a negativně ovlivnit začátek nového podnikání. Navíc by mohlo dojít k poškození reputace tohoto exkluzivního ubytovacího zařízení.

Vývojářský tým dokázal aplikaci vytvořit během čtyř dní. Před jejím předáním klientovi je však nezbytné provést důkladné testování, aby byla zajištěna její kvalita a funkčnost. Úkolem testovacího týmu je aplikaci otestovat, poskytnout zpětnou vazbu vývojářům a tím přispět k úspěšnému spuštění možností rezervace v daném zařízení.

Protože spolupráce s tímto klientem bude pokračovat i po dodání aplikace a projekt bude dále rozvíjen, je důležité myslet i na budoucnost. Vývoj aplikace dneškem nekončí. Není nutné mít vše dokonale implementováno již nyní, ale je klíčové stanovit směr a způsob, jakým se bude testování aplikace v budoucnu ubírat.

Tento testovací plán detailně popisuje postupy a metody, které budou použity k zajištění kvality aplikace a definuje klíčové oblasti, které je třeba před spuštěním prověřit. Zároveň doporučuje postup testování v delším časovém horizontu a implementaci nástrojů a postupů sloužící k udržitelnosti projektu.

## 1.2 Cíle testovacího plánu

- Identifikace informací o projektu a softwarových komponent, které budou testovány
- Doporučení a popis testovacích strategií, které budou použity během testování
- Identifikace potřebných zdrojů (personál, nástroje) a odhad úsilí potřebného k testování (estimace)
- Vytvoření seznamu výstupů (dokumentů) z testování projektu
- Návrh testovací strategie z dlouhodobého hlediska (budoucnost a udržitelnost projektu)

# 2 Rozsah projektu

Projekt je definován ve spolupráci zákazníka a Product Ownera, přičemž obsahuje klíčové komponenty k testování, které jsou uspořádány podle jejich priority. Tento přístup umožňuje zaměřit se nejdříve na nejdůležitější funkce, čímž bude zajištěno, že kritické části projektu budou dokončeny včas a podle očekávání. Prioritizace komponent také umožňuje efektivnější plánování a rozdělení zdrojů, což přispívá k hladkému průběhu projektu a minimalizaci rizik spojených s jeho realizací.

## 2.1 User stories – funkce aplikace

<table class="table" cellpadding="10" cellspacing="0" style="border-collapse: collapse;">
  <tr>
    <th>Funkce</th>
    <th>Komponenty</th>
    <th>Priorita</th>
  </tr>
  <tr>
    <td rowspan="9">Reservation process</td>
    <td>Search for available rooms</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
  </tr>
  <tr>
    <td>Main page room reservation</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
  </tr>
  <tr>
    <td>Reservation of room from list of available rooms</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
  </tr>
  <tr>
    <td>Edit search criteria from list of available rooms</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Filtering results using amenities</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span>
  </div></td>
  </tr>
  <tr>
    <td>Clear filter</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Results sorting</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Filtering results using rating</td>
    <td ><div class="blue">
    <div class="color-box"></div>
    <span>Low</span></td>
  </tr>
  <tr>
    <td>Filtering results using price</td>
    <td ><div class="blue">
    <div class="color-box"></div>
    <span>Low</span></td>
  </tr>
    <td rowspan="11">Checkout</td>
    <td>Shopping cart</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
  </tr>
  <tr>
    <td>Checkout page</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
  </tr>
  <tr>
    <td>Payment methods</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
  </tr>
  <tr>
    <td>Online payment</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
  </tr>
  <tr>
    <td>Payment by Check</td>
    <td ><div class="high">
    <div class="color-box"></div>
    <span>High</span>
  </div></td>
  </tr>
  <tr>
    <td>Money transfer</td>
    <td ><div class="high">
    <div class="color-box"></div>
    <span>High</span>
  </div></td>
  </tr>
  <tr>
    <td>Additional facilities</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Terms And conditions</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Confirmation email</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Payment information email</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Guest/Account checkout</td>
    <td ><div class="blue">
    <div class="color-box"></div>
    <span>Low</span></td>
  </tr>
  <tr>
    <td rowspan="6">Accounts – login/registration</td>
    <td>Authentication page</td>
    <td ><div class="high">
    <div class="color-box"></div>
    <span>High</span>
  </div></td>
  </tr>
  <tr>
    <td>Login</td>
    <td ><div class="high">
    <div class="color-box"></div>
    <span>High</span>
  </div></td>
  </tr>
  <tr>
    <td>Log out</td>
    <td ><div class="high">
    <div class="color-box"></div>
    <span>High</span>
  </div></td>
  </tr>
  <tr>
    <td>My account page</td>
    <td ><div class="high">
    <div class="color-box"></div>
    <span>High</span>
  </div></td>
  </tr>
  <tr>
    <td>Create account</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Forgot password</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td rowspan="5">My Account</td>
    <td>Order history and details</td>
    <td ><div class="high">
    <div class="color-box"></div>
    <span>High</span>
  </div></td>
  </tr>
  <tr>
    <td>Order details</td>
    <td ><div class="high">
    <div class="color-box"></div>
    <span>High</span>
  </div></td>
  </tr>
  <tr>
    <td>Credit slips</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>My addresses</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>My personal information</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
</table>

## 2.2 User stories – statické prvky aplikace

<table class="table" cellpadding="10" cellspacing="0" style="border-collapse: collapse;">
  <tr>
    <th>Prvek</th>
    <th>Komponenta</th>
    <th>Priorita</th>
  </tr>
  <tr>
    <td rowspan="7">Shared and Common Features</td>
    <td>Footer section</td>
    <td ><div class="high">
    <div class="color-box"></div>
    <span>High</span>
  </div></td>
  </tr>
  <tr>
    <td>Header section</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Header – Login in header section</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Header – Shopping cart in header section</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Header – Menu in header section</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Newsletter subscription</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Language switcher</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td rowspan="6">Main Page</td>
    <td>Main sections of home page</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Default language selection</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
  <tr>
    <td>Interior section</td>
    <td ><div class="blue">
    <div class="color-box"></div>
    <span>Low</span></td>
  </tr>
  <tr>
    <td>Amenities section</td>
    <td ><div class="blue">
    <div class="color-box"></div>
    <span>Low</span></td>
  </tr>
  <tr>
    <td>Our rooms section</td>
    <td ><div class="blue">
    <div class="color-box"></div>
    <span>Low</span></td>
  </tr>
  <tr>
    <td>Testimonials section</td>
    <td ><div class="blue">
    <div class="color-box"></div>
    <span>Low</span></td>
  </tr>
  <tr>
    <td rowspan="3">Non functional requirements</td>
    <td>Website protocol</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
  </tr>
  <tr>
    <td>GDPR</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
  </tr>
  <tr>
    <td>SEO optimalization</td>
    <td ><div class="yellow">
    <div class="color-box"></div>
    <span>Medium</span></td>
  </tr>
</table>

# 3 Horizonty vývoje a testování aplikace

Vývoj a testování aplikace lze efektivně strukturovat na základě dvou časových horizontů: krátkodobého a dlouhodobého. Krátkodobý horizont se zaměřuje na bezprostřední cíle a úkoly, které jsou plánovány pro nadcházející Hackathon. Tento horizont zahrnuje detaily úkolů, jež je nutné splnit během Hackathonu, přidělení rolí a odpovědností v týmu, přípravu prostředí a nástrojů nezbytných pro testování a vývoj, a stanovení konkrétních výstupů a cílů.

Naopak dlouhodobý horizont se soustředí na udržitelnost a rozvoj aplikace v průběhu jejího životního cyklu. Tento horizont zahrnuje strategické plánování pro budoucí verze a aktualizace aplikace, definování postupů pro efektivní a kontinuální testování, identifikaci a implementaci osvědčených postupů a metodik pro dlouhodobé testování, doporučení pro implementaci nástrojů a technologií, a plánování školení a rozvoje týmu. Tato struktura umožňuje efektivní řízení jak bezprostředních, tak dlouhodobých cílů, což zajišťuje, že aplikace bude nejen připravena na krátkodobé události, jako je Hackathon, ale také udržitelná a efektivní z hlediska dlouhodobého vývoje a testování.

## 3.1 Krátkodobý horizont projektu – Hackathon

### 3.1.1 Týmová příprava

Zhruba týden před konáním Hackathonu jsme naplánovali schůzku spolu s naším mentorem a diskutovali o týmové strategii. Nakonec jsme se dohodli na následujících bodech:

1.  Nebudeme mít SCRUM Mastera

    a. Vyhovovala nám definice SCRUM týmu jako samořiditelné jednotky s důrazem na vzájemnou spolupráci. V rámci Digitální akademie jsme absolvovaly tři sprinty, během nichž jsme zjistily, že v našich podmínkách SCRUM Master neplní roli tak, jak je obvykle definována (tj. spíše jako kouč). Tři z nás měly možnost si tuto roli během sprintů vyzkoušet. Vzhledem k nedostatku zkušeností s touto seniorní pozicí jsme však v některých sprintech nechtěně sklouzly k tomu, že SCRUM Master fungoval spíše jako projektový manažer, který zadává úkoly. Tohoto přístupu jsme se chtěly vyvarovat.

    b. Zohlednily jsme také skutečnost, že Hackathon je jednodenní projekt,
    a proto nebyla role SCRUM Mastera tak nezbytná. Namísto toho jsme
    potřebovaly maximalizovat počet člověkohodin věnovaných samotnému
    testování a souvisejícím činnostem. Na druhou stranu jsme již měly
    zkušenost z předchozích sprintů a dobře jsme se navzájem znaly, což
    nám umožnilo efektivně využít naše dovednosti a vědět, na koho se
    můžeme v konkrétních situacích obrátit.

2.  Příprava podkladů a dokumentace:

    a. Sdílený dokument:

    - Vzorové šablony pro test case a bug report

    - Myšlenková mapa

    - Struktura složek v Postmanu pro případné API testy

    - Shrnutí pravidel odsouhlasených během uplynulých tří sprintů

    - Na co si dávat pozor při reportování v systému Jira

    - Jak efektivně pojmenovávat test case a bug report, aby byly snadno pochopitelné a předešlo se duplicitám

    - Odkaz na uvedený [Checklist](https://docs.google.com/spreadsheets/d/15ME-jIUTQBHlJ_v-eYZdHrpyr3_4OLuc/edit#gid=1696534826)

d. Individuální příprava

- Každá z nás se zaměřila na oblasti, které ji nejvíce zajímaly z hard
  skills, které jsme se v akademii učily, a ty jsme v rámci našich
  možností dále rozvíjely

c. Připravené základní podklady s ohledem na neznalost zadání:

-     Poznámky k testování SQL
-     Requesty pro API
-     Šablony pro automatizované testy
-     Tabulky pro risk-based analýzu

3.  Individuální seznámení s aplikací

- Doba trvání: minimálně dvě hodiny
- Aktivity:

  - Prostředí aplikace a analýza aplikace, exploratory testing

  - Dokumentace v systému Jira

  - Prostudování dostupných podkladů

  - Příprava materiálů potřebných pro testování

4.  Předem nastavený proces

- Stand-upy po cca 45 minutách maximálně soustředěné práce
- Hlídání délky trvání stand-upu a neodbíhání od témat společných všem

### 3.1.2 Stanovení cílů a rozsahu testování

Analýza aplikace počíná prostudováním obchodních a technických požadavků aplikace a diskusí s Product Ownerem pro lepší porozumění.

<table class="table" cellpadding="10" cellspacing="0" style="border-collapse: collapse;">
  <tr>
    <th colspan="2">Cíl testování: Zajistit správnou funkčnost testované aplikace</th>
  </tr>
  <tr>
    <td><strong>Technika:</strong></td>
    <td>
      Testování vybraných funkcí (user stories) s použitím platných a neplatných dat za účelem ověření následujícího:<br>
      - Očekávané výsledky se objeví při použití platných dat.<br>
      - Při použití neplatných dat se zobrazí příslušné chybové nebo varovné zprávy.
    </td>
  </tr>
  <tr>
    <td><strong>Definition of Ready:</strong></td>
    <td>
      US má jasný popis, definované požadavky, stanovenou prioritu.<br>
      Dokumentace a technická specifikace je k dispozici.<br>
      Testovací prostředí je připraveno.<br>
      Zadání bylo schváleno stakeholdery (zákazník, product owner).<br>
      Jsou k dispozici potřebné nástroje.
    </td>
  </tr>
  <tr>
    <td><strong>Definition of Done:</strong></td>
    <td>
      Všechny plánované testy jsou provedeny.<br>
      Všechny chyby s vysokou prioritou a závažností jsou nahlášeny.<br>
      Výsledky testů jsou vyhodnoceny, prodiskutovány a schváleny.<br>
      Produkt nemá otevřené závažné chyby bránící nasazení.<br>
      Předměty na otestování aplikace a zaprotokolování chyb předá vývojáři testovacích scénářů nebo ten, který je znovu zprovoznitelný.<br>
      <span style="color:blue;">Aplikace je responzivní (i pro mobilní zařízení).</span><br>
      <span style="color:green;">Aplikace je bezpečná.</span>
    </td>
  </tr>
</table>

Hlavním cílem je test těch komponent aplikace, které jsou označeny jako vysoce prioritní a souvisejí se základní funkčností aplikace. Jedná se konkrétně o následující user stories, ke kterým bude přiřazen konkrétní člen týmu:
Ось HTML-код для таблиці, яку ви надали:

<table class="table" cellpadding="10" cellspacing="0" style="border-collapse: collapse;">
  <tr>
    <th>Funkce</th>
    <th>Komponenty</th>
    <th>Priorita</th>
    <th>Assigned</th>
  </tr>
  <tr>
    <td rowspan="3">Reservation process</td>
    <td>Search for available rooms</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
    <td>Petra S.</td>
  </tr>
  <tr>
    <td>Main page room reservation</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
    <td>Markéta Ch.</td>
  </tr>
  <tr>
    <td>Reservation of room from list of available rooms</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
    <td>Petra S.</td>
  </tr>
  <tr>
    <td rowspan="4">Checkout</td>
    <td>Shopping cart</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
    <td>Michaela Š.</td>
  </tr>
  <tr>
    <td>Checkout page</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
    <td>Eva A.</td>
  </tr>
  <tr>
    <td>Payment methods</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
    <td>Inna D.</td>
  </tr>
  <tr>
    <td>Online payment</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
    <td>Inna D.</td>
  </tr>
  <tr>
    <td rowspan="2">Non functional requirements</td>
    <td>Website protocol</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
    <td>Simona P. J.</td>
  </tr>
  <tr>
    <td>GDPR</td>
    <td ><div class="highest">
    <div class="color-box"></div>
    <span>Highest</span>
  </div></td>
    <td>Simona P. J.</td>
  </tr>
</table>

### 3.1.3 Identifikace testovacích nástrojů a prostředí

<table class="table" cellpadding="10" cellspacing="0" style="border-collapse: collapse;">
  <tr>
    <th>Funkce</th>
    <th>Nástroj</th>
  </tr>
  <tr>
    <td>Reportování testovacích scénářů a chyb</td>
    <td>Jira<br>Zephyr – doplněk k systému Jira</td>
  </tr>
  <tr>
    <td>Testování na API vrstvě</td>
    <td>Postman</td>
  </tr>
  <tr>
    <td>Automatizované testování</td>
    <td>Visual Studio Code<br>Playwright</td>
  </tr>
  <tr>
    <td>Vytvoření zálohy</td>
    <td>Git Kraken<br>Github</td>
  </tr>
  <tr>
    <td>Práce s databází aplikace</td>
    <td>MySQL</td>
  </tr>
  <tr>
    <td style="background-color: #ffffcc;">Doplňkové</td>
    <td>DevTools<br>Chat GPT v. 4.0<br>Codeium – doplněk pro VS Code</td>
  </tr>
</table>

### 3.1.4 Seznam prohlížečů a zařízení pro testování

<div style="display: flex;">
  <table class="table" cellpadding="10" cellspacing="0" style="border-collapse: collapse; margin-right: 20px;">
    <tr>
      <th >Prohlížeče</th>
    </tr>
    <tr>
      <td>Chrome</td>
    </tr>
    <tr>
      <td>Firefox</td>
    </tr>
    <tr>
      <td>Safari</td>
    </tr>
    <tr>
      <td>Edge</td>
    </tr>
  </table>

  <table class="table" cellpadding="10" cellspacing="0" style="border-collapse: collapse;">
    <tr>
      <th style="background-color: #e6ffe6;">Zařízení</th>
    </tr>
    <tr>
      <td>Desktop – Windows 10</td>
    </tr>
    <tr>
      <td>Desktop – macOS Sonoma 14.4.1</td>
    </tr>
    <tr>
      <td>Android zařízení</td>
    </tr>
    <tr>
      <td>iOS zařízení</td>
    </tr>
  </table>
</div>

### 3.1.5 Testovací postup

1.  Příprava testovacích případů:

- Vytváření testovacích scénářů na základě požadavků.
- Psaní podrobných testovacích případů s jasnými vstupy, kroky a očekávanými výsledky.
- Vytvoření requestů pro testování na API vrstvě - HODIT DO PROVEDENÍ - [link](https://drive.google.com/file/d/19Din16TSh9rZHc4NBPOnZJbIgGTutAMP/view?usp=share_link)
- Vytvoření automatizovaných testů

2.  Provedení testů:

- Funkční testování: Ověření, že všechny funkce softwaru fungují podle specifikací.
- Testování kompatibility: Ověření, že software funguje správně na různých webových prohlížečích a různých zařízeních.
- Testování bezpečnosti: Ověření protokolu webové aplikace a právních norem v souvislosti s cílem aplikace.
- Manuální provádění testovacích případů podle předem definovaných kroků.
- Spuštění automatizovaných testů.
- Dokumentace výsledků každého testovacího případu.

3.  Zaznamenání chyb:

- Identifikace a dokumentace chyb a nedostatků.
- Vytváření podrobných bug reportů s kroky k replikaci, očekávaným a aktuálním výsledkem a prioritou chyby.

4.  Příprava dokumentace:

- Sestavení zprávy o výsledcích testování, včetně testovacího plánu a hlášení o chybách.
- Shrnutí klíčových nálezů, metrik a doporučení.

## 3.2 Dlouhodobý plán projektu

Níže jsou uvedeny klíčové oblasti zaměřené na zlepšení a strategické plánování testování aplikace, spolu s několika konkrétními kroky a doporučeními.

### 3.2.1 Kontinuální zlepšování

1.  Analýza výsledků testování:

- Nutné pro identifikaci slabých míst a oblastí, které potřebují zlepšení.
- Používat tyto analýzy k formulování konkrétních kroků pro zvýšení kvality softwaru.

3.  Aktualizace testovacích případů a strategií:

- Na základě požadavků zákazníka průběžně aktualizovat testovací případy a přizpůsobovat testovací strategii.

### 3.2.2 Strategické plánování pro budoucí verze a aktualizace aplikace

1.  Stanovení kritérií kvality

- Produkt musí fungovat v souladu s požadavky a funkční specifikací
- Konečná verze projektu nesmí obsahovat kritické a blokující chyby.

2.  Definování postupů pro efektivní a kontinuální testování:

- Vytvoření a udržování procesů, které zajistí konzistentní a efektivní testování všech verzí aplikace.
- Zajištění, že tyto procesy podporují vysokou kvalitu a spolehlivost aplikace.

3.  Identifikace a implementace osvědčených postupů a metodik:

- Regresní testování: Ověření, že nové změny neovlivní stávající funkcionality.
- Sanity testing (bugfix): Opětovné testování po opravě chyb.
- Automatizace testovacích procesů: Zavedení nástrojů pro automatizované testování k zvýšení efektivity a pokrytí.
- Pravidelné code reviews: Zajištění kvality kódu prostřednictvím pravidelných kontrol.

4.  Doporučení pro implementaci nástrojů a technologií pro:

- automatizované testování
- CI/CD procesy
- testování výkonu (performance testy) v JS v Grafana k6
- integrační testy
- testování API
- testování uživatelského rozhraní z hlediska srozumitelnosti a vizuálního dojmu
- testování použitelnosti a přívětivosti aplikace
- testování spouštění a běhu aplikace: Hodnocení, jak se software spouští a běží na podporovaných prohlížečích a zařízeních, včetně času potřebného ke spuštění

### 3.2.3 Potenciální rizika testovacího procesu

<table class="table" cellpadding="10" cellspacing="0" style="border-collapse: collapse;">
  <tr>
    <th style="background-color: #ffcccc;">Riziko</th>
    <th style="background-color: #ffcccc;">Dopad</th>
    <th style="background-color: #ffcccc;">Preventivní opatření</th>
  </tr>
  <tr>
    <td>Testovací tým nemá aktuální a platné dokumenty</td>
    <td>Nesprávné testování, možné přehlédnutí chyb</td>
    <td>Zajistit, aby tým měl vždy přístup k aktuálním dokumentům</td>
  </tr>
  <tr>
    <td>Nedostatek potřebného vybavení, nástrojů, zařízení a softwaru</td>
    <td>Zpoždění testovacího procesu, neúplné testování</td>
    <td>Připravit a zajistit veškeré potřebné vybavení před zahájením testování</td>
  </tr>
  <tr>
    <td>Kritické chyby nejsou opraveny včas</td>
    <td>Vysoké riziko výskytu závažných problémů v produkci</td>
    <td>Opravit všechny kritické chyby co nejdříve</td>
  </tr>
  <tr>
    <td>Chybí poznámky k aktualizaci aplikace nebo jsou nedostatečné</td>
    <td>Nejasnosti ohledně nových funkcí a změn, riziko nesprávného použití softwaru</td>
    <td>Přikládat poznámky k vydání ke každé nové verzi softwaru, vysvětlit nové prvky a jejich dopad</td>
  </tr>
  <tr>
    <td>Neplánované a neprojednané změny a úpravy aplikace</td>
    <td>Potenciální destabilizace aplikace, nesoulad s původními požadavky</td>
    <td>Zavést proces schvalování a dokumentace všech změn a úprav před jejich implementací</td>
  </tr>
  <tr>
    <td>Neprojednané změny v softwaru používaného při vývoji aplikace</td>
    <td>Riziko nesouladu mezi vývojem a testovacím týmem, zvýšené náklady na redesign</td>
    <td>Zajistit, aby všechny změny v požadavcích byly projednány a schváleny relevantními stranami</td>
  </tr>
</table>
