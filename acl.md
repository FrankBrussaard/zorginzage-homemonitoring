Below table contains all access rules that need to be implemented by all parties involved in home monitoring.

# Definitions
The table uses the following definitions:
- CarePlan.subject The patient related to the resource.
- CarePlan.addresses[Condition].code The type of condition, like COPD.
- CarePlan.activity[ServiceRequest].code The type of service, like Home monitoring.
- Resource, the resource type.

# ACL
|Condition.code|Request.code|Resource query|
|----------------|--------------|----------------|
| *              | *            | Patient?id=patient.id |
| 13645005 (COPD) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 840539006, 840533007, 840534001 (COVID) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 11687002 (Zwangerschapsdiabetes) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 84114007 (Hartfalen) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 195979001, 304527002, 389145006 (Astma) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 46635009, 1290118005 (Diabetes type 1) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 230690007 (Post-CVA) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 287500001 (Post-darm) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 49436004 (Atriumfibrilleren) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 16114001 (Enkelfractuur) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 125605004 (VFC) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 408403008 (Geboortezorg) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 11687002 (Perioperatief) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 410942007 (Sys. therapie) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 431855005 (Chr. nierschade) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 38341003 (Hypertensie) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 239873007, 239872002 (Knie/heup-atrose) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 64766004 (IBD) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
| 254637007 (Longkanker) | 719858009 (Telehealth monitoring) | Condition?subject=patient&category=[alle somatische aandoeningen] |
||||
