# CoronaRiskScoring

This is an effort to have a broad and comparative discussion around risk scoring algorithms in Bluetooth based corona-tracking apps, highlighting subtle nuances in their conception and parametrization. 

It is worth reminding all those going through those pages that:
* Bluetooth only serves in those apps as a proxy for distance;
* that it is [very imperfect](https://medium.com/personaldata-io/inferring-distance-from-bluetooth-signal-strength-a-deep-dive-fe7badc2bb6d);
* that there is a lot of selection bias in the data;
* that it is not clear such interventions are more helpful than alternatives.

We currently use the following color coding, which will evolve:
- ![#c5f015](https://via.placeholder.com/15/c5f015/000000?text=+) low risk / good / present <green>
- ![#FFFF33](https://via.placeholder.com/15/FFFF33/000000?text=+) medium risk / medium / deadline set <yellow>
- ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) high risk / bad / no deadline set <red>

| Project | Twitter | Authority	| Protocol | Code Repository | Reproducible Build | Parameter Transparency	| Parameter Update Transparency | COVID+ key repo|
|:-:	|:-:	|:-:	|:-:	|:-:	|:-:	|:-:	|:-:	|:-: |
|  [StopCovid](https://gitlab.inria.fr/stopcovid19) 	| [#StopCovid](https://twitter.com/search?q=%23StopCovid&src=typed_query&f=live)|  France  | custom  |  [GitHub](https://gitlab.inria.fr/stopcovid19)   |       ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) |   [robert-server/#22](https://gitlab.inria.fr/stopcovid19/robert-server/-/issues/22)   | ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) | Not applicable|
|  [SwissCovid](https://github.com/DP-3T/) 	| [@SwissCovid](https://twitter.com/SwissCovid), [#SwissCovid](https://twitter.com/search?q=%23SwissCovid&src=typed_query&f=live) |   [@BAG_OFSP_UFSP](https://twitter.com/BAG_OFSP_UFSP), Switzerland  	|  [Google](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Google-Exposure-Notification-framework-configuration)/ [Apple](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Apple-Exposure-Notification-framework-configuration) Exposure Notification   |  [GitHub](https://github.com/DP-3T/)   | ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) |  [#3](https://github.com/PersonalDataIO/CoronaRiskScoring/issues/3)   |    ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) |[#13](https://github.com/PersonalDataIO/CoronaRiskScoring/issues/13)|
|   ApturiCovid	|  [@apturicovid](https://twitter.com/apturicovid), [#ApturiCovid](https://twitter.com/search?q=%23ApturiCovid&src=typed_query&f=live)  |  Latvia   |  [Google](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Google-Exposure-Notification-framework-configuration)/ [Apple](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Apple-Exposure-Notification-framework-configuration) Exposure Notification  | ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+)|  ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+)   |   ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+)  | ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+)| security by obscurity|
|   [SmitteStop](https://smittestop.dk/)	|  [@apturicovid](https://twitter.com/smittestop), [#SmitteStop](https://twitter.com/search?q=%23SmitteStop&src=typed_query&f=live)  |  Statens Serum Institut, Denmark  |  [Google](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Google-Exposure-Notification-framework-configuration)/ [Apple](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Apple-Exposure-Notification-framework-configuration) Exposure Notification  | ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+)|  ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+)   |   ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+)  | ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+)|security by obscurity|
|  [Immuni](https://github.com/immuni-app)	| [#ImmuniApp](https://twitter.com/hashtag/ImmuniApp?src=hashtag_click), [#Immuni](https://twitter.com/hashtag/Immuni?src=hashtag_click) |   Extraordinary Commissioner for the COVID-19 Emergency, Italy  	|  [Google](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Google-Exposure-Notification-framework-configuration)/ [Apple](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Apple-Exposure-Notification-framework-configuration) Exposure Notification   |  [GitHub](https://github.com/immuni-app)   | ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) |  [#5](https://github.com/PersonalDataIO/CoronaRiskScoring/issues/5), [Android v1](https://get.immuni.gov.it/v1/settings?platform=android&build=1), [iOS v1](https://get.immuni.gov.it/v1/settings?platform=ios&build=1)  |    ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) |[#14](https://github.com/PersonalDataIO/CoronaRiskScoring/issues/14)|
|  [ProteGo Safe](https://github.com/ProteGO-Safe)	| [#ProteGoSafe](https://twitter.com/hashtag/ProteGoSafe?src=hashtag_click) |   ??, Poland 	|  [Google](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Google-Exposure-Notification-framework-configuration)/ [Apple](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Apple-Exposure-Notification-framework-configuration) Exposure Notification   |  [GitHub](https://github.com/ProteGo-Safe)   | ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) |  [#6](https://github.com/PersonalDataIO/CoronaRiskScoring/issues/6)  |    ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) |[#10](https://github.com/PersonalDataIO/CoronaRiskScoring/issues/10)|
|  [CoronaWarn](https://github.com/corona-warn-app)	| #CoronaWarnApp @CoronaWarnApp|  Germany 	|  [Google](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Google-Exposure-Notification-framework-configuration)/ [Apple](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Apple-Exposure-Notification-framework-configuration) Exposure Notification   |  [GitHub](https://github.com/corona-warn-app)   | ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) |  [#7](https://github.com/PersonalDataIO/CoronaRiskScoring/issues/7)  |    ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) |[#9](https://github.com/PersonalDataIO/CoronaRiskScoring/issues/9)|
|  [CovidTracker](https://covidtracker.gov.ie/)	| |  Ireland 	|  [Google](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Google-Exposure-Notification-framework-configuration)/ [Apple](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Apple-Exposure-Notification-framework-configuration) Exposure Notification   |  [GitHub](https://github.com/HSEIreland/covidtracker-documentation)   | ![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) | TBD| TBD |TBD|
|  StoppCorona 	|    [GitHub](https://github.com/austrianredcross/stopp-corona-documentation) 	|  Austria  |     |     |     |  See  https://github.com/austrianredcross/stopp-corona-documentation/wiki/Key-matching-process#batches-provided-by-the-server   ||

Other projects analyzed:
- [OpenCoronavirus](https://github.com/open-coronavirus)
- UK: [NHSx](https://github.com/nhsx/)
- [MITL/PACT East](https://github.com/mitll/)
- [SafePath](https://github.com/Path-Check)
- Austria: [StoppKorona](https://github.com/austrianredcross)
- Norway: [SmitteStopp](https://www.simula.no/news/digital-contact-tracing-qa)
- Netherlands: https://github.com/minvws
- [Google](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Google-Exposure-Notification-framework-configuration)/ [Apple](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Apple-Exposure-Notification-framework-configuration) Exposure Notification based

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
