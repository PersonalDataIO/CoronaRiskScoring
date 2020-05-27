# CoronaRiskScoring

This is an effort to have a broad and comparative discussion around risk scoring algorithms in Bluetooth based corona-tracking apps, highlighting subtle nuances in their conception and parametrization. 

It is worth reminding all those going through those pages that:
* Bluetooth only serves in those apps as a proxy for distance;
* that it is [very imperfect](https://medium.com/personaldata-io/inferring-distance-from-bluetooth-signal-strength-a-deep-dive-fe7badc2bb6d);
* that there is a lot of selection bias in the data;
* that it is not clear such interventions are more helpful than alternatives.

Projects analyzed:
- France: [StopCovid](https://gitlab.inria.fr/stopcovid19)
- [OpenCoronavirus](https://github.com/open-coronavirus)
- UK: [NHSx](https://github.com/nhsx/)
- [MITL/PACT East](https://github.com/mitll/)
- [SafePath](https://github.com/Path-Check)
- Austria: [StoppKorona](https://github.com/austrianredcross)
- Norway: [SmitteStopp](https://www.simula.no/news/digital-contact-tracing-qa)
- Google ([wiki](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Google-Exposure-Notification-framework-configuration))/Apple ([wiki](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Apple-Exposure-Notification-framework-configuration)) Exposure Notification based
  - Switzerland: [SwissCovid](https://github.com/DP-3T/), see [issue #3](https://github.com/PersonalDataIO/CoronaRiskScoring/issues/3). [configuration rationale](https://github.com/DP-3T/documents/blob/master/DP3T%20-%20Exposure%20Score%20Calculation.pdf)
  - Germany: [Corona Warn](https://github.com/corona-warn-app)
  - Italy: [Immuni](https://github.com/immuni-app)
- 
- [< many we are missing, listed in PersonalData.IO's database>](https://query.personaldata.io/embed.html#PREFIX%20pdio%3A%20%3Chttps%3A%2F%2Fwiki.personaldata.io%2Fentity%2F%3E%0APREFIX%20pdiot%3A%20%3Chttps%3A%2F%2Fwiki.personaldata.io%2Fprop%2Fdirect%2F%3E%0APREFIX%20pdiop%3A%20%3Chttps%3A%2F%2Fwiki.personaldata.io%2Fprop%2F%3E%0APREFIX%20pdiops%3A%20%3Chttps%3A%2F%2Fwiki.personaldata.io%2Fprop%2Fstatement%2F%3E%0APREFIX%20pdiopq%3A%20%3Chttps%3A%2F%2Fwiki.personaldata.io%2Fprop%2Fqualifier%2F%3E%0A%0ASELECT%20%3Fitem%20%3FitemLabel%20%3Fandroid_store_id%20WHERE%20%7B%0A%20%20%3Fitem%20pdiot%3AP3%20pdio%3AQ4513.%0A%20%20SERVICE%20wikibase%3Alabel%20%7B%0A%20%20%20%20bd%3AserviceParam%20wikibase%3Alanguage%20%22en%22%20.%20%0A%20%20%7D%0A%20%20OPTIONAL%20%7B%3Fitem%20pdiot%3AP41%20%3Fandroid_store_id%7D%0A%20%20%0A%7D%0ALIMIT%20100)


# How to contribute?

* expand the list above
* contribute an issue describing your understanding of how risk scoring works in the app

Please consider:
* Android vs iOS
* Bluetooth ranging (is there an explicit step to produce a distance measurement?)
* How is risk calculated from a distance measurement?
* How transparent the app is about the whole process?
* see also [#2](https://github.com/PersonalDataIO/CoronaRiskScoring/issues/2)
* ...

# How to assist?
If you have experience contributing to or setting up a project such as this one, please provide suggestions on how to improve (for instance which features should we use?)
