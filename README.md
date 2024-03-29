# Proiect-Practic-Testare-Manuala

Scopul proiectului final pentru cursul de testare manuală ITF este de a folosi toate cunoștințele acumulate de-a lungul cursului și de a le aplica în practică, folosind o aplicație live.

Website în curs de testare: https://www.amaratour.ro/

Documentația API: https://www.amaratour.ro/amaratour-api-doc/

**Proiectul final va fi împărțit în 2 secțiuni: [Secțiunea de testare](https://github.com/iulia6/Proiect-Practic-Testare-Manuala/blob/main/README.md#1-sec%C8%9Biunea-de-testare) și [Secțiunea SQL](https://github.com/iulia6/itf_manual_testing_final_project_template/blob/main/Final%20Project/SQL).**

Instrumente folosite: JIRA, Zephyr Squad, MySQL Workbench.

# Specificații funcționale

Povestea de mai jos a fost creată în JIRA și descrie specificațiile funcționale ale modulului Clienti, pentru care se realizează proiectul final.

![imagine](https://github.com/iulia6/Proiect-Practic-Testare-Manuala/blob/main/story1.JPG)


# 1 Secțiunea de testare

## 1.1 Planificarea testelor

Planul de testare este conceput pentru a descrie toate detaliile testării pentru modulul Dependenți din websiteul Amara Tour.

Planul identifică elementele de testat, caracteristicile care trebuie testate, tipurile de testare care trebuie efectuate, personalul responsabil de testare, resursele și programul necesar pentru finalizarea testării și riscurile asociate cu planul.

#### 1.1.1 Rolurile atribuite proiectului și persoanele alocate

* Manager de proiect - Ormenisan Vlad
* Product owner - Florea Ioana
* Dezvoltator software - Vasiu Tudor
* Inginer QA - Negru Silvia

#### 1.1.2 Criteriile de intrare definite

* sunt definite specificatiile functionale
* sunt alocate rolurile necesare pentru proiect
* au fost detectate și atenuate riscurile inițiale ale proiectului

#### 1.1.3 Criteriile de ieșire definite

* numărul de erori nerezolvate este nesemnificativ sau au prioritate scăzută
* toate testele au fost executate
* toate erorile rezolvate au fost re-testate și aprobate de echipa QA
* termenul limită a fost atins
* niciun risc major detectat nu a rămas neatenuat

#### 1.1.4 Domeniul testului

* __Teste în domeniu:__ Toate caracteristicile crearii unui cont care au fost definite în specificațiile cerințelor software trebuie testate: testare funcțională, testare GUI și testare API
* __Teste care nu intră în domeniul de aplicare:__ testare de performanță, integrări ale modulului de dependență cu alte module, testare de compatibilitate cu mai multe browsere

#### 1.1.5 Riscuri detectate

* Riscuri ale proiectului: lipsa de experiență a echipei QA, schimbari neprevazute de cerinte, concurenta si evolutia tehnologiei
* Riscuri de produs: performanta, securitatea datelor, suport tehnic din partea echipei care a creat websiteul si se ocupa de mentenanta acestuia

#### 1.1.6 Evaluarea criteriilor de intrare

Criteriile de intrare definite în faza de planificare a testelor au fost atinse și procesul de testare poate continua.

## 1.2 Monitorizare și control de testare

Au fost generate diverse rapoarte periodice pentru a reflecta stadiul actual al procesului de testare, în cazul unor probleme majore s-ar putea lua măsuri de control.
Următorul raport de stare a fost generat după ce 40% din cazurile de testare au fost executate, la 14 august 2023:

![imagine](https://github.com/iulia6/Proiect-Practic-Testare-Manuala/blob/main/Zephyr%20test%20metrics.JPG)


## 1.3 Analiza testului

Procesul de testare va fi executat pe baza cerințelor de mai sus pentru modulul Clienti. Au fost găsite următoarele condiții de testare:
  * Verify if a user can create a new account on www.amaratour.ro website
  * Verify if a user can login into his account on www.amaratour.ro website
  * Verify if a user can change the password of his account created on www.amaratour.ro website
  * Verify if a user can log out from his account created on www.amaratour.ro website
  * Verify the "Parola pierduta?" function on www.amaratour.ro website
  * Verify if a user can filter the touristic package search by number hotel of stars
  * Verify if a user can filter the touristic package search by hotel's name
  * Verify if a user can sort the touristic packages selection by price
  * Verify if an user can book a touristic package on www.amaratour.ro website
  * Verify if an user can download the documents from a successfully booked touristic package on www.amaratour.ro website
  * Verify if a user can sort the touristic packages selection by Denumire (Z-A)

## 1.4 Testare de proiectare

Cazurile de testare funcționale au fost create în Zephyr Squad. Pe baza analizei specificațiilor, tehnicile de proiectare a testelor utilizate pentru generarea cazurilor de testare
sunt analiza valorii limită, partiționarea echivalenței și testarea cazurilor de utilizare.

**Cazuri de testare:**

![imagine](https://github.com/iulia6/Proiect-Practic-Testare-Manuala/blob/main/Test%20case%20raport.JPG)


Cazurile de testare cu pași pot fi vizualizate aici: [Create_account_test_cases.pdf](https://github.com/iulia6/Proiect-Practic-Testare-Manuala/blob/main/IS-17.pdf)

Pentru API-ul Dependents, a fost generată următoarea listă de verificare: [API_test_checklist.csv](https://github.com/julai215/itf_final_project_example_and_portofolio/blob/main/Final%20Project/API_test_checklist.csv)


## 1.5 Implementarea testului

Următoarele elemente sunt necesare pentru a fi pregătite înainte de începerea fazei de execuție a testului:

* Mediul de testare este activ și rulează: https://www.amaratour.ro/
* Accesul la mediul de testare este dat: Nume utilizator : pavel.m87@yahoo.com | Parola: super87
* Cycle summaryul a fost creat
* Cazurile de testare au fost adăugate la rezumatul ciclului
* A fost creată colecția Postman cu metodele API dependente
* Tokenul de autorizare a fost creat pentru accesarea API-ului

## 1.6 Execuția testului

* Cazurile de testare sunt executate pe rezumatul ciclului de testare creat: [Creares_cont_summary_execution.pdf](https://github.com/iulia6/Proiect-Practic-Testare-Manuala/blob/main/Cycle%20summary.csv)
* Bug-urile au fost create pe baza testelor eșuate. Rapoartele complete ale erorilor pot fi găsite aici: [Creare_cont_bugs.pdf](https://github.com/iulia6/Proiect-Practic-Testare-Manuala/blob/main/Bug%20report.JPG)
     * Formatul datei nu este zz/ll/aaaa
     * „Data nașterii” viitoare poate fi selectată din calendar
     * Sunt permise doar 50 de caractere pentru câmpul „Vă rugăm să specificați”.
     * Numai 50 de caractere sunt permise pentru câmpul „Nume”.
* Testele API sunt executate pe baza listei de verificare. Colecția folosită poate fi găsită aici: [Fișier JSON cu colecția de solicitări creată pentru API-ul Creare_cont](https://github.com/julai215/itf_final_project_example_and_portofolio/blob/main/Final%20Project/OrangeHRM%20API%20-% 20Dependents.postman_collection.json)
* Testarea completă a regresiei este necesară după ce erorile sunt remediate

## 1.7 Finalizarea testului

* Deoarece criteriile de ieșire au fost îndeplinite și satisfăcute așa cum se menționează în secțiunea corespunzătoare, echipa de testare sugerează această funcție să fie lansata
* Matricea de trasabilitate a fost generată și poate fi găsită aici: [Traceability_matrix.csv](https://github.com/iulia6/Proiect-Practic-Testare-Manuala/blob/main/Matricea%20trasabilitatii.JPG)
* A fost generată diagrama de execuție a testelor, raportul final arată că un număr de 5 teste au eșuat din total 23
* Un număr de 11 de cazuri de testare au fost planificate pentru execuție și toate au fost executate
* S-au găsit un număr de 2 erori în total, dintre care prioritatea este: 1 este medie și 1 este scăzută

![imagine](https://github.com/iulia6/Proiect-Practic-Testare-Manuala/blob/main/Test%20Execution%20Chart.JPG)


# 2 Secțiunea SQL

A creat o bază de date numită „amaratour” și un tabel numit „clienti” cu toate coloanele necesare pentru a salva datele conform specificațiilor. Au efectuat diferite interogări în interiorul fișierului sql: [clienti.sql](https://github.com/iulia6/itf_manual_testing_final_project_template/blob/main/Final%20Project/SQL)
