# Example Allergy (Penicillin) - Zimbabwe Medication IG v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Example Allergy (Penicillin)**

## Example AllergyIntolerance: Example Allergy (Penicillin)

Profile: [Zimbabwe Allergy Intolerance](StructureDefinition-zw-allergy-intolerance.md)

**clinicalStatus**: Active

**verificationStatus**: Confirmed

**type**: Allergy

**category**: Medication

**criticality**: High Risk

**code**: Penicillin

**patient**: `zw-patient-example`

**recordedDate**: 2026-05-01

**recorder**: `practitioner1`

### Reactions

| | |
| :--- | :--- |
| - | **Manifestation** |
| * | Urticaria (hives) |



## Resource Content

```json
{
  "resourceType" : "AllergyIntolerance",
  "id" : "allergyintolerance1",
  "meta" : {
    "profile" : ["http://mohcc.gov.zw/fhir/medication/StructureDefinition/zw-allergy-intolerance"]
  },
  "clinicalStatus" : {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/allergyintolerance-clinical",
      "code" : "active",
      "display" : "Active"
    }]
  },
  "verificationStatus" : {
    "coding" : [{
      "system" : "http://terminology.hl7.org/CodeSystem/allergyintolerance-verification",
      "code" : "confirmed",
      "display" : "Confirmed"
    }]
  },
  "type" : "allergy",
  "category" : ["medication"],
  "criticality" : "high",
  "code" : {
    "text" : "Penicillin"
  },
  "patient" : {
    "reference" : "zw-patient-example"
  },
  "recordedDate" : "2026-05-01",
  "recorder" : {
    "reference" : "practitioner1"
  },
  "reaction" : [{
    "manifestation" : [{
      "text" : "Urticaria (hives)"
    }]
  }]
}

```
