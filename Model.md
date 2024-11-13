### Projecte-llenguatge-de-marques

![image](https://github.com/user-attachments/assets/99d381ad-8432-4fae-b82a-fab236129e02)


# **Explicació**

**GENERAL**

Aquest projecte té com a temàtica el videojoc *VALORANT*. Aquest és un 5vs5 que consisteix en dos bàndols: un que ataca i un altre que defensa. El bàndol que ataca ha de plantar una bomba en un *site*, una zona especial, i els defensors han d'evitar-ho o, en el pitjor dels casos, desactivar la bomba. Pel que fa al treball, he decidit incloure 4 personatges i 4 mapes, que estan relacionats perquè cada mapa té unes característiques diferents que fan que alguns personatges siguin millors que altres. Cada personatge compta amb el nom que té el personatge al videojoc en format **ATTLIST**, la data en què va entrar al joc en format **ATTLIST**, el tipus de personatge (el rol principal dins del joc), que pot variar en 4 tipus diferents en format **ATTLIST**, les seves habilitats (depenent del personatge pot tenir diferents) i l'habilitat final, amb una explicació de l’*habilitat final* (també coneguda com a *ulti*) en format **ATTLIST**, foto del personatge (enllaç a la imatge de *GOOGLE*) i una breu descripció del personatge extreta de la pàgina oficial del joc. Pel que fa als mapes, he posat el nom, la foto (enllaç a la imatge de *GOOGLE*), la data en què van entrar al joc en format **ATTLIST**, el millor personatge per a aquest mapa en format **ATTLIST** i una breu descripció extreta de la pàgina oficial del joc. 

**DTD**

El DTD és la base d'aquest projecte, de manera que ha d'estar ben format per a poder augmentar la mida de l'XML en qualsevol moment. Primer de tot, vaig definir l'element principal, VALORANT, que conté agents (els personatges del joc) i els mapes. Dins de agents tenim els **ATTLIST** nom, data d'entrada al joc i tipus del personatge (duelista, centinela, controlador, iniciador) i els elements habilitats, foto i descripció. Dins d'habilitats tenim en **ATTLIST** habilitats1-3 i habilitat final, juntament amb la descripció de l'habilitat final, que és única per a cada personatge. En la part de mapes tenim **ATTLIST** la data d'entrada al joc i el millor agent per a aquest mapa (ja que en aquest projecte només parlem de 4 personatges, he posat que només es poden posar aquests 4; en cas d'una expansió on incloguéssim més personatges, hauríem d'ampliar-ho també en aquest DTD per tal que no doni error) i els elements nom, foto i descripció. Tots els elements són necessaris de conèixer, per la qual cosa no tenim cap **EMPTY** ni cap definit amb un **?**. En el cas de les habilitats normals dels personatges, estan definides de manera que ha de ser una de les que apareixen en cadascuna de les habilitats 1, 2 o 3. En el cas de l'habilitat final, com que és exclusiva de cada personatge, no cal especificar-ne cap, ja que tenen noms diferents.

# **Procediment**

Una vegada decidit el tema del projecte, vaig començar plantejant quina informació podia mostrar del joc, a més d’aquesta. Després de pensar-ho, vaig decidir que els personatges i els mapes eren els més fàcils per al projecte, ja que tenien característiques fàcils d'incloure. Una vegada tot plantejat, vaig començar amb el DTD per donar-li el format correcte al treball. Finalment, amb el DTD acabat, vaig començar amb l’XML. Per últim, vaig decidir quins personatges i mapes volia mostrar en l’XML. En el cas dels personatges, vaig elegir-ne un de cada tipus diferent per mostrar característiques variades a l’XML.

![image](https://github.com/user-attachments/assets/b9be6cb8-85c6-4516-8400-eacb088b9c39)
