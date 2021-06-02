denik 6
=======

`Zpet na obsah <https://bravo-cizek.github.io/>`_

Opakovani
---------

- program je spustitelny soubor, na win pripona .exe, na unixech bez pripony. Stavaji se spustitelnymi pomoci ``chmod + x``
- program se sklada z jedne nebo dvou funkci, podle toho jak je napsany a zaroven podle op
- strcmp = string compare

1.  kompilace programu zahrnuje
  

    a) assembly, assembler
    b) kompilaci
    c) linkovani
 

- priklad ::

                cc- o csgo.exe csgo.c
                object file -c flag
- kompilator si musi overit zahlavi, zahlavi = prototyp
- protoyp se dodava pomoci hlavicky ``include``
- narocne na pamet,procesor a cas.


MakeFile
--------

- csgo.exe zavisi na: ``main.o\str.o\net.o``
- pokud je hlavicka (include) zavisi i na nich.

- GUID = globaly unique identifier. GUID = UUID


Eviron - user environment
-------------------------

- je deklarovany v ``<unistd.h>``

- Eviron je zacinajici prostredi v shellu, je ulozeny "osidleny" v ruznych cestach.
- jako definice z ``etc/env`` ktere jsou spousteny z ``pam_env`` pro vsechny uzivatele v log timeu.

- argumenty mohou byt vlozeny do env v pripade pouziti ``exec`` 

- c  program muze manipulovat se svym prostredim pouzitim funkci: ::

                                                                        - getenv
                                                                        - putenv
                                                                        - setenv
                                                                        - unsetenv


tmpdir
------

- ovlivnuje cesty prefixu jmen vytvorenych ``tempnam`` a ``tempdiru`` vyuzivanych Sort programem a jinymi.

- posix definuje rozhrani na unixech, aby byli programy ``prenositelne`` na ruzne HW.


Ruzne vysvetlivky
-----------------

- WildCard umoznuje zapsat jednim vyrazem vetsi mnozstvi retezcu, napr. jmen souboru atd.

- Find umoznuje prohledavani adresaru nebo souboru, prikaz umoznuje urcit vlastnosti hledaneho objektu (napr. velikost, cast nazvu, atd.)
- syntaxe findu ::

                   find {cesta} {hledany vyraz} {co s tim ma delat}
- priklad kdy find najde vsechny .txt soubory, ktere jsou starsi nez osm dnu ::

                find {cesta} - type f -name *.txt -mtime +8

- promenna pro vsechny argumenty ``$@``
- ``DWP`` v prikazove radce prohodi znaky
- ``ctrl xl`` nabidka pouzitych vyrazu >> ``ctrl j`` nabidku potvrdi

