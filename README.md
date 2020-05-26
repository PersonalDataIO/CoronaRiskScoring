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
- Google ([wiki](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Google-Exposure-Notification-framework-configuration))/Apple ([wiki](https://github.com/PersonalDataIO/CoronaRiskScoring/wiki/Apple-Exposure-Notification-framework-configuration)) Exposure Notification based
  - Switzerland: [SwissCovid](https://github.com/DP-3T/)
  - Germany: [Corona Warn](https://github.com/corona-warn-app)
  - Italy: [Immuni](https://github.com/immuni-app)
- < many we are missing >


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
