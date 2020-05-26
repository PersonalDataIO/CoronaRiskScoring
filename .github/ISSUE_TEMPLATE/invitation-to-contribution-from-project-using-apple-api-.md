---
name: 'Invitation to contribution from project using Apple API '
about: This template quickly explains the situation to a project leveraging the Apple
  API
title: How is ExposureConfiguration set in XXXX ?
labels: ExposureConfiguration, InvitationToContribute
assignees: ''

---

The [CoronaRiskScoring](https://github.com/PersonalDataIO/CoronaRiskScoring/) project is trying to assess how different contact tracing apps are being parametrized. We are first focusing on apps using the Apple API as it will enable quickest comparison. 

**Project considered**
We are looking at XXXX.

**What we need**
We need pointers to the places in the code where the following parameters are set:
* `ENExposureConfiguration`.**[`attenuationLevelValues`](https://developer.apple.com/documentation/exposurenotification/enexposureconfiguration/3586319-attenuationlevelvalues)**, 
* `ENExposureConfiguration`.**[`daysSinceLastExposureLevelValues`](https://developer.apple.com/documentation/exposurenotification/enexposureconfiguration/3586320-dayssincelastexposurelevelvalues)**,
* `ENExposureConfiguration`.**[`durationLevelValues`](https://developer.apple.com/documentation/exposurenotification/enexposureconfiguration/3586321-durationlevelvalues)**, 
* `ENExposureConfiguration`.**[`transmissionRiskLevelValues`](https://developer.apple.com/documentation/exposurenotification/enexposureconfiguration/3586323-transmissionrisklevelvalues)** and 
* `ENExposureConfiguration`.`metadata`.**[`attenuationDurationThresholds`](https://developer.apple.com/documentation/exposurenotification/enexposureconfiguration/3586322-metadata)**

**Nice to have**
We would also like to understand what is done with `ENExposureDetectionSummary` and `ENExposureInfo`, after the risks are calculated. 

**Excellent to have**
This is only the beginning for us. We want the above so we can track how the parameters are being changed. It is likely actually that this is passed dynamically to the apps. If so, we need to know the process behind these changes, so we can ask the right people for this information. 

If you have pointers in the right direction, they would be greatly appreciated.
