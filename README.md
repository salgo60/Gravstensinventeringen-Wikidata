# Gravstensinventeringen-Wikidata
Se hur vi kan kan koppla ihop WIkidata och Gravstensinventeringen bättre

Idag finns egenskap [Property:P5259](https://www.wikidata.org/wiki/Property:P5259) i Wikidata med ung, 500 poster kopplade 
* [video](https://www.youtube.com/watch?v=hNaK1iNSvhE)
* SPARQL [andra WD egenskaper där P5259 finns](https://w.wiki/5xGr) / [enbart externa](https://w.wiki/5xGo)
* Karta gravar / [kyrkogårdar](https://w.wiki/5xJd)
  * karta [FindAGrave och Gravstensinventeringen](https://w.wiki/5xKc) / [alla FindAgrave begravningsplatser i WD](https://w.wiki/5xQt) > 12000
* [Möte 2018](https://phabricator.wikimedia.org/T202219#4573028)
* [Video](https://youtu.be/QPpYAFSgJ3g) hur Wikidata kopplar ihop Wikipedia och bilder på gravar

## Gravar kopplas till person/koordinat i Wikidata 
Exempel
* [Gävle Gamla kyrkogård](http://minancestry.blogspot.com/2020/03/gavle.html)
* Norra Begravningsplatsen karta / 
  * [Födelseplatser på personer](http://tinyurl.com/m2935bb) begravda på Norra Begravningsplatsen enl. Wikidata
  * Personer på [Norra Begravningsplatsen som har artikel > 10 språk](https://query.wikidata.org/embed.html#%23title%3A%20Gravar%20d%C3%A4r%20personen%20finns%20m%2Ced%20artikel%20%3E%2010%20spr%C3%A5k%0A%23defaultView%3AMap%0ASELECT%20%3Fitem%20%3FitemLabel%20%3FitemDescription%20%3Fcoord%20(SAMPLE(%3FpicGrave)%20as%20%3FpicGrave)%20(SAMPLE(%3Fimg)%20as%20%3Fimg)%20%3Farticle%20%3FGeni%20(SAMPLE(%3Fgraveplot)%20as%20%3Fgraveplot)%20%0A(COUNT(%3Fitem)%20AS%20%3Frank)%0A%09WHERE%20{%20%0A%20%09%09%09%09%09%3Fitem%20wdt%3AP119%20wd%3AQ252312%20.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%3Fitem%20p%3AP119%20%3FplaceofBurial%20.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20{%20%3Fitem%20wdt%3AP18%20%3Fimg}.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20{%20%3Fitem%20wdt%3AP569%20%3FbirthDate}.%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20{%20%3FplaceofBurial%20pq%3AP965%20%3Fgraveplot}%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20{%20%3FplaceofBurial%20pq%3AP625%20%3Fcoord}%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20{%20%3Fitem%20wdt%3AP1442%20%3FpicGrave%20}%20%0A%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20%20OPTIONAL%20{%20%3Fitem%20wdt%3AP2600%20%3FGeniID%20}%0A%20%20%20%20OPTIONAL%20{%0A%20%20%20%20%20%20%3Farticle%20schema%3Aabout%20%3Fitem%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AinLanguage%20%22sv%22%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AisPartOf%20%3Chttps%3A%2F%2Fsv.wikipedia.org%2F%3E%20.%0A%20%20%20%20}%0A%20%20%20%20OPTIONAL%20{%0A%20%20%20%20%20%20%3Farticle%20schema%3Aabout%20%3Fitem%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AinLanguage%20%22en%22%20.%0A%20%20%20%20%20%20%3Farticle%20schema%3AisPartOf%20%3Chttps%3A%2F%2Fen.wikipedia.org%2F%3E%20.%0A%20%20%20%20}%0A%20%20%20%20BIND%20(URI(CONCAT(%22https%3A%2F%2Fwww.geni.com%2Fpeople%2F%22%2C%3FGeniID))%20AS%20%3FGeni)%0A%20%20%0A%20%20%20%09OPTIONAL%20{%20%3Farticlerank%20schema%3Aabout%20%3Fitem.%20}%0A%20%20%20SERVICE%20wikibase%3Alabel%20{%20bd%3AserviceParam%20wikibase%3Alanguage%20%22sv%22%2C%22en%22.%20}%0A}%0AGROUP%20BY%20%3Fitem%20%3FitemLabel%20%3FitemDescription%20%3Fcoord%20%3Farticle%20%3FGeni%20Having%20(%3Frank%20%3E%2010)%0AORDER%20BY%20DESC(%3Frank)%0A)
 * Uppsala Gamla kykogård [karta](https://w.wiki/YgA) / [lista](https://sv.wikipedia.org/wiki/Anv%C3%A4ndare:Salgo60/%C3%96nskem%C3%A5l_om_bilder/Sverige/Uppsala_Gamla)
 * [Adolf Fredriks kyrkogård blog](http://minancestry.blogspot.com/2018/05/adolf-fredriks-kyrkogard.html)
