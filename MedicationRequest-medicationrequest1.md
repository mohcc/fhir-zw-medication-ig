# Example Medication Request (Antimalarial) - Zimbabwe Medication IG v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Example Medication Request (Antimalarial)**

## Example MedicationRequest: Example Medication Request (Antimalarial)

Profile: [Zimbabwe Medication Request](StructureDefinition-zw-medication-request.md)

**status**: Active

**intent**: Order

**medication**: Artemether/Lumefantrine 20/120 mg tablet

**subject**: `zw-patient-example`

**encounter**: `encounter1`

**authoredOn**: 2026-05-01

**requester**: `practitioner1`

**reasonReference**: `condition1`

### DosageInstructions

| | |
| :--- | :--- |
| - | **Text** |
| * | 1 tablet twice daily for 3 days |



## Resource Content

```json
{
  "resourceType" : "MedicationRequest",
  "id" : "medicationrequest1",
  "meta" : {
    "profile" : ["http://mohcc.gov.zw/fhir/medication/StructureDefinition/zw-medication-request"]
  },
  "status" : "active",
  "intent" : "order",
  "medicationCodeableConcept" : {
    "text" : "Artemether/Lumefantrine 20/120 mg tablet"
  },
  "subject" : {
    "reference" : "zw-patient-example"
  },
  "encounter" : {
    "reference" : "encounter1"
  },
  "authoredOn" : "2026-05-01",
  "requester" : {
    "reference" : "practitioner1"
  },
  "reasonReference" : [{
    "reference" : "condition1"
  }],
  "dosageInstruction" : [{
    "text" : "1 tablet twice daily for 3 days"
  }]
}

```
