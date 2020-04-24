![CI](https://github.com/sensein/covid19/workflows/CI/badge.svg)

# Covid19 voice protocol

Activities (tasks):
* covid19
    * Items: covid19_clinical_history, covid19_status, covid19_symptoms, fever, smoking_history 
* voice
    * Items: caterpillar_fast, kmart_exhale, nasal_pinched, say_ah, say_ng
* voice_opt

Test all files with ```@content``` from command line:
```
npm install -g jsonlint
grep -r --exclude-dir=node_modules --exclude-dir=ui --exclude-dir=.github "@context" . | cut -d: -f1 | xargs -I fname jsonlint -q fname
```

Test individual files here: ```https://jsonlint.com/```

Test protocol: ```https://schema.repronim.org/ui/#/?url=https://raw.githubusercontent.com/sensein/covid19/master/protocol/Covid19_schema```

the url is available in ```protocol/Covid19_schema``` and replace `context` with `schema` as done above
