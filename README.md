Prompting Handbook
====================
- [Prompting Handbook](#prompting-handbook)
  * [Wstęp](#wstęp)
  * [1) Precyzyjnie formułuj instrukcje](#1--precyzyjnie-formu-uj-instrukcje)
  * [2) Oddzielaj instrukcje od treści promptu](#2--oddzielaj-instrukcje-od-tre-ci-promptu)
    + [Przykłady złych vs. dobrych promptów:](#przyk-ady-z-ych-vs-dobrych-prompt-w--1)
    + [👉 Kluczowe elementy oddzielania instrukcji:](#---kluczowe-elementy-oddzielania-instrukcji-)
    + [Praktyczne wskazówki:](#praktyczne-wskaz-wki--1)
    + [💡 Przykład kompleksowego promptu:](#---przyk-ad-kompleksowego-promptu--1)
  * [3) Nadawaj modelowi konkretną rolę](#3-nadawaj-modelowi-konkretną-rolę)
    + [Przykłady złych vs. dobrych promptów:](#przyk-ady-z-ych-vs-dobrych-prompt-w--2)
    + [👉 Popularne role do wykorzystania:](#---popularne-role-do-wykorzystania-)
    + [Praktyczne wskazówki:](#praktyczne-wskaz-wki--2)
    + [💡 Przykład kompleksowego promptu:](#---przyk-ad-kompleksowego-promptu--2)

## Wstęp
Hej, witam Cię drogi czytelniku! Ten ebook ma na celu przedstawić Ci najważniejsze techniki pisania promptów dla modeli językowych. Jeśli więc kożystasz z np. chataGPT, Cloude.ai lub bezpośrednio z jakiegoś modelu LLM to ten poradnik jest właśnie dla Ciebie.

Ułożyłem go w formie krótkich punktów tak, żeby się nie rozpisywać i żebyś mógł szybko z niego skorzystać.

Także poniżej lista najważniejszych dobrych praktyk pisania promptów:

## 1) Precyzyjnie formułuj instrukcje

Jedną z najważniejszych zasad tworzenia skutecznych promptów jest precyzyjne formułowanie instrukcji. Model językowy nie potrafi czytać w naszych myślach - będzie działał dokładnie według tego, co napiszemy. Im bardziej szczegółowa i jednoznaczna instrukcja, tym lepsze rezultaty otrzymamy.

**Dlaczego precyzja jest kluczowa?**

Modele LLM interpretują nasze polecenia dosłownie. Brak precyzji może prowadzić do niepełnych odpowiedzi lub odpowiedzi niezgodnych z tematem.

### Przykłady złych vs. dobrych promptów:

<details>
  <summary>Przykład 1</summary>
  
❌ Źle: "Napisz o Świętym Mikołaju."

✅ Dobrze: "Napisz opis postaci Świętego Mikołaja uwzględniając jego pochodzenie historyczne, tradycje w różnych krajach oraz współczesny wizerunek. Tekst powinien zawierać informacje o stroju, atrybutach i zwyczajach związanych z wręczaniem prezentów."
</details>

<details>
  <summary>Przykład 2</summary>
  
❌ Źle: "Zrób listę prezentów."

✅ Dobrze: "Stwórz listę 10 pomysłów na prezenty świąteczne dla dzieci w wieku 5-7 lat, w przedziale cenowym 50-100 zł. Uwzględnij zarówno zabawki edukacyjne, jak i rozrywkowe, dodaj krótki opis każdego prezentu."
</details>

### 👉 Kluczowe elementy precyzyjnej instrukcji:

1. Określenie formatu odpowiedzi
2. Podanie konkretnych liczb/wartości
3. Wyszczególnienie wymaganych elementów
4. Zdefiniowanie kontekstu
5. Określenie ograniczeń

> ### Praktyczne wskazówki:
> - Używaj punktów lub numeracji dla złożonych poleceń
> - Określaj pożądaną długość odpowiedzi
> - Wskazuj docelowego odbiorcę
> - Definiuj poziom szczegółowości

### 💡 Przykład kompleksowego promptu:

```
Napisz artykuł na bloga o znaczeniu symbolu choinki w Polsce. Artykuł powinien:
- mieć długość 800-1000 słów
- zawierać 5 konkretnych korzyści posidania choinki w domu na Święta
- być napisany przystępnym językiem dla osób początkujących
- zawierać praktyczne wskazówki jak kupić choinkę
- kończyć się podsumowaniem i zachętą do działania
```
***
## 2) Oddzielaj instrukcje od treści promptu

Kolejną kluczową zasadą jest wyraźne oddzielanie instrukcji dotyczących formy i sposobu odpowiedzi od właściwej treści promptu. Takie podejście pomaga modelowi lepiej zrozumieć, czego dokładnie od niego oczekujemy i jak ma przetworzyć podane informacje.

**Dlaczego oddzielanie jest ważne?**

Gdy instrukcje i treść są przemieszane, model może mieć trudność z rozróżnieniem co jest poleceniem, a co treścią do przetworzenia. Może to prowadzić do nieprawidłowych lub niekompletnych odpowiedzi.

### Przykłady złych vs. dobrych promptów:

<details>
  <summary>Przykład 1</summary>
  
❌ Źle: "Napisz profesjonalny list do świętego Mikołaja po angielsku z prośbą o prezent i dodaj formalny ton."

✅ Dobrze: 
"Instrukcje:
- Napisz list do śwętego Mikołaja w języku angielskim
- Użyj formalnego tonu
- Długość: 150-200 słów

Treść:
Prośba do świętego Mikołaja o nowe klocki LEGO."
</details>

<details>
  <summary>Przykład 2</summary>
  
❌ Źle: "Streść ten artykuł naukowy w prostych słowach i zrób to w formie punktów."

✅ Dobrze:
"Instrukcje:
- Przygotuj streszczenie w formie punktów
- Użyj prostego, nietechnicznego języka
- Zachowaj najważniejsze wnioski
- Maksymalnie 5-7 punktów

Tekst do streszczenia:
[treść artykułu naukowego]"
</details>

### 👉 Kluczowe elementy oddzielania instrukcji:

1. Wyraźne nagłówki (np. "Instrukcje:", "Treść:", "Kontekst:")
2. Formatowanie wizualne (odstępy, punktory)
3. Hierarchiczna struktura informacji
4. Jasne rozgraniczenie poleceń od materiału źródłowego

> ### Praktyczne wskazówki:
> - Używaj sekcji i podsekcji
> - Stosuj formatowanie tekstu (jeśli dostępne)
> - Numeruj kolejne instrukcje
> - Grupuj podobne polecenia

### 💡 Przykład kompleksowego promptu:
```
INSTRUKCJE FORMATOWANIA:
- Format: post na LinkedIn
- Długość: 200-250 słów
- Styl: profesjonalny ale przystępny
- Dodaj 2-3 hashtagi na końcu

INSTRUKCJE DOTYCZĄCE TREŚCI:
- Podkreśl główne zalety produktu
- Dodaj jeden przykład zastosowania
- Zakończ call-to-action

TREŚĆ DO PRZETWORZENIA:
[Opis produktu, który ma być promowany]
```
***
## 3) Nadawaj modelowi konkretną rolę

Określenie konkretnej roli dla modelu językowego znacząco wpływa na jakość i trafność otrzymywanych odpowiedzi. Kiedy model "wie", jaką rolę ma odgrywać, może lepiej dostosować ton, słownictwo i poziom szczegółowości odpowiedzi.

**Dlaczego rola jest ważna?**

Przypisanie roli pomaga modelowi lepiej zrozumieć kontekst i oczekiwania, a także dostosować sposób komunikacji do danej sytuacji. To jak instruowanie aktora, jaką postać ma zagrać w przedstawieniu świątecznym.

### Przykłady złych vs. dobrych promptów:

<details>
  <summary>Przykład 1</summary>
  
❌ Źle: "Wytłumacz dzieciom, skąd się biorą prezenty pod choinką."

✅ Dobrze: "Wciel się w rolę pomocnika Świętego Mikołaja i wytłumacz 6-letnim dzieciom, w magiczny i przyjazny sposób, jak działa proces dostarczania prezentów w Wigilię. Używaj prostego języka i odwołuj się do wyobraźni dzieci."
</details>

<details>
  <summary>Przykład 2</summary>
  
❌ Źle: "Napisz przepis na pierniki."

✅ Dobrze: "Jako doświadczony cukiernik specjalizujący się w wypiekach świątecznych, przedstaw szczegółowy przepis na tradycyjne pierniki. Uwzględnij profesjonalne wskazówki i sekrety, które sprawiają, że pierniki są wyjątkowo smaczne i aromatyczne."
</details>

### 👉 Popularne role do wykorzystania:

1. Ekspert w danej dziedzinie
2. Nauczyciel/mentor
3. Doradca
4. Krytyk
5. Storyteller

> ### Praktyczne wskazówki:
> - Określaj poziom ekspertyzy roli
> - Dodawaj kontekst do roli
> - Precyzuj styl komunikacji
> - Definiuj "osobowość" roli

### 💡 Przykład kompleksowego promptu:
```
Wciel się w rolę doświadczonego dekoratora wnętrz specjalizującego się w aranżacjach świątecznych z 15-letnim stażem. Przygotuj poradnik dekorowania domu na Święta, który:
- uwzględnia najnowsze trendy na rok 2023
- zawiera praktyczne wskazówki dotyczące doboru kolorów
- proponuje rozwiązania dla różnych budżetów
- podaje konkretne przykłady dekoracji
- uwzględnia zasady zrównoważonego rozwoju
Pisz w profesjonalnym, ale przystępnym tonie, używając specjalistycznej terminologii z wyjaśnieniami.
```
***
## 4) Określaj styl i ton wypowiedzi

Precyzyjne określenie stylu i tonu wypowiedzi jest kluczowe dla uzyskania odpowiedniego rezultatu. Modele LLM potrafią dostosować się do różnych stylów komunikacji - od formalnego po casualowy, od entuzjastycznego po poważny. Najskuteczniejszą metodą jest podanie przykładu wypowiedzi w pożądanym tonie.

**Dlaczego określanie stylu jest ważne?**

Ten sam komunikat może być odebrany zupełnie inaczej w zależności od sposobu jego przekazania. Odpowiedni ton pomaga w skuteczniejszej komunikacji z docelowym odbiorcą i realizacji zamierzonych celów.

### Przykłady złych vs. dobrych promptów:

<details>
  <summary>Przykład 1</summary>
  
❌ Źle: "Napisz ogłoszenie o przybyciu Świętego Mikołaja do centrum handlowego."

✅ Dobrze: "Napisz ogłoszenie o przybyciu Świętego Mikołaja do centrum handlowego. Użyj entuzjastycznego, radosnego tonu, podobnego do tego:
'Hurra! Mamy wspaniałe wieści dla wszystkich małych i dużych marzycieli! 🎅✨ Czy jesteście gotowi na magiczne spotkanie?'"
</details>

<details>
  <summary>Przykład 2</summary>
  
❌ Źle: "Napisz mail do pracowników o świątecznej przerwie."

✅ Dobrze: "Napisz mail do pracowników o świątecznej przerwie używając profesjonalnego, ale ciepłego tonu, jak w przykładzie:
'Szanowni Współpracownicy, z przyjemnością informuję, że zbliża się nasz zasłużony czas świątecznego odpoczynku...'"
</details>

### 👉 Popularne style wypowiedzi:

1. Formalny i profesjonalny
2. Przyjazny i casualowy
3. Entuzjastyczny i energiczny
4. Edukacyjny i wyjaśniający
5. Empatyczny i wspierający
6. Humorystyczny i lekki

> ### Praktyczne wskazówki:
> - Zawsze podawaj przykład pożądanego tonu
> - Określaj docelową grupę odbiorców
> - Wskazuj poziom formalności
> - Definiuj emocje, które tekst ma wywołać

### 💡 Przykład kompleksowego promptu:
```
INSTRUKCJE:
Napisz post na Facebook o warsztatach świątecznych dla dzieci.

STYL:
Entuzjastyczny i przyjazny dla rodziców, podobny do:
"Kochani Rodzice! 🎄 Czy Wasze pociechy są gotowe na magiczną przygodę? Przygotowaliśmy coś wyjątkowego, co sprawi, że ich oczka zabłysną jaśniej niż świąteczne lampki! ✨"

WYMAGANIA:
- Długość: 100-150 słów
- Dodaj emotikony
- Zawrzyj praktyczne informacje
- Zakończ call-to-action

TREŚĆ:
[Szczegóły warsztatów do opisania]
```
***
## 5) Zero-shot prompting - proste i skuteczne podejście

Zero-shot prompting to technika, w której model językowy wykonuje zadanie bez wcześniejszych przykładów czy specjalnego treningu. Jest to najbardziej podstawowa forma promptingu, ale często bardzo skuteczna. Warto od niej zacząć i jeśli efekt nie będzie zadowalający spróbować bardziej zaawansowanych metod.

**Dlaczego zero-shot jest użyteczny?**

Ta metoda jest szczególnie przydatna, gdy chcemy szybko uzyskać odpowiedź bez skomplikowanego kontekstu czy przykładów. Jest to także dobry sposób na przetestowanie podstawowych możliwości modelu.

### Przykłady złych vs. dobrych promptów:

<details>
  <summary>Przykład 1</summary>
  
❌ Źle: "Co sądzisz o świętach?"

✅ Dobrze: "Wymień 5 najważniejszych tradycji Bożonarodzeniowych w Polsce i krótko wyjaśnij znaczenie każdej z nich."
</details>

<details>
  <summary>Przykład 2</summary>
  
❌ Źle: "Napisz coś o reniferach."

✅ Dobrze: "Sklasyfikuj renifery Świętego Mikołaja według ich tradycyjnych imion i opisz charakterystyczne cechy każdego z nich."
</details>

### 👉 Kluczowe elementy zero-shot promptingu:

1. Jasne, pojedyncze polecenie
2. Konkretne oczekiwania co do formatu
3. Precyzyjne określenie zakresu odpowiedzi
4. Brak zbędnego kontekstu
5. Bezpośrednie pytanie lub instrukcja

> ### Praktyczne wskazówki:
> - Używaj czasowników akcji (wymień, opisz, wyjaśnij)
> - Określaj konkretną liczbę elementów w odpowiedzi
> - Unikaj dwuznaczności
> - Zadawaj jedno pytanie na raz

### 💡 Przykład kompleksowego promptu:
```
Napisz przepis na świąteczne pierniki. Uwzględnij:
- Listę składników z dokładnymi proporcjami
- Czas przygotowania i pieczenia
- Kolejne kroki przygotowania
- Wskazówki dotyczące dekorowania
- Informację o czasie przechowywania
```

### 🎯 Najlepsze zastosowania:

- Proste klasyfikacje
- Podstawowe analizy tekstu
- Generowanie krótkich opisów
- Odpowiedzi na konkretne pytania
- Podstawowe zadania kreatywne
***
## 6) One-shot prompting - nauka na przykładzie

One-shot prompting to technika, w której pokazujemy modelowi jeden przykład tego, jakiej odpowiedzi oczekujemy. Jest to jak pokazanie wzoru, według którego model ma działać. Ta metoda jest szczególnie skuteczna, gdy chcemy otrzymać odpowiedź w konkretnym formacie lub stylu.

**Dlaczego one-shot prompting jest skuteczny?**

Modele LLM świetnie uczą się na przykładach. Pokazując jeden wzorcowy przykład, znacznie zwiększamy szansę na otrzymanie odpowiedzi w dokładnie takim formacie, jakiego oczekujemy.

### Przykłady złych vs. dobrych promptów:

<details>
  <summary>Przykład 1</summary>
  
❌ Źle: "Napisz życzenia świąteczne dla pracowników."

✅ Dobrze: 
"Napisz życzenia świąteczne dla pracowników w podobnym stylu do poniższego przykładu:

Przykład:
'Drodzy Współpracownicy,
Z okazji nadchodzących Świąt Bożego Narodzenia składam Wam serdeczne życzenia spokoju, radości i rodzinnego ciepła. Niech magiczna moc wigilijnego wieczoru przyniesie Wam spokój i odpoczynek, a Nowy Rok obdaruje pomyślnością i szczęściem.
Wesołych Świąt!
Dyrektor Jan Kowalski'

Teraz napisz życzenia od zespołu marketingu dla działu sprzedaży."
</details>

<details>
  <summary>Przykład 2</summary>
  
❌ Źle: "Napisz przepis na świąteczne ciasteczka."

✅ Dobrze:
"Napisz przepis na świąteczne ciasteczka według poniższego formatu:

Przykład:
🎄 PIERNICZKI ŚWIĄTECZNE
Czas przygotowania: 30 min
Składniki:
- 2 szklanki mąki
- 1/2 szklanki miodu
[...]
Przygotowanie:
1. W dużej misce wymieszaj...
2. Zagnieć ciasto...
Wskazówki:
- Przechowuj w szczelnym pojemniku
- Najlepiej smakują po 2-3 dniach

Teraz napisz przepis na maślane ciasteczka świąteczne zachowując dokładnie ten sam format."
</details>

### 👉 Kluczowe elementy one-shot promptingu:

1. Jasny przykład wzorcowy
2. Dokładne określenie elementów do zachowania
3. Wyraźne rozgraniczenie przykładu od nowego zadania
4. Zachowanie spójnej struktury

> ### Praktyczne wskazówki:
> - Wybieraj reprezentatywne przykłady
> - Zaznacz kluczowe elementy formatu
> - Używaj wyraźnych znaczników oddzielających przykład od zadania
> - Podkreśl, które elementy mają być zachowane

### 💡 Przykład kompleksowego promptu:
```
Zadanie: Napisz opisy produktów świątecznych według poniższego wzoru:

PRZYKŁAD:
🎁 Świąteczny Sweter "Rudolf"
Cena: 129,99 zł
Rozmiary: S, M, L, XL
Opis: Ciepły, świąteczny sweter z motywem renifera Rudolfa. Wykonany z miękkiej wełny merino, idealny na rodzinne spotkania przy choince.
Dostępne kolory: czerwony, zielony
Tags: #Christmas #WinterFash
```
***
## 7) Few-shot prompting - ucz model na przykładach

Few-shot prompting to technika, w której pokazujemy modelowi kilka przykładów tego, jak ma wykonać zadanie, zanim poprosimy go o właściwą odpowiedź. Jest to jak pokazanie Elfom w fabryce Świętego Mikołaja, jak dokładnie mają pakować prezenty, zanim zabiorą się do właściwej pracy.

**Dlaczego few-shot prompting jest skuteczny?**

Modele LLM uczą się przez analogię - pokazując im konkretne przykłady, znacznie zwiększamy szansę na otrzymanie odpowiedzi w dokładnie takim formacie i stylu, jakiego oczekujemy.

### Przykłady złych vs. dobrych promptów:

<details>
  <summary>Przykład 1</summary>
  
❌ Źle: "Napisz życzenia świąteczne w stylu haiku."

✅ Dobrze: 
"Napisz życzenia świąteczne w stylu haiku. Oto przykłady poprawnych haiku świątecznych:

Biały śnieg prószy
Choinka błyszczy w mroku
Święta już blisko

Dzwonki sań dźwięczą
Mikołaj mknie przez niebo
Prezenty niesie

Teraz napisz nowe, oryginalne haiku świąteczne w tym samym stylu."
</details>

<details>
  <summary>Przykład 2</summary>
  
❌ Źle: "Napisz przepis na świąteczne ciasteczka."

✅ Dobrze:
"Napisz przepis na świąteczne ciasteczka według poniższego formatu:

Przykład 1:
🍪 Pierniczki korzenne
Czas: 45 min
Składniki: mąka, miód, przyprawy
Kroki:
1. Wymieszaj składniki
2. Wyrób ciasto
3. Wałkuj i wycinaj
4. Piecz 15 min

Przykład 2:
🍪 Ciasteczka maślane
Czas: 30 min
Składniki: masło, cukier, mąka
Kroki:
1. Utrzyj masło
2. Dodaj pozostałe składniki
3. Formuj ciasteczka
4. Piecz 12 min

Teraz napisz przepis na swoje autorskie świąteczne ciasteczka w tym samym formacie."
</details>

### 👉 Kluczowe elementy few-shot promptingu:

1. Podanie 2-3 przykładów przed właściwym zadaniem
2. Zachowanie spójnego formatu we wszystkich przykładach
3. Użycie przykładów reprezentatywnych dla oczekiwanego rezultatu
4. Jasne oddzielenie przykładów od właściwego polecenia

> ### Praktyczne wskazówki:
> - Używaj przykładów o różnym poziomie złożoności
> - Pokazuj zarówno dobre, jak i złe przykłady
> - Zachowaj spójny format we wszystkich przykładach
> - Dodaj krótkie wyjaśnienie, dlaczego dane przykłady są dobre/złe

### 💡 Przykład kompleksowego promptu:
```
Zadanie: Napisz krótkie opowiadanie świąteczne według poniższego schematu.

Format przykładowy:

TYTUŁ: [zabawny tytuł]
BOHATER: [imię i krótki opis]
PROBLEM: [świąteczne wyzwanie]
ROZWIĄZANIE: [kreatywne rozwiązanie]
MORAŁ: [świąteczna nauka]

Przykład 1:
TYTUŁ: Renifer z katarem
BOHATER: Rudolf - renifer z czerwonym nosem
PROBLEM: Złapał katar w Wigilię
ROZWIĄZANIE: Inne renifery przyniosły mu ziołowy napar
MORAŁ: Przyjaźń pomaga pokonać każdą przeszkodę

Przykład 2:
TYTUŁ: Zgubiony prezent
BOHATER: Elf Tymek - najmłodszy pomocnik Mikołaja
PROBLEM: Zgubił ostatni prezent z sań
ROZWIĄZANIE: Użył magicznego dzwoneczka, by go odnaleźć
MORAŁ: Zawsze jest sposób, by naprawić błąd

Teraz napisz własne opowiadanie świąteczne według tego samego schematu."
```
### 🎯 Najlepsze praktyki few-shot promptingu:

1. **Stopniowanie trudności**
   - Zacznij od prostszych przykładów
   - Stopniowo wprowadzaj bardziej złożone przypadki

2. **Różnorodność przykładów**
   - Pokaż różne możliwe warianty
   - Uwzględnij edge cases

3. **Precyzja formatu**
   - Zachowaj identyczne formatowanie
   - Użyj tych samych elementów strukturalnych

4. **Kontekst**
   - Wyjaśnij, dlaczego przykłady są dobre
   - Podkreśl kluczowe elementy

Few-shot prompting to jak trenowanie nowych elfów w fabryce Świętego Mikołaja - im lepsze przykłady im pokażesz, tym lepiej będą wykonywać swoją pracę! 🎅🎁
***
## 8) Chain-of-Thought (CoT) - Myślenie krok po kroku

Chain-of-Thought to technika, która polega na prowadzeniu modelu przez proces rozumowania krok po kroku. Zamiast prosić o końcową odpowiedź, zachęcamy model do pokazania całego toku myślenia.

**Dlaczego CoT jest skuteczne?**

Prowadzenie modelu przez kolejne kroki rozumowania znacząco poprawia jakość i dokładność odpowiedzi, szczególnie w przypadku złożonych zadań wymagających logicznego myślenia.

### Przykłady złych vs. dobrych promptów:

<details>
  <summary>Przykład 1</summary>
  
❌ Źle: "Oblicz, ile Święty Mikołaj musi wydać na prezenty dla rodziny 5-osobowej, jeśli na każdą osobę chce przeznaczyć 200 zł, a dodatkowo musi kupić choinkę za 150 zł i ozdoby za 100 zł."

✅ Dobrze: 
"Rozwiążmy to zadanie krok po kroku:
1. Najpierw oblicz koszt prezentów dla rodziny:
   - Liczba osób: 5
   - Koszt na osobę: 200 zł
   - Oblicz: 5 × 200 zł
2. Następnie dodaj koszt choinki (150 zł)
3. Na końcu dodaj koszt ozdób (100 zł)
4. Zsumuj wszystkie koszty

Pokaż obliczenia dla każdego kroku."
</details>

<details>
  <summary>Przykład 2</summary>
  
❌ Źle: "Zaplanuj świąteczne przyjęcie dla 12 osób."

✅ Dobrze:
"Zaplanujmy świąteczne przyjęcie krok po kroku:
1. Najpierw określ budżet na osobę
2. Następnie zaplanuj menu:
   - Ile potraw głównych?
   - Jakie przystawki?
   - Jakie desery?
3. Potem oblicz ilość potrzebnych składników
4. Zaplanuj harmonogram przygotowań
5. Na końcu stwórz listę potrzebnego wyposażenia

Proszę o szczegółowe rozpisanie każdego z tych kroków."
</details>

### 👉 Kluczowe elementy Chain-of-Thought:

1. Rozbicie problemu na mniejsze części
2. Logiczna kolejność kroków
3. Jasne przejścia między etapami
4. Weryfikacja każdego kroku
5. Podsumowanie końcowych wniosków

> ### Praktyczne wskazówki:
> - Używaj numeracji dla kolejnych kroków
> - Zadawaj pytania kontrolne po każdym etapie
> - Proś o uzasadnienie każdego kroku
> - Zachęcaj do sprawdzania poprawności rozumowania

### 💡 Przykład kompleksowego promptu:
```
Pomóż mi zaplanować świąteczną zbiórkę charytatywną. Przeanalizujmy to krok po kroku:

1. Najpierw określmy cel zbiórki:
   - Dla kogo zbieramy?
   - Jakie są potrzeby?
   - Jaki jest cel kwotowy?

2. Następnie zaplanujmy logistykę:
   - Gdzie będzie się odbywać?
   - Kiedy?
   - Ilu wolontariuszy potrzebujemy?

3. Potem marketing:
   - Jakie kanały promocji wykorzystamy?
   - Jaki będzie przekaz?

4. Na końcu budżet:
   - Koszty organizacyjne
   - Przewidywane wpływy
   - Margines bezpieczeństwa

Proszę o szczegółowe rozpisanie każdego z tych elementów z uwzględnieniem realistycznych założeń i potencjalnych ryzyk.
```

### ⚡ Kiedy szczególnie warto stosować CoT:

- Przy rozwiązywaniu problemów matematycznych
- W zadaniach logicznych
- Przy planowaniu złożonych projektów
- W procesach decyzyjnych
- Przy analizie przypadków
***
## 9) Zero-Shot Chain-of-Thought (ZeroShotCoT)

Zero-Shot Chain-of-Thought to technika, która pozwala modelowi LLM na "myślenie na głos" bez wcześniejszego treningu na podobnych przykładach. Polega na dodaniu do promptu frazy "Pomyślmy o tym krok po kroku" (ang. "Let's think step by step") lub podobnej, co zachęca model do pokazania procesu rozumowania. Nie ma już potrzeby podawania konkretnych przykładów. Jest to metoda dużo szybsza niż pełny CoT, a często równie skuteczna.

**Dlaczego ZeroShotCoT jest skuteczne?**

Ta metoda znacząco poprawia jakość odpowiedzi, szczególnie w zadaniach wymagających logicznego myślenia, rozwiązywania problemów matematycznych czy analizy złożonych scenariuszy.

### Przykłady złych vs. dobrych promptów:

<details>
  <summary>Przykład 1</summary>
  
❌ Źle: "Ile prezentów może dostarczyć Święty Mikołaj w ciągu jednej nocy, jeśli spędza 2 sekundy w każdym domu i odwiedza 1000 domów?"

✅ Dobrze: "Ile prezentów może dostarczyć Święty Mikołaj w ciągu jednej nocy, jeśli spędza 2 sekundy w każdym domu i odwiedza 1000 domów? Pomyślmy o tym krok po kroku:
</details>

<details>
  <summary>Przykład 2</summary>
  
❌ Źle: "Czy opłaca się kupić sztuczną choinkę zamiast żywej?"

✅ Dobrze: "Przeanalizujmy krok po kroku, czy opłaca się kupić sztuczną choinkę zamiast żywej.
</details>

### 💡 Przykład kompleksowego promptu:
```
Pytanie: Jak zaplanować idealne przyjęcie świąteczne dla 12 osób, mając budżet 1000 zł?

Pomyślmy o tym krok po kroku. Proszę o szczegółowe przeanalizowanie każdego kroku.
```
***

I to są moim zdaniem najważniejsze i najbardziej przydatne techniki promptowania dużych modeli językowych. Oczywiście takich metod jest więcej, zachęcam Cię do zgłębiania wiedzy w tym temacie. W internecie na pewno znajdziesz mnóstwo materiałów.

**Dziękuję Ci i powodzenia!**

W razie pytań pisz smiało na kontakt@piotrkalinowski.cloud

Piotr Kalinowski
