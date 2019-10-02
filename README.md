# Cours-SAS

<!-- TOC -->

- [**TD1**](#td1)
  - [Les tables SAS](#les-tables-sas)
  - [la librairie SAS](#la-librairie-sas)
  - [Quelques `libname` utiles](#quelques-libname-utiles)
    - [la `work`](#la-work)

<!-- /TOC -->

---
#  **TD1**

## Les tables SAS

Il s'agit d'un tableau contenant les données. Les colonnes sont appelées des `variables` et les lignes des `observations`.

| observation | var1  | var2  |
|---          |---    |---    |
|1            |toto   |12     |
|2            |tata   |13     |
|3            |tutu   |14     |

## la librairie SAS

Elle sert à stocker les `tables` SAS que nous allons manipuler.
Il faut lui indiquer à quel endroit celles-ci le seront.

- Elle contient :
  - un `nom` : pas plus de **8 caractères**, chiffres et lettres mais doit commencer par une lettre.
  - un `chemin` d'accès au dossier

```sas
libname nom "chemin";
```

Voici un exemple d'utilisation d'une `librairie` que nous nommerons **td1**.
Celle ci stockera les tables dans le dossier **memo** situé sur le lecteur **E:**.

```sas
libname td1 "E:\memo";
```

## Quelques `libname` utiles

### la `work`

Par défaut, si l'utilisateur ne précise rien les tables sont stockées dans la librairie `work`. Celle-ci ne conserve les tables que pour la durée de la session.

### la `sashelp`

Moins utile que la précèdente, elle contient un certain nombre de `tables` chargées par défaut. Celles-ci sont utile pour la documentation de **SAS**.
