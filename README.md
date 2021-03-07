# Social-media-analytics
Social media analytics
Kuinka tutkia asiakaskokemusta Twitter-viesteistä?

Kuinka tehdä täydellinen Twitter-analyysi asiakaskokemuksesta?

Miten ja kuinka voidaan tutkia asiakaskokemusta asiakkaiden Twitter-viesteistä? Miten asiakkaat olivat reagoineet, tunteneet ja ajatelleet Twitter-viesteissä heti asiakaskokemuksen tai palvelukohtaamisen jälkeen? Saatiinko yhtä paljon myönteisiä, kielteisiä ja neutraaleja tunteita? Mitä tekstuaalinen data Twitter-viesteistä voi kertoa kielteisistä ja myönteisistä tunteista? Mitkä olivat yleisimmät syyt, kun asiakkaat kertoivat kielteisistä tunteista. Onko ajalla esimerkiksi yhteyttä kielteisiin tunteisiin?

Näihin kysymyksiin hain vastauksia. Käytettävissä oli helmikuulta 2015 data, joka sisälsi noin 15 000 riviä tietoa. Twitter-viestien lähettäjinä olivat yhdysvaltalaisten lentoyhtiöiden asiakkaat heti asiakaskohtaamisen jälkeen.

Laajaa datajoukkoa kävin läpi sentimenttianalyysillä, joka kategorisoi tekstipohjaiset viestit eli tviitit sävyn mukaan. Sävy voi olla joko myönteinen, neutraali tai kielteinen. Samalla viesteistä eritellään esiin nousevat teemat eli usein esiintyvät termit ja aiheet. Tarkoituksena oli tarkastella myönteisiä ja kielteisiä kokemuksia sekä vertailla näitä tuloksia lentoyhtiöiden välillä. Kuinka asiakkaat olivat reagoineet, tunteneet ja ajatelleet asiakaskokemuksesta Twitterissä kohtaamisen jälkeen? Siksi viesteistä oli nostettu esiin syyt muun muassa kielteiselle asiakaskokemukselle.

Datassa oli edustettuna kuusi suurta yhdysvaltalaista lentoyhtiötä. Kaikki lentoyhtiöt saivat kielteisiä reaktioita enemmän kuin neutraaleja tai myönteisiä.

Virgin America sai lähes yhtä paljon kielteisiä, myönteisiä ja neutraaleja. Virgin Americalla tviittien kokonaismäärä oli kuitenkin merkittävästi pienempi kuin muilla lentoyhtiöillä.

Tehdään seuraavaksi sanapilvianalyysi kielteisistä sentimenteistä. Mitä suurempi sanafontti, sitä suurempi frekvenssi on tekstidatassa. Sanat kuten cancelled, bag, delay, plane, hold, time ovat yleisimpien sanojen joukossa. Mutta joukossa on myös sanoja, jotka eivät välttämättä tarkoita mitään.

Tehdään seuraavaksi sanapilvianalyysi myönteisistä sentimenteistä. Mitä suurempi sanafontti, sitä suurempi frekvenssi on tekstidatassa. Sanat kuten thank, best, customer, love, flying, good ovat yleisimpien sanojen joukossa. Mutta joukossa on myös sanoja, jotka eivät välttämättä tarkoita mitään.

Tehdään seuraavaksi sanapilvianalyysi neutraalista sentimenteistä. Mitä suurempi sanafontti, sitä suurempi frekvenssi on tekstidatassa. Sanat kuten thank, flight, ticket, change ovat yleisimpien sanojen joukossa. Mutta joukossa on myös sanoja, jotka eivät välttämättä tarkoita mitään.

Seuraavaksi lasketaan frekvenssit. Sanat kuten flight, cancelled, change ovat yleisimpien joukossa. Mutta joukossa on myös sanoja, jotka eivät välttämättä tarkoita mitään. Suurin osa on niin sanottuja stop-sanoja, jotka pitää filtteröidä pois, jos analyysi halutaan viedä vielä pidemmälle. Lista frekvensseistä on Python-koodissani.

Lasketaan seuraavaksi yleisimmät syyt kielteisistä sentimenteistä. Suurin selittävä syy kielteiselle asiakaskokemukselle oli tietty asiakaspalveluun liittynyt tilanne. Toiseksi yleisin syy oli lennon myöhästyminen. Kolmanneksi yleisin syy oli se, että vastaaja ei kyennyt kertomaan tarkkaa syytä kielteiselle asiakaskokemukselle. Neljänneksi yleisin syy oli peruuntunut lento ja viidenneksi kadonneet matkatavarat lennon aikana.

Yksittäinen asiakaspalvelun aihe oli yleisin kielteinen syy US Airways, United, American, Southwest, Virgin America-aineistoissa. Lentojen myöhästyminen eli Late Flight oli yleisin kielteinen syy Deltalle. Virgin America sai vähiten kielteisiä syitä. Toisaalta US Airways, United, American saivat yli 500 kielteistä syytä, selittävänä tekijä muun muassa yksittäinen asiakaspalvelun tilanne (Customer Service Issue).

Seuraavaksi katsotaan, onko päivämäärällä yhteyttä kielteisiin sentimentteihin. Miltä sentimentit näyttävät ajanjaksolle maanantaista 16.2.2015 seuraavan viikon tiistaihin 24.2.2015 kullekin lentoyhtiölle? Sunnuntai oli 22.2.2015. Plotataan alle seuraavaksi sentimentit ajanjaksoille.

Kiinnostavaa on se, että American-yhtiöllä kielteinen sentimentti nousi jyrkästi 23.2.2015, joka puolittui 24.2.2015. Virgin America -yhtiöllä on vähiten kielteisiä tviittejä, pitää kuitenkin muistaa, että Virgin Americalla on tviittejä vähiten kokonaismäärältään suhteessa muihin. Kielteisten tviittien määrä on vinoutunut loppuviikosta suhteessa muuhun viikkoon.

Asiakaskokemuksen mittaaminen on noussut keskeiseen asemaan monessa työyhteisössä. Miksi sen mittaaminen on tärkeää? Erinomainen asiakaskokemus vetää myynnin ja kasvun mittareita ylöspäin. Asiakaskokemuksen ydin on työyhteisön ja asiakkaan vuorovaikutuksessa.

Asiakaskokemus käsittää mielikuvia ja tunteita, jotka syntyvät asiakkaalle kohtaamisista yhteisön edustajien, kanavien ja palveluiden kanssa. Hyvä asiakaskokemus tarkoittaa, että asiakaskokemus vastaa hänen odotuksiaan. Myönteinen asiakaskokemus pitää yllä asiakasuskollisuutta ja houkuttelee uusia asiakkaita.

Tämän analyysin tuloksena voidaan suositella, että lentoyhtiöt parantaisivat asiakaskokemustaan, jos ne panostaisivat lentojen täsmällisyyteen ja asiakasvuoropuheluun kadonneitten tavaroiden tapauksessa.
