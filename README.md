# Gravstensinventeringen-Wikidata
Status: **slowly moving forward**

Se hur vi kan kan koppla ihop [Wikidata](https://www.youtube.com/watch?v=m_9_23jXPoE) och [Gravstensinventeringen](https://www.rotter.se/gsi/begravningsplatser) bättre - mer på [Wikidata project](https://www.wikidata.org/wiki/Wikidata:WikiProject_Gravstensinventeringen)

Svenska Släktforskarförbundet har byggt om sin [gravinventeringar](https://www.rotter.se/gsi/begravningsplatser) så tanken ör att koppla ihop alla Sveriges begravningsplatser med Wikidata

Idag finns egenskap [Property:P5259](https://www.wikidata.org/wiki/Property:P5259) i Wikidata med ung, <del>500</del>4500 poster kopplade 
* [video](https://www.youtube.com/watch?v=hNaK1iNSvhE)
* SPARQL [andra WD egenskaper där P5259 finns](https://w.wiki/5xGr) / [enbart externa](https://w.wiki/5xGo)
* Karta gravar / [kyrkogårdar](https://w.wiki/5xJd)
  * karta [FindAGrave och Gravstensinventeringen](https://w.wiki/5xKc) > 920/ [alla FindAgrave begravningsplatser i WD](https://w.wiki/5xQt) > 12000
    * karta [FindAgrave med länk karta FindaGrave MAP](https://w.wiki/6ioK) ex. [Norra Begravningsplatsen](https://www.findagrave.com/cemetery/1972857/map)

<img width="1339" alt="image" src="https://github.com/salgo60/Gravstensinventeringen-Wikidata/assets/14206509/dbe23923-404c-4a25-bb3b-d11b6a19dcbf">


  * karta WD objekt kyrkogårdar med [P8592 Flygfoto WIP](https://w.wiki/5zqo)
     * karta [WD kyrkor ej kopplade med P8592 Flygfoto](https://w.wiki/5zzY)
  * karta [WD objekt utan OSM](https://w.wiki/5ztV) / [med](https://w.wiki/68x$)
 * [Kyrkogårdar kopplade till en kyrka i Wikidata med en svensk Wikipedia sida](https://w.wiki/6QFa) / [ej kopplade]([sss](https://w.wiki/6QFg))
 * [Wikishootme vilka kyrkogårdar som saknar bilder](https://wikishootme.toolforge.org/#lat=59.32108734509658&lng=18.027788288891315&zoom=10&layers=wikidata_image,wikidata_no_image&sparql_filter=%3Fq%20wdt%3AP6104%20wd%3AQ115206846&worldwide=1)

[<img width="1203" alt="image" src="https://user-images.githubusercontent.com/14206509/205506865-899cdfd4-7bb7-49bb-9e90-b9f3ce930442.png">](https://wikishootme.toolforge.org/#lat=59.32108734509658&lng=18.027788288891315&zoom=10&layers=wikidata_image,wikidata_no_image&sparql_filter=%3Fq%20wdt%3AP6104%20wd%3AQ115206846&worldwide=1)


* [Video](https://youtu.be/QPpYAFSgJ3g) hur Wikidata kopplar ihop Wikipedia och bilder på gravar
* [Larske SPARQL](https://w.wiki/64xt) att hitta dubletter
* [Begravningsplatser kopplade till FindAGrave](https://w.wiki/66bE)


[<img width="1386" alt="image" src="https://user-images.githubusercontent.com/14206509/202914138-bed57998-6068-4424-b054-8298229dcb94.png">](https://w.wiki/5xGo)

[<img width="542" alt="image" src="https://user-images.githubusercontent.com/14206509/202914273-1245a118-88c0-4cf1-9855-cf378f903ccb.png">](https://w.wiki/5xJd)

[<img width="636" alt="image" src="https://user-images.githubusercontent.com/14206509/202914538-df40e166-6980-4d87-a138-3b20b3f966be.png">](https://w.wiki/5zqo)
### Fel funna i Gravstensinventeringen
* [Koordinat fel](https://github.com/salgo60/Gravstensinventeringen-Wikidata/issues?q=+label%3A%22fel+koordinat+gravstensinventeringen%22+)
  * [SPARQL](https://w.wiki/6RLa)
* [Kyrkogård som saknas i Svenska Gravstensinventeringen](https://w.wiki/5xuY)

## Gravar i Gravstensinventeringen kopplade till Wikidata
* [lista > 600 personer](https://w.wiki/6ojR)

## Gravar kopplas till person/koordinat i Wikidata 
Exempel
* [Gävle Gamla kyrkogård](http://minancestry.blogspot.com/2020/03/gavle.html)
* Norra Begravningsplatsen Q252312 [karta](https://query.wikidata.org/embed.html#%23title%3A%20Gravar%20%0A%23defaultView%3AMap%0ASELECT%20%3Fitem%20%3FitemLabel%20%3FitemDescription%20%3Fcoord%20%28SAMPLE%28%3FpicGrave%29%20as%20%3FpicGrave%29%20%28SAMPLE%28%3Fimg%29%20as%20%3Fimg%29%20%3Farticle%20%3FGeni%20%28SAMPLE%28%3Fgraveplot%29%20as%20%3Fgraveplot%29%20%0A%0A%09WHERE%20%7B%20%0A%20%09%09%09%09%09%3Fitem%20wdt%3AP119%20wd%3AQ252312%20.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%3Fitem%20p%3AP119%20%3FplaceofBurial%20.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP18%20%3Fimg%7D.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP569%20%3FbirthDate%7D.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3FplaceofBurial%20pq%3AP965%20%3Fgraveplot%7D%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3FplaceofBurial%20pq%3AP625%20%3Fcoord%7D%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP1442%20%3FpicGrave%20%7D%20%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP2600%20%3FGeniID%20%7D%0A%20%20%20%20OPTIONAL%20%7B%0A%20%20%20%20%20%20%3Farticle%20schema%3Aabout%20%3Fitem%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AinLanguage%20%22sv%22%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AisPartOf%20%3Chttps%3A%2F%2Fsv.wikipedia.org%2F%3E%20.%0A%20%20%20%20%7D%0A%20%20%20%20OPTIONAL%20%7B%0A%20%20%20%20%20%20%3Farticle%20schema%3Aabout%20%3Fitem%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AinLanguage%20%22en%22%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AisPartOf%20%3Chttps%3A%2F%2Fen.wikipedia.org%2F%3E%20.%0A%20%20%20%20%7D%0A%20%20%20%20BIND%20%28URI%28CONCAT%28%22https%3A%2F%2Fwww.geni.com%2Fpeople%2F%22%2C%3FGeniID%29%29%20AS%20%3FGeni%29%0A%20%20%0A%20%20%20%09OPTIONAL%20%7B%20%3Farticlerank%20schema%3Aabout%20%3Fitem.%20%7D%0A%20%20%20SERVICE%20wikibase%3Alabel%20%7B%20bd%3AserviceParam%20wikibase%3Alanguage%20%22sv%22%2C%22en%22.%20%7D%0A%7D%0AGROUP%20BY%20%3Fitem%20%3FitemLabel%20%3FitemDescription%20%3Fcoord%20%3Farticle%20%3FGeni%20%0AORDER%20BY%20DESC%28%3Frank%29%0A) / 
  * [Födelseplatser på personer](http://tinyurl.com/m2935bb) begravda på Norra Begravningsplatsen enl. Wikidata
  * Personer på [Norra Begravningsplatsen som har artikel > 10 språk](https://query.wikidata.org/embed.html#%23title%3A%20Gravar%20d%C3%A4r%20personen%20finns%20m%2Ced%20artikel%20%3E%2010%20spr%C3%A5k%0A%23defaultView%3AMap%0ASELECT%20%3Fitem%20%3FitemLabel%20%3FitemDescription%20%3Fcoord%20(SAMPLE(%3FpicGrave)%20as%20%3FpicGrave)%20(SAMPLE(%3Fimg)%20as%20%3Fimg)%20%3Farticle%20%3FGeni%20(SAMPLE(%3Fgraveplot)%20as%20%3Fgraveplot)%20%0A(COUNT(%3Fitem)%20AS%20%3Frank)%0A%09WHERE%20{%20%0A%20%09%09%09%09%09%3Fitem%20wdt%3AP119%20wd%3AQ252312%20.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%3Fitem%20p%3AP119%20%3FplaceofBurial%20.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20{%20%3Fitem%20wdt%3AP18%20%3Fimg}.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20{%20%3Fitem%20wdt%3AP569%20%3FbirthDate}.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20{%20%3FplaceofBurial%20pq%3AP965%20%3Fgraveplot}%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20{%20%3FplaceofBurial%20pq%3AP625%20%3Fcoord}%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20{%20%3Fitem%20wdt%3AP1442%20%3FpicGrave%20}%20%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20{%20%3Fitem%20wdt%3AP2600%20%3FGeniID%20}%0A%20%20%20%20OPTIONAL%20{%0A%20%20%20%20%20%20%3Farticle%20schema%3Aabout%20%3Fitem%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AinLanguage%20%22sv%22%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AisPartOf%20%3Chttps%3A%2F%2Fsv.wikipedia.org%2F%3E%20.%0A%20%20%20%20}%0A%20%20%20%20OPTIONAL%20{%0A%20%20%20%20%20%20%3Farticle%20schema%3Aabout%20%3Fitem%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AinLanguage%20%22en%22%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AisPartOf%20%3Chttps%3A%2F%2Fen.wikipedia.org%2F%3E%20.%0A%20%20%20%20}%0A%20%20%20%20BIND%20(URI(CONCAT(%22https%3A%2F%2Fwww.geni.com%2Fpeople%2F%22%2C%3FGeniID))%20AS%20%3FGeni)%0A%20%20%0A%20%20%20%09OPTIONAL%20{%20%3Farticlerank%20schema%3Aabout%20%3Fitem.%20}%0A%20%20%20SERVICE%20wikibase%3Alabel%20{%20bd%3AserviceParam%20wikibase%3Alanguage%20%22sv%22%2C%22en%22.%20}%0A}%0AGROUP%20BY%20%3Fitem%20%3FitemLabel%20%3FitemDescription%20%3Fcoord%20%3Farticle%20%3FGeni%20Having%20(%3Frank%20%3E%2010)%0AORDER%20BY%20DESC(%3Frank)%0A)
 * Skogskyrkogården Q213988 gravar med koordinat och artikel på sv:Wikipedia [karta = 182]([https://w.wiki/6okG](https://w.wiki/6okG)) / [karta personer utan bild på graven = 173](https://w.wiki/6okB](https://w.wiki/6okK) / [Lista saknar gravbild Skogskyrkogården](https://sv.wikipedia.org/wiki/Wikipedia:%C3%96nskem%C3%A5l_om_bilder/Sverige/Skogskyrkog%C3%A5rden) 
    * [Personer på Skogskyrkogården som har artikel > 5 språk](https://query.wikidata.org/embed.html#%23title%3A%20Gravar%20d%C3%A4r%20personen%20finns%20med%20artikel%20%3E%2010%20spr%C3%A5k%0A%23defaultView%3AMap%0ASELECT%20%3Fitem%20%3FitemLabel%20%3FitemDescription%20%3Fcoord%20%28SAMPLE%28%3FpicGrave%29%20as%20%3FpicGrave%29%20%28SAMPLE%28%3Fimg%29%20as%20%3Fimg%29%20%3Farticle%20%3FGeni%20%28SAMPLE%28%3Fgraveplot%29%20as%20%3Fgraveplot%29%20%0A%28COUNT%28%3Fitem%29%20AS%20%3Frank%29%0A%09WHERE%20%7B%20%0A%20%09%09%09%09%09%3Fitem%20wdt%3AP119%20wd%3AQ213988%20.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%3Fitem%20p%3AP119%20%3FplaceofBurial%20.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP18%20%3Fimg%7D.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP569%20%3FbirthDate%7D.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3FplaceofBurial%20pq%3AP965%20%3Fgraveplot%7D%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3FplaceofBurial%20pq%3AP625%20%3Fcoord%7D%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP1442%20%3FpicGrave%20%7D%20%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP2600%20%3FGeniID%20%7D%0A%20%20%20%20OPTIONAL%20%7B%0A%20%20%20%20%20%20%3Farticle%20schema%3Aabout%20%3Fitem%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AinLanguage%20%22sv%22%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AisPartOf%20%3Chttps%3A%2F%2Fsv.wikipedia.org%2F%3E%20.%0A%20%20%20%20%7D%0A%20%20%20%20OPTIONAL%20%7B%0A%20%20%20%20%20%20%3Farticle%20schema%3Aabout%20%3Fitem%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AinLanguage%20%22en%22%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AisPartOf%20%3Chttps%3A%2F%2Fen.wikipedia.org%2F%3E%20.%0A%20%20%20%20%7D%0A%20%20%20%20BIND%20%28URI%28CONCAT%28%22https%3A%2F%2Fwww.geni.com%2Fpeople%2F%22%2C%3FGeniID%29%29%20AS%20%3FGeni%29%0A%20%20%0A%20%20%20%09OPTIONAL%20%7B%20%3Farticlerank%20schema%3Aabout%20%3Fitem.%20%7D%0A%20%20%20SERVICE%20wikibase%3Alabel%20%7B%20bd%3AserviceParam%20wikibase%3Alanguage%20%22sv%22%2C%22en%22.%20%7D%0A%7D%0AGROUP%20BY%20%3Fitem%20%3FitemLabel%20%3FitemDescription%20%3Fcoord%20%3Farticle%20%3FGeni%20Having%20%28%3Frank%20%3E%205%29%0AORDER%20BY%20DESC%28%3Frank%29%0A) och [saknar gravbild](https://query.wikidata.org/embed.html#%23title%3A%20Gravar%20d%C3%A4r%20personen%20finns%20med%20artikel%20%3E%205%20spr%C3%A5k%20och%20saknar%20gravbild%0A%23defaultView%3AMap%0ASELECT%20%3Fitem%20%3FitemLabel%20%3FitemDescription%20%3Fcoord%20%28SAMPLE%28%3FpicGrave%29%20as%20%3FpicGrave%29%20%28SAMPLE%28%3Fimg%29%20as%20%3Fimg%29%20%3Farticle%20%3FGeni%20%28SAMPLE%28%3Fgraveplot%29%20as%20%3Fgraveplot%29%20%0A%28COUNT%28%3Fitem%29%20AS%20%3Frank%29%0A%09WHERE%20%7B%20%0A%20%09%09%09%09%09%3Fitem%20wdt%3AP119%20wd%3AQ213988%20.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%3Fitem%20p%3AP119%20%3FplaceofBurial%20.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP18%20%3Fimg%7D.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP569%20%3FbirthDate%7D.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3FplaceofBurial%20pq%3AP965%20%3Fgraveplot%7D%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3FplaceofBurial%20pq%3AP625%20%3Fcoord%7D%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20minus%20%7B%20%3Fitem%20wdt%3AP1442%20%3FpicGrave%20%7D%20%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20%7B%20%3Fitem%20wdt%3AP2600%20%3FGeniID%20%7D%0A%20%20%20%20OPTIONAL%20%7B%0A%20%20%20%20%20%20%3Farticle%20schema%3Aabout%20%3Fitem%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AinLanguage%20%22sv%22%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AisPartOf%20%3Chttps%3A%2F%2Fsv.wikipedia.org%2F%3E%20.%0A%20%20%20%20%7D%0A%20%20%20%20OPTIONAL%20%7B%0A%20%20%20%20%20%20%3Farticle%20schema%3Aabout%20%3Fitem%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AinLanguage%20%22en%22%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AisPartOf%20%3Chttps%3A%2F%2Fen.wikipedia.org%2F%3E%20.%0A%20%20%20%20%7D%0A%20%20%20%20BIND%20%28URI%28CONCAT%28%22https%3A%2F%2Fwww.geni.com%2Fpeople%2F%22%2C%3FGeniID%29%29%20AS%20%3FGeni%29%0A%20%20%0A%20%20%20%09OPTIONAL%20%7B%20%3Farticlerank%20schema%3Aabout%20%3Fitem.%20%7D%0A%20%20%20SERVICE%20wikibase%3Alabel%20%7B%20bd%3AserviceParam%20wikibase%3Alanguage%20%22sv%22%2C%22en%22.%20%7D%0A%7D%0AGROUP%20BY%20%3Fitem%20%3FitemLabel%20%3FitemDescription%20%3Fcoord%20%3Farticle%20%3FGeni%20Having%20%28%3Frank%20%3E%205%29%0AORDER%20BY%20DESC%28%3Frank%29%0A)
    * [Personer på Skogskytkogården med deras yrken](https://query.wikidata.org/embed.html#%23title%3A%20Yrken%20WikiData%20personer%20med%20gravplats%20wd%3AQ213988%20Skogskyrkog%C3%A5rden%0A%23defaultView%3AMap%0Aselect%20distinct%20%3FgroupLabel%20%28%3FgroupLabel%20as%20%3Flayer%29%20%3Farticle%20%3Fperson%20%3FpersonLabel%20%20%3FpersonDescription%20%20%3Fgraveplot%20%3Fcoord%20%3Fpic%20%3FpicGrave%20%3FWikiTree%20%3FFindAGrave%0A%28IRI%28CONCAT%28%22https%3A%2F%2Fwww.google.com%2Fmaps%2F%3Fq%3D%22%2C%20STR%28%3Flat%29%2C%20%22%2C%22%2C%20STR%28%3Flon%29%29%29%20AS%20%3FGoogleMap%29%20%3FGravstensinv%20%7B%0A%7B%0A%09%3Fperson%20wdt%3AP119%20wd%3AQ213988%3B%20%23Place%20of%20burial%0A%20%20%20%20%20%20%20%20%20%20%20%20p%3AP119%20%5B%20%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20pq%3AP965%20%3Fgraveplot%3B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20pq%3AP625%20%3Fcoord%3B%20%20%20%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20pqv%3AP625%20%5B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20wikibase%3AgeoLatitude%20%3Flat%3B%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20wikibase%3AgeoLongitude%20%3Flon%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%5D%0A%20%20%20%20%20%20%20%20%20%20%20%20%5D.%20%20%20%20%20%20%20%20%0A%20%20%20OPTIONAL%20%7B%20%3Fperson%20wdt%3AP535%20%3FFindAGraveID%20.%7D%20%09%09%23%20If%20we%20have%20a%20FindAGrave%20ID%0A%20%20%20OPTIONAL%20%7B%20%3Fperson%20wdt%3AP18%20%3Fpic%20.%7D%20%09%09%09%09%09%23%20If%20we%20have%20an%20illustration%0A%20%20%20OPTIONAL%20%7B%20%3Fperson%20wdt%3AP5259%20%3Fgid%20.%7D%20%09%09%20%20%20%20%20%20%20%20%0A%20%20%20OPTIONAL%20%7B%20%3Fperson%20wdt%3AP1442%20%3FpicGrave%20.%7D%20%09%09%09%23%20If%20we%20have%20a%20picture%20of%20the%20grave%0A%20%20%20BIND%20%28URI%28CONCAT%28%22https%3A%2F%2Fwww.rotter.se%2Fgsi%2F%22%2C%3Fgid%29%29%20AS%20%3FGravstensinv%29%0A%20%20%20BIND%20%28URI%28CONCAT%28%22http%3A%2F%2Fwww.findagrave.com%2Fcgi-bin%2Ffg.cgi%3Fpage%3Dgr%26df%3Dall%26GRid%3D%22%2C%3FFindAGraveID%29%29%20AS%20%3FFindAGrave%29%0A%20%20OPTIONAL%20%7B%0A%20%20%20%20%20%20%3Farticle%20schema%3Aabout%20%3Fperson%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AinLanguage%20%22sv%22%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AisPartOf%20%3Chttps%3A%2F%2Fsv.wikipedia.org%2F%3E%20.%0A%20%20%20%20%7D%0A%0A%20%20%20OPTIONAL%20%7B%20%3Fperson%20wdt%3AP106%20%3Fgroup%20.%7D%20%09%09%09%23%20Occupation%20in%20Layer%0A%0A%7D%20%20%20%0A%20%20SERVICE%20wikibase%3Alabel%20%7B%20bd%3AserviceParam%20wikibase%3Alanguage%20%22sv%22%2C%22en%22%7D%0A%20%7D%0AOrder%20by%20%3FgroupLabel)
 * Uppsala Gamla kykogård [karta](https://w.wiki/YgA) / [lista](https://sv.wikipedia.org/wiki/Anv%C3%A4ndare:Salgo60/%C3%96nskem%C3%A5l_om_bilder/Sverige/Uppsala_Gamla)
 * [Adolf Fredriks kyrkogård blog](http://minancestry.blogspot.com/2018/05/adolf-fredriks-kyrkogard.html)

* [Entity Schema E380](https://www.wikidata.org/wiki/EntitySchema:E380) -  [video](https://youtu.be/Ef5qKnByR2c) se nedan _CheckShex.js_
  *  [video2](https://www.youtube.com/watch?v=Utdg8z28GJw)


## Verktyg Wikidata 
Anpassningar som kan göras i Wikidata med gadgets...
* [Video hur OSM kopplingen fungerar](https://youtu.be/UJsT2UOkiTI) / [video2](https://youtu.be/Utdg8z28GJw)

se mer verktyg jag använder se [exempel där jag beskriver vad vi gjort med Riksdagens data](https://github.com/salgo60/Wikidata_riksdagen-corpus/issues/84#issuecomment-1352632278)

Exempel rad som skall in i Wikidata [common.js](https://www.wikidata.org/wiki/Special:MyPage/common.js) jmf med [min](https://www.wikidata.org/wiki/User:Salgo60/common.js)
> mw.loader.load( '//www.wikidata.org/w/index.php?title=User:Tohaomg/rearrange_values.js&action=raw&ctype=text/javascript' ); // [[User:Tohaomg/rearrange values.js]]

* detta verktyg gär att man kan flytta runt värden enklare på ett WD objekt

### Open Street Map (OSM) iFrame

Exempel hur en OSM kyrkogård med Wikidata koppling visas i en iframe på WD sida

<img width="1258" alt="image" src="https://user-images.githubusercontent.com/14206509/210293364-aaf6fc91-8b33-4db9-8d95-a6d254e7e47e.png">

* rad som skall in i common.js
> mw.loader.load( '//www.wikidata.org/w/index.php?title=User:Mxn/overpass.js&action=raw&ctype=text/javascript' );

### Schema ShAcl
* verktyg för att validera objekt mot ett entity schema se [video](https://youtu.be/Ef5qKnByR2c) / [video2](https://www.youtube.com/watch?v=Utdg8z28GJw)

> importScript( 'User:Teester/CheckShex.js' );
#### Quota problem - 

Mark Tully, [2022-07-11 11:47]
CheckShex uses PyShexy to check entities against schemas.  Unfortunately, it tends to fail fairly often as the backend relies on WDQS and keeps overusing its quota.

> Mark Tully, [2022-07-11 11:47]
> EntityShape provides per statement and per property checks against the schema.  It uses the mediawiki api to perform the checks so doesn't have the quota problem that CheckShex has, but it doesn't support all the features of entityschemas.  In particular, it doesnt support IMPORT or AND or OR statements, but it works well for simple schemas.

## Browser Plug-in

* [Wikidata:Entity_Explosion](https://www.wikidata.org/wiki/Wikidata:Entity_Explosion)
* [Video](https://youtu.be/Al-I_qMCuUk)

<img width="691" alt="image" src="https://user-images.githubusercontent.com/14206509/201900611-2e0a1626-e696-4f79-8864-1664e3eedfc4.png">

## Licens
* [Wikidata licens](https://www.wikidata.org/wiki/Wikidata:Licensing) CC-0

## Misc
* [Möte 2018 med släktforskarförbundet](https://phabricator.wikimedia.org/T202219#4573028)

# Andra projekt / tankar 
## Kopplingar RAÄ böcker kyrkor
Kyrkor dokumenteras av RAÄ och kan innehålla info om gravplatsen och gravar. Jag gjorde en snabb test 2018 att koppla ihop dessa böcker med rätt kyrka men äve för Riddarholmskyrkan vilka personers grava i en kyrka som beskrivs se GITHUB [salgo60/SamlaLibris](https://github.com/salgo60/SamlaLibris)

* [Map with churches](https://w.wiki/38V) that are documented in a RAÄ Book (also links LIBRIS/LIBRIS XL/sv:Wikipedia)

[![image](https://user-images.githubusercontent.com/14206509/210299045-b708da96-6db8-470a-97cd-e2dd0047bbda.png)](https://w.wiki/38V)

* [Personer beskrivna begravda i Riddarholmskyrkan](https://w.wiki/3Dd) beskrivna av en book [wd:Q61765464](https://www.wikidata.org/wiki/Q61765464)

[![image](https://user-images.githubusercontent.com/14206509/210299177-e44ec736-8b0a-4bef-88e5-6c26b366ee87.png)](https://w.wiki/3Dd)

## Hitta bilder på personer som ligger begravda på en kyrkogård med WIkidata / Svenskt porträttarkiv

[Video](https://youtu.be/j-OhaeNshhE) - [GITHUB SPA2Commons](ss) - [Wikicommons Kategori för uppladade bilder från SPA](https://commons.wikimedia.org/wiki/Category:Uploaded_with_spa2Commons)
* [Notebook](https://github.com/salgo60/spa2Commons/blob/main/Notebook/SPA%20cemetery.ipynb) som letar alla personer kopplade till Gamla Gävle begravningsplats i Wikidata men saknar bild och slår sedan mot Svenskt Porträtt arkiv om det finns där kandidater
  * [WD Q26257009](https://www.wikidata.org/wiki/Q26257009) Gamla Gävle Begravningsplats

Exempel hur en kandidat presenteras med Ranking

<img width="1260" alt="image" src="https://user-images.githubusercontent.com/14206509/210300100-7f57f027-4ad7-4f76-b6ba-9593c0b33bad.png">

* [Blog om Gamla Gävle Begravningsplats](http://minancestry.blogspot.com/2020/03/gavle.html) i Wikidata

## WD <-> FindAgrave cemetery
* [Map all locations](https://w.wiki/6LcM) withs a FindAGrave cemetery property
** Map all also connected to Open Street Map

[<img width="983" alt="image" src="https://user-images.githubusercontent.com/14206509/218990978-edafd4dd-9674-46c0-820b-acfaeeb76fa5.png">](https://w.wiki/6LcM) 

## Riksdagsmän finns ofta på kyrkogårdar
* Wikimedia Sverige försöker nu jobba med Hembyggdsföreningar ett "enkelt" fall kanske är Riksdagspolitiker som finns i socken
** Wikimedia Sverige projekt sponsat av sss
** Hur vi [kopplar alla Sveriges Riksdagsmän #38](https://github.com/salgo60/Wikidata_riksdagen-corpus/issues/38)
** Projekt som HUMLAB startar för att göra en "kopia av" Wikidata dvs. en Kunskapsgraf
*** [Karta där Riksdagsgubbarna är födda enl. Wikidata](https://w.wiki/6BmD)

<img width="666" alt="image" src="https://user-images.githubusercontent.com/14206509/210617736-df16844b-6acb-4969-9120-5e89f6fe952e.png">

* [Projekt:Wikipedia för hela Sverige 2022](https://se.wikimedia.org/wiki/Projekt:Wikipedia_f%C3%B6r_hela_Sverige_2022)

<img width="1084" alt="image" src="https://user-images.githubusercontent.com/14206509/210618794-67f13951-00a9-4b71-b9c0-ffa52f466970.png">
