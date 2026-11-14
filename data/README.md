# Data

The data used in this study was obtained from the Hospital Clínic de Barcelona. All information
originates from the hospital’s institutional data warehouse, which serves as a centralized repository
for clinical data.  

Access to the data was granted with the approval of the Comité de Ética de la Investigación con
Medicamentos (CEIm) of the Hospital Clínic de Barcelona. 

## Source files

The raw data consisted of 15 separate files, each with a different type of
clinical or administrative information.

| Event type | Content |
|------------|---------|
| Administration | Treatments given to patients: drugs administered, route of administration and amounts |
| Admission and discharge | Patient admissions and discharges, showing when patients enter and leave the hospital |
| Care level | Care levels assigned to patients throughout their episodes |
| Clinical records | Detailed clinical records and results, including tests and measurements taken during an episode |
| Demographic | Date of birth, sex and nationality |
| Diagnostic | Hospital discharge diagnoses (ICD-10-CM) and other diagnostic events |
| DRG | Diagnosis-Related Groups, which classify inpatients into categories with similar care processes and resource use; mainly used for billing and reimbursement |
| Encounter | Detailed records of patient encounters within the healthcare system |
| Episode | Start and end dates of each episode, a continuous period of care for a patient |
| Exitus | Patient deaths |
| Health issues | Patient health problems (coded in SNOMED CT) |
| Laboratory | Laboratory test results and details of the tests performed |
| Movement | Patient transfers between locations or care units |
| Perfusion | Infusion treatments (slow administration of fluids or drugs, typically intravenous) during an episode |
| Prescription | Prescribed drugs and dosages |

## Processed dataset

The 15 files were cleaned and merged into a single table using the patient
and episode identifiers, and new variables were derived (for example, age at
admission and episode duration). 