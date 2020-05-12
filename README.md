![CI](https://github.com/sensein/covid19/workflows/CI/badge.svg)

# Covid19 voice protocol

This a protocol being used to assess impact of SARS-COV2 on speech production. 
The overall protocol is in the `protocol`folder and individual tasks and items
are in the `covid19`, `voice`, and `voice-opt` folders. 

Activities (tasks):
* covid19
    * Items: covid19_clinical_history, covid19_status, covid19_symptoms, fever, smoking_history 
* voice
    * Items: caterpillar_fast, kmart_exhale, nasal_pinched, say_ah, say_ng
* voice_opt
    * Items: An extend set of tasks

# Technical details

1. This repo uses [ReproSchema](https://github.com/ReproNim/reproschema/),
[ReproSchema-UI](https://github.com/ReproNim/reproschema-ui/).
2. The UI is added as a submodule (`ui`) and changes relative to the UI are stored 
in `ui-changes`.
3. The entire build is carried out by Github actions and deployed via gh-pages.

Test protocol: ```https://schema.repronim.org/ui/#/?url=https://raw.githubusercontent.com/sensein/covid19/master/protocol/Covid19_schema```