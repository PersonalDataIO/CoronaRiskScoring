---
name: Where are the keys
about: This template quickly asks where the keys are
title: Where are the keys stored in XXX ?
labels: ''
assignees: ''

---

The [CoronaRiskScoring](https://github.com/PersonalDataIO/CoronaRiskScoring/) project is trying to assess how different contact tracing apps are being parametrized. For this purpose, we need to know how many TEKs get published per day, and their risk levels (all public information). 

**Project considered**
We are looking at XXXX.

**What we need**
We need to have a procedure describing how to pull down the keys reliably. 

**Nice to have**
We would like to find in the code where this code is downloaded from, which is generally around [`func detectExposures(configuration: ENExposureConfiguration, 
    diagnosisKeyURLs: [URL], 
   completionHandler: @escaping ENDetectExposuresHandler) -> Progress`](https://developer.apple.com/documentation/exposurenotification/enmanager/3586331-detectexposures) in the iOS app. 

**Excellent to have**
Ideally we would have a little code snippet to run and pull down the necessary data, or a URL to do this directly.
