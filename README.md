## Projecte-llenguatge-de-marques

#**Explicació**

**GENERAL**

Aquest projecte té com a temàtica el videojoc *VALORANT*. Aquest és un 5vs5 que consisteix en dos bàndols, un que ataca i un altre que defensa. El bàndol que ataca ha de plantar una bomba en un *site*, una zona especial, i els defensors han d'evitar-ho o, en el pitjor dels casos, desactivar la bomba. Pel que fa al treball, he decidit incloure 4 personatges i 4 mapes, aques están relacionats degut a que cada mapa te unes característiques diferents que va que alguns personatges siguen millors que altres. Cada personatge compta amb el nom que te el personatge al videojoc en format **ATTLIST**, data en què va entrar al joc en format **ATTLIST**, tipus de personatge (el rol principal dins del joc) que por variar en 4 diferents en format **ATTLIST**, les seves habilitats (depenent del personatge pot tindre diferents) y habilitat final amb una explicació de l’*habilitat final* (també coneguda com a *ulti*) en format **ATTLIST**, foto del personatge (link a l'imatge de *GOOGLE*) i una breu descripció del persontage treta de la página oficial del joc. Pel que fa als mapes, he posat el nom d'aquest, foto (link a l'imatge de *GOOGLE*), data en què van entrar al joc en format **ATTLIST**, millor personatge per a aquest mapa en format **ATTLIST** i una breu descripció extreta de la pàgina oficial del joc. 

**DTD**

El DTD es la base d'aquest projecte, de manera que ha d'estar ven format per a poder aaugmentar el tamny del XML en cualsevol moment. Primer de tot vaig definir el element principal, VALORANT que conté agents (el personatges del joc) i els mapes. Dins de agents tenim els **ATTLIST** nom, data d'entrada al joc i tipus del persontage (duelista, centinela, controladors, iniciadors) i els elements habilitats, foto y descripció. Dins de habilitats tenims en **ATTLIST** habilitats1-3 i habilitat final juntament amd la descripció de l'habilitat final que es única per a cada personatge. En la part de mapes tenim **ATTLIST** la data d'entrada al joc i el millor agent per a aquest mapa (degut a que en aquest projecte nomes parlem de 4 personatge he posat que nomes es pugen posar eixos 4, en cas d'una expansió on posarem mes personatges deuriem ampliarlo també en aquest DTD perque no donara error) i els elements nom foto y descripció. Tots els elements son necesaris de coneixer per lo que no tenim ningun **EMPTY** ni ningun defint amb un **?**. En el cas de les habilitats normals del personatges están definides de maneraa que ha de ser una de les que apareixen a cada una de les habilitats 1, 2 o 3. En el cas de l'habilitat final al ser exclusiva de cada personatge no necesitem especificar alguna ja que tenen noms diferents. 

#**Procediment**

Una vegada decidit el tema del projecte, vaig començar plantejant quina informació podia mostrar del joc a més d’aquesta. Després de pensar-ho, vaig decidir que els personatges i els mapes eren el més fàcil per al projecte, ja que tenien característiques fàcils d'incloure. Una vegada tot plantejat, vaig començar amb el DTD per donar-li el format correcte al treball. Finalment, amb el DTD acabat, vaig començar amb l’XML. Per últim, vaig decidir quins personatges i mapes volia mostrar en l’XML. En el cas dels personatges, vaig elegir-ne un de cada tipus diferent per mostrar característiques variades a l’XML.
