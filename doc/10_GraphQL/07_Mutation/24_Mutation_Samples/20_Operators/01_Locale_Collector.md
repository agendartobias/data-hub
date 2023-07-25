---
title: Locale Collector
---

# Sample for Mutation Operator "Locale Collector"

```graphql
mutation {
  updateTable(
    id: 7
    input: {
      name_translated: {
        en: "Dinner table"
        de: "Esstisch"
      }
    }
  ) {
    success
    message
    output {
      name_en: name(language: "en")
      name_de: name(language: "de")
    }
  }
}
```

To get this working you must first add Locale Collector in your Mutation Schema definition to Available Fields

![Car_locale_collector](https://github.com/pimcore/data-hub/assets/28923508/2d5c37af-150e-46fb-863a-1bcf1cd929dc)
