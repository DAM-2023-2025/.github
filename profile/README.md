# Repositori de l'Organització DAM-2023-2025

## Repositori de l'Organització **```DAM-20233-2025```**

<details><summary>Desplega per veure les hores del cicle</summary>

## Curs 1r de DAM

|Mòduls professionals|Hores|
|----|----:|
|MP01 - Sistemes informàtics|121|
|MP02 - Bases de dades|110|
|MP03 - Programació|187|
|MP04 - Llenguatges de marques i sistemes de gestió d’informació|77|
|MP05 - Entorns de desenvolupament|55|
|MP06 - Accés a dades|88|
|MP11 - Formació i orientació laboral|66|
|MP12 - Empresa i iniciativa emprenedora|66|
|MP15 - Game design|33|
|MP16 - Disseny 2D i 3D|88|
|**Total primer curs**|**891**|

## Curs 2n de DAM
|Mòduls professionals|Hores|
|----|----:|
|MP07. Desenvolupament d’interfícies|88|
|MP08. Programació multimèdia i dispositius mòbils|77|
|MP09. Programació de serveis i processos|55|
|MP10. Sistemes de gestió empresarial|55|
|MP13. Projecte|297|
|MP17. Programació de videojocs 2D i 3D|154|
|MP14. Formació en centres de treball|383|
|**Total segon curs**|**1109**|

## Cicle de DAM

|Curs|Hores|
|----|----:|
|Total primer curs|891|
|Total segon curs|1109|
|**Total cicle**|**2000**|

</details>


### Primer curs (2023-2024) - DAM1

## MP05: **Entorns de desenvolupament**

<hr>

### MP05 - ***UF01***: Desenvolupament de programari

## A01U - Activitat 1: Servidor i contenidor nginx (part servidor)

**1.**  Crea un **repositori local** **```<Cognom>-docker-nginx```**
**2.**  Crea un **repositori remot** **```<Cognom>-docker-nginx```**
**2.1.**  Tipus **privat**
**2.2.**  convida usuari **```joanpardogine```**
**3.**  Modifica el fitxer **```README.md```** perquè aparegui una explicació detallada de tots els passos que heu fet per instal·lar el servidor web amb ***```NGINX```*** en un **servidor ```ubuntu```**.

De cada pas cal que aparegui:
    * la comanda feta i
    * una explicació detallada de què fa la comanda.

**4.**  el servidor cal que mostri una pàgina web que hàgiu fet de qualsevol altre mòdul.


## A02U - Activitat 2: Servidor amb nginx i php (part php)

**1.** Modifica el fitxer **README.md** perquè aparegui una explicació detallada de tots els passos que heu fet per instal·lar el servidor web PHP al servidor que ja tens amb NGINX funcionant.

**2.** Un cop que el servidor d'nginx ja tingui instal·lat PHP, crea a la carpeta corresponent el fitxer index.php, amb el següent contingut:

```php
<?php
    phpinfo();
?>
```

**3.** Obre el navegador i mostra **```<ipDelSerbvidor>/index.php```**

**4.** Afegeix al **```README.md```** una imatge del navegador mostrant el resultat d'accedir a l'adreça <ipDelSerbvidor>/index.php

## A03U - Activitat 3: Servidor amb mariadb (part base de dades)

Cal instal·lar en un nou servidor amb ubuntu el sistema gestor de bases de dades mariadb.

**1.** Modifica el fitxer **README.md** perquè aparegui una explicació detallada de tots els passos que heu fet per instal·lar en el nou servidor de base de dades, mariadb.

**2.** Connectat a mariadb i crea la següent base de dades:

```sql
CREATE DATABASE ctrlUsuaris;

USE ctrlUsuaris;

CREATE TABLE usuaris (
idUsuari INT AUTO_INCREMENT PRIMARY KEY,
nomUsuari VARCHAR(50),
correuUsuari VARCHAR(100)
);

INSERT INTO usuaris (nomUsuari, correuUsuari) VALUES
('Pere', 'pere@exemple.com'),
('Anna', 'anna@exemple.com'),
('Carles', 'carles@example.com'),
('David', 'david@exemple.com');
```

**3.** Afegeix al **```README.md```** una imatge de la resposta que torna mariadb en executar la següent comanda:

```sql
SELECT * FROM usuaris;
```



## A04U - Activitat 4: Crear web amb php i accés a les dades del servidor de mariadb (part comunicació entre servidors)

Cal crear en el servidor a on teniu l'**nginx** i el **PHP**, un programa (**```llistat_usuaris.php```**) fet amb **PHP** que es connecti a la base de dades **```ctrlUsuaris```** que es troba al sistema gestor de bases de dades **```mariadb```**.
El programa (**```llistat_usuaris.php```**) fet amb **PHP** cal que mostri una taula amb tota la informació de la taula **```usuaris```**.

**1.** Modifica el fitxer **README.md** perquè aparegui una explicació detallada de **TOTS** els passos que heu fet assolir el que es demana a l'activitat.

**2.** En el fitxer **README.md** cal que aparegui el contingut del fitxer **```llistat_usuaris.php```**, amb format **, que heu fet servir.

**3.** Afegeix també al **README.md** una imatge de l'execució del programa **```llistat_usuaris.php```**, a on vegi tota la informació de la taula **```usuaris```** en format taula.


## A05U - Activitat 5: Modificació de literals del PHP i dades de la base de dades

[dam1-mp05-uf01-a05u](https://github.com/DAM-2023-2025/dam1-mp05-uf01-a05u.git)

<hr>

[**00-pseudocodi**](https://github.com/DAM-2023-2025/00-pseudocodi)