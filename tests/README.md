# gbiz-templates

Public raw templates for Grok Bot tests.

## Layout

```
tests/
  phase1/                  # current friend test (EA + Follow-up Desk + Research Assistant)
    pack-manifest.yaml
    ea-right-hand/
    followup-desk/
    research-assistant/
    starters/
```

Future tests sit as siblings under `tests/`.
Bot templates live one level deeper inside each test folder.
