# Proiect_stive_AI

Mutarea blocurilor se face cu urmatoarele restrictii:

Putem muta un bloc b1 peste alt bloc b2 doar dacă numerele din cele două blocuri sunt prime între ele (de exemplu nu pot muta 15 peste 6 (fiindcă cel mai mare divizor comun al lor este 3), dar îl pot muta peste 14 (deoarece cmmdc-ul numerelor 15 și 14 este 1 deci sunt prime între ele)
nu putem muta un bloc pe o stivă dacă pe același nivel, pe stivele din stânga și dreapta avem deja un bloc cu aceeași valoare
Costul mutarii este egal cu numărul de divizori pe care îl are numărul din blocul mutat.

Nu este necesar ca starea inițială să respecte condițiile de mutare (de exemplu în starea inițială pot să am blocuri cu numere neprime între ele unele peste altele), doar la mutări se vor aplica acele condiții.

Fisierul de intrare va conține starea inițială (stivele cu blocurile). O stare în fișierul de input se va reprezenta astfel:
- fiecare stivă pe câte un rând. Se consideră că baza stivei e la stânga și vârful stivei e la dreapta.
- blocurile de pe o stivă se vor separa cu simbolul ";" (punct si virgulă)
- informația dintr-un bloc va fi numărul corespunzător
- Stivele vide se evidențiază prin "~"
Sub starea inițială se va găsi un separator "-----" și un rănd cu un număr N de numere, unde N reprezintă numărul de stive. Suma numerelor de pe acel rand trebuie să fie egală cu numărul de blocuri. Se va verifica dacă fișierul de intrare e corect.

O stare e considerata scop daca pentru orice stiva (având indicele i) e adevarat ca înălțimea ei este egala cu numărul cu indicele i din șirul de numere de la finalul fișierului de intrare. Practic acel șir de numere specifică înălțimea dorită pentru fiecare stivă în parte, indiferent de blocurile existente.

Deci pot fi mai multe stari finale posibile pentru aceeasi configuratie initiala si testarea atingerii scopului trebuie facuta prin verificarea conditiei, NU prin enumerarea posibilitatilor de nod scop.


Exemplu de stare initială:

![Screenshot 2023-02-27 134902](https://user-images.githubusercontent.com/82332641/221556225-5ff6cefb-de2c-4921-95ae-c06b6d704c79.png)

Și dorim sa o aducem în starea "5 5 0 1", adică prima stivă să aiba lungimea de 5 blocuri, a 2 a tot de 5 blocuri, a 3 a 0, iar ultima să aibă doar un bloc.

Exemplu stare scop/finală:

![Screenshot 2023-02-27 134902](https://user-images.githubusercontent.com/82332641/221557594-edbb243e-2660-494b-8a91-ad59b07b44d3.png)
