# MPSC U-22070: Consumers Energy discovery responses

This repository holds discovery responses served by **Consumers Energy Company** in Michigan
Public Service Commission **Case No. U-22070**, Consumers' electric general rate case. Almost all
are responses to requests from **Urban Core Collective (UCC)**; one is a response to an MPSC Staff
request. The files are republished as served, organised by request set, so that work citing them
can be checked against the source. The repository holds the responses and this README only.

- **49 files:** 44 workbooks and 5 response PDFs.
- **As served.** Every workbook, and every PDF but two, is byte-identical to the file as served,
  including its embedded metadata. The two exceptions are published with some pages removed (see
  [Pages removed](#pages-removed)).
- **Filenames are exactly as served,** spaces included.

The case docket is <https://efile.mpsc.state.mi.us/efile/viewcase.php?casenum=22070>.

## Contents

- [Layout](#layout)
- [Response numbers and question numbers](#response-numbers-and-question-numbers)
- [UCC 1st request](#ucc-1st-request-ucc_request_1)
- [UCC 3rd request](#ucc-3rd-request-ucc_request_3)
- [UCC 5th request](#ucc-5th-request-ucc_request_5)
- [Staff request](#staff-request-staff_request)
- [Answers inside the response PDFs](#answers-inside-the-response-pdfs)
- [Known issues in the served data](#known-issues-in-the-served-data)
- [Pages removed](#pages-removed)
- [Not in this repository](#not-in-this-repository)

## Layout

```
├── ucc_request_1/                     UCC 1st request: workbooks
│   └── superseded_incorrect_geoids/   original serves with invalid tract IDs, kept for audit
├── ucc_request_3/                     UCC 3rd request: workbooks and response PDFs
├── ucc_request_5/                     UCC 5th request: workbooks and response PDFs
└── staff_request/                     MPSC Staff request: SA-CE-184
```

## Response numbers and question numbers

Consumers numbers each response sequentially across the case. Within a UCC request set, the
response number is the question number plus a fixed offset:

| Request set | Folder | Response number | Example |
|---|---|---|---|
| UCC 1st | `ucc_request_1/` | question + 89 | 0090 answers Q1 |
| UCC 3rd | `ucc_request_3/` | question + 422 | 0424 answers Q2 |
| UCC 5th | `ucc_request_5/` | question + 889 | 0891 answers Q2 |

Question numbers restart in each request set, so 0091 (1st request, Q2) and 0891 (5th request,
Q2) answer different questions. Column-name suffixes inside a workbook do not always match the
question number. Where a workbook has a first sheet named `Discovery Question N`, that sheet
holds the question text.

Five 5th-request answers cite their attachments under other numbers: 0859 is served as 0892,
0865 as 0898, 0866 as 0899, 0867 as 0900 and 0868 as 0901.

**Status** in the tables below:
- `current`: the file to use.
- `superseded`: replaced by a later serve and kept for audit only.
- `narrative`: a PDF of questions and answers in text.
- `reference`: not analytical data.

**Served** is the cover-letter date where one was served with the file. Otherwise it is blank.

## UCC 1st request (`ucc_request_1/`)

| File | Response | Q | Witness | Served | Topic | Geography | Frequency | Period | Notes |
|---|---|---|---|---|---|---|---|---|---|
| `U22070-UCC-CE-0090_Gast_Att_1.xlsx` | 0090 | 1 | Gast |  | Residential consumption, average bill, customer counts, 60+ day arrears | zip | monthly | 2019-01 to 2026 (arrears from 2020-11) |  |
| `U22070-UCC-CE-0091_Gast_Att_1.xlsx` | 0091 | 2 | Gast |  | Same measures as 0090 | census tract | monthly | 2019-01 to 2026 (arrears from 2020-11) | superseded. Tract IDs have leading zeros stripped; not valid GEOIDs |
| `U22070-UCC-CE-0092_Gast_Att_1.xlsx` | 0092 | 3 | Gast |  | Shutoff protections (winter, senior, medical, veterans, extreme weather, other) | zip (medical: territory) | monthly | 2019-01 to 2026-07 | Q3(b) not answered as asked |
| `U22070-UCC-CE-0093_Gast_Att_1.xlsx` | 0093 | 4 | Gast |  | Same protections as 0092 | census tract (medical: territory) | monthly | 2019-01 to 2026-07 | superseded. Tract IDs are not valid GEOIDs |
| `U22070-UCC-CE-0094_Gast_Att_1.xlsx` | 0094 | 5 | Gast |  | Shutoff notices, shutoffs (all, low-income, senior), customers, shutoff duration | zip | monthly | 2019-01 to 2026-07 |  |
| `U22070-UCC-CE-0095_Gast_Att_1 UPDATED.xlsx` | 0095 | 6 | Gast |  | Same measures as 0094 | census tract | monthly | 2019-01 to 2026-08 | Re-serve with 11-digit GEOIDs; replaces the original in superseded_incorrect_geoids/ |
| `U22070-UCC-CE-0096_Gast_Att_1.xlsx` | 0096 | 7 | Gast |  | Customers by number of shutoff notices received | zip | monthly | 2019-01 to 2026-07 | Sheet d has no zip column |
| `U22070-UCC-CE-0097_Gast_Att_1 UPDATED.xlsx` | 0097 | 8 | Gast |  | Same distribution as 0096 | census tract | monthly | 2019-01 to 2026-08 | Re-serve with 11-digit GEOIDs |
| `U22070-UCC-CE-0098_Gast_Att_1.xlsx` | 0098 | 9 | Gast |  | Customers by number of shutoffs experienced | zip | monthly | 2019-01 to 2026-07 |  |
| `U22070-UCC-CE-0099_Gast_Att_1 UPDATED.xlsx` | 0099 | 10 | Gast |  | Same distribution as 0098 | census tract | monthly | 2019-01 to 2026-08 | Re-serve with 11-digit GEOIDs, received without a transmittal; six long sheets consolidated into one wide sheet a-f |
| `U22070-UCC-CE-0100_Gast_Att_1.xlsx` | 0100 | 11 | Gast |  | Shutoff duration bands (<24h to >672h) | zip | monthly | 2019-01 to 2026-07 | Question asked for low-income customers; served for all residential customers |
| `U22070-UCC-CE-0101_Gast_Att_1 UPDATED.xlsx` | 0101 | 12 | Gast |  | Same duration bands as 0100 | census tract | monthly | 2019-01 to 2026-08 | Re-serve with 11-digit GEOIDs |
| `U22070-UCC-CE-0103_Duke_ATT_1 (Outage Duration).xlsx` | 0103 | 14 | Duke |  | System customer-hours of outage | system | monthly | 2019-01 to 2026 |  |
| `U22070-UCC-CE-0107_Gast_Att_1.xlsx` | 0107 | 18 | Gast |  | Low-income profile: counts, cost per kWh, late fees, EWR outreach and savings | zip | annual and monthly | 2019 to 2026 | UCC-CE-0902 says total_res_ca_count double counts and should have been excluded |
| `U22070-UCC-CE-0108_Gast_Att_1 UPDATED.xlsx` | 0108 | 19 | Gast |  | Same profile as 0107 | census tract | annual and monthly | 2019 to 2026 | Re-serve with 11-digit GEOIDs; sheets j/k corrected by UCC-CE-0898; sub-parts g/h/i answered by UCC-CE-0894 |
| `U22070-UCC-CE-0109_Gast_Att_1.xlsx` | 0109 | 20 | Gast |  | Additional deposits and reconnection fees paid | zip | annual | 2019 to 2026 |  |
| `U22070-UCC-CE-0110_Gast_Att_1 UPDATED.xlsx` | 0110 | 21 | Gast |  | Same as 0109 | census tract | annual | 2019 to 2026 | Re-serve with 11-digit GEOIDs |
| `U22070-UCC-CE-0115_Gast_Att_1.xlsx` | 0115 | 26 | Gast |  | Residential Senior Credit and Residential Income Assistance enrollment | system | monthly | 2019-01 to 2026-06 |  |
| `U22070-UCC-CE-0126_Gast_Att_1.xlsx` | 0126 | 37 |  |  | Community engagement event tracker (108 events) | county | event | 2026-01 to 2026-07 | No question sheet in the workbook |
| `U22070-UCC-CE-0133_Gast_Att_1.xlsx` | 0133 | 44 | Gast |  | Commercial and industrial customers, arrears aging, shutoffs, fees | system | monthly | 2019-01 to 2026 (arrears from 2020-11) |  |

### Superseded originals (`ucc_request_1/superseded_incorrect_geoids/`)

**Do not use these for analysis.** These are Consumers' original serves of six census-tract
responses. Their tract identifiers are not valid 11-digit Census GEOIDs (2-digit state + 3-digit
county + 6-digit tract). Each was re-served with valid GEOIDs as the `UPDATED` file of the same
number in `ucc_request_1/`. They sit in their own folder because their names would otherwise
collide with the re-serves.

| Original (this folder) | Replaced by (`ucc_request_1/`) |
|---|---|
| `U22070-UCC-CE-0095_Gast_Att_1.xlsx` | `U22070-UCC-CE-0095_Gast_Att_1 UPDATED.xlsx` |
| `U22070-UCC-CE-0097_Gast_Att_1.xlsx` | `U22070-UCC-CE-0097_Gast_Att_1 UPDATED.xlsx` |
| `U22070-UCC-CE-0099_Gast_Att_1.xlsx` | `U22070-UCC-CE-0099_Gast_Att_1 UPDATED.xlsx` |
| `U22070-UCC-CE-0101_Gast_Att_1.xlsx` | `U22070-UCC-CE-0101_Gast_Att_1 UPDATED.xlsx` |
| `U22070-UCC-CE-0108_Gast_Att_1.xlsx` | `U22070-UCC-CE-0108_Gast_Att_1 UPDATED.xlsx` |
| `U22070-UCC-CE-0110_Gast_Att_1.xlsx` | `U22070-UCC-CE-0110_Gast_Att_1 UPDATED.xlsx` |

A 6-digit tract code repeats across Michigan's 83 counties, so it cannot be joined to Census
geography without the county. A code with its leading zeros stripped cannot be padded back
reliably. The same defect affects 0091 and 0093, which stay in `ucc_request_1/` because they
were replaced under new numbers (0891 and 0893 in the 5th request).

## UCC 3rd request (`ucc_request_3/`)

| File | Response | Q | Witness | Served | Topic | Geography | Frequency | Period | Notes |
|---|---|---|---|---|---|---|---|---|---|
| `U22070-UCC-CE-0429_Att1.xlsx` | 0429 | 7 |  | 2026-08-17 | Electric customers by rate class (months as columns) | system | monthly | 2019-01 to 2026-06 |  |
| `U22070-UCC-CE-0436_Gast_Att_1.xlsx` | 0436 | 14 | Gast | 2026-08-17 | Protection-plan defaults (WPP, SPP, CARE, PIPP) | zip and census tract on one row; system for CARE/PIPP | monthly | 2019-01 to 2026-08 | Q14(e) not answered |
| `U22070-UCC-CE-0455_Gast_Att_1.xlsx` | 0455 | 33 | Gast | 2026-08-17 | Demand-response enrollment (ACPC, CPP, PTR) by income | system | monthly | 2019-01 to 2026-08 | Annual subtotal rows are interleaved with month rows |
| `U22070-UCC-CE-0463_Foster_ATT_3.xlsx` | 0463 | 41 | Foster | 2026-08-17 | Records-retention schedule |  |  |  | reference |
| `U22070-UCC3-CE-0423-0444, 0446-0460, and 0462-0472.pdf` | 0423-0472 | 1-50 | various | 2026-08-17 | The 3rd request and 46 answers (0445 and 0461 were served separately) |  |  |  | narrative. Some pages removed; see Pages removed |
| `U22070-UCC3-CE-0445.pdf` | 0445 | 23 |  | 2026-08-18 | Narrative answer: ASP/CO plan by tract |  |  |  | narrative |
| `U22070-UCC3-CE-0461.pdf` | 0461 | 39 |  | 2026-08-24 | Narrative answer: customers reconnected before the 2026 extreme-weather events |  |  |  | narrative |

## UCC 5th request (`ucc_request_5/`)

| File | Response | Q | Witness | Served | Topic | Geography | Frequency | Period | Notes |
|---|---|---|---|---|---|---|---|---|---|
| `U22070-UCC-CE-0891_Gast_Att_1.xlsx` | 0891 | 2 | Gast | 2026-09-18 | Re-serve of 0091 with valid GEOIDs | census tract | monthly | 2019-01 to 2026-07 (arrears from 2020-11) |  |
| `U22070-UCC-CE-0892_Gast_Att_1.xlsx` | 0892 | 3 | Gast | 2026-09-24 | Residential and low-income arrears, >60-day splits | census tract | monthly | 2020-11 to 2026-06 | 2025-05, 2026-01 and 2026-02 missing |
| `U22070-UCC-CE-0893_Gast_Att_1.xlsx` | 0893 | 4 | Gast | 2026-09-18 | Re-serve of 0093 with valid GEOIDs | census tract (medical, military: territory) | monthly | 2019-01 to 2026-07 |  |
| `U22070-UCC-CE-0894_Gast_Att_1.xlsx` | 0894 | 5 | Gast | 2026-09-18 | Payment plans and bill assistance by program (0108 sub-parts g/h/i) | census tract and zip, one sheet each | annual | 2023 to 2025 | 2023-2025 only |
| `U22070-UCC-CE-0895_Gast_Att_1.xlsx` | 0895 | 6 | Gast | 2026-09-18 | EWR participation and first-year and lifetime savings | census tract and zip, one sheet each | annual | 2019 to 2025 | Question asked for monthly data |
| `U22070-UCC-CE-0898_Gast_Att_1.xlsx` | 0898 | 9 | Gast | 2026-09-24 | Corrected late fees, all and low-income (replaces 0108 j/k) | census tract | annual | 2019 to 2026 |  |
| `U22070-UCC-CE-0899_Gast_Att_1.xlsx` | 0899 | 10 | Gast | 2026-09-24 | Deposit and reconnection-fee territory totals before and after suppression | system | annual | 2019 to 2025 |  |
| `U22070-UCC-CE-0900_Gast_Att_1.xlsx` | 0900 | 11 | Gast | 2026-09-24 | Customers who paid reconnection fees or deposits | zip | annual | 2019 to 2025 |  |
| `U22070-UCC-CE-0901_Gast_Att_1.xlsx` | 0901 | 12 | Gast | 2026-09-24 | Fee and deposit payers, distinct customers shut off, shutoff-count distribution | census tract | annual | 2019 to 2025 |  |
| `U22070-UCC-CE-0905_Duke_ATT_1.xlsx` | 0905 | 16 | Duke | 2026-09-18 | SAIDI/SAIFI of EJ-serving circuits against IEEE quartiles | distribution circuit | annual | 2019 to 2023 |  |
| `U22070-UCC-CE-0906_Duke_ATT_1.xlsx` | 0906 | 17 | Duke | 2026-09-18 | Reliability indices, 56 EJ tracts against matched non-EJ tracts | census tract | annual | 2019 to 2023 |  |
| `U22070-UCC-CE-0908_Partlan_Attachment_1.xlsx` | 0908 | 19 | Partlan | 2026-09-18 | Status of the 11 bridge-period VCRP projects | VCRP project | snapshot | 2026-09-17 |  |
| `U22070-UCC-CE-0912_Duke_ATT_1.xlsx` | 0912 | 23 | Duke | 2026-09-18 | Other projects on the VCRP circuits | VCRP project |  | bridge period and test year |  |
| `U22070-UCC5-CE-0890-0917 Batch 1.pdf` | 0890-0917 | 1-28 | various | 2026-09-18 | The 5th request and 19 answers |  |  |  | narrative. Some pages removed; see Pages removed |
| `U22070-UCC5-CE-0892, 0897-0902.pdf` | 0892, 0897-0902 | 3, 8-13 | various | 2026-09-24 | Cover letter and 7 answers |  |  |  | narrative |

## Staff request (`staff_request/`)

| File | Response | Q | Witness | Served | Topic | Geography | Frequency | Period | Notes |
|---|---|---|---|---|---|---|---|---|---|
| `U22070-SA-CE-184_Davis_ATT_1.xlsx` | SA-CE-184 |  | Davis |  | Hourly (8760) delivered load by cost-of-service class | system | hourly | 2025 | Delivered (loss-inclusive) energy, not billed |

## Answers inside the response PDFs

Each response PDF holds the questions and Consumers' written answers. Many answers have no
workbook and exist only in these PDFs. **Attachment** names the workbook in this repository that
an answer refers to, where there is one.

### `ucc_request_3/U22070-UCC3-CE-0423-0444, 0446-0460, and 0462-0472.pdf`

Served 2026-08-17. 46 answers.

| Response | Q | Witness | Topic | Attachment |
|---|---|---|---|---|
| 0423 | 1 | Gast | Census-tract data from the 1st request re-served with 11-digit GEOIDs | the `UPDATED` workbooks in `ucc_request_1/` |
| 0424 | 2 | Grondin | Monthly residential consumption percentiles, 2025; answered with twelve tables in the text |  |
| 0425 | 3 | Breuring | Customer counts by heating type, by tract; data not available |  |
| 0426 | 4 | Breuring | Consumption percentiles by heating type; data not available |  |
| 0427 | 5 | Davis | Daily residential peak demand, 2025; refers to SA-CE-184 | `staff_request/U22070-SA-CE-184_Davis_ATT_1.xlsx` |
| 0428 | 6 | Davis | Residential peak demand by percentile; not developed by the load study, refers to SA-CE-184 | `staff_request/U22070-SA-CE-184_Davis_ATT_1.xlsx` |
| 0429 | 7 | Breuring | Customers by rate schedule, by month | `U22070-UCC-CE-0429_Att1.xlsx` |
| 0430 | 8 | Davis | Hourly consumption by rate schedule; refers to SA-CE-184 | `staff_request/U22070-SA-CE-184_Davis_ATT_1.xlsx` |
| 0431 | 9 | Gast | Definitions of Dunning Levels and how customers are assigned to them |  |
| 0432 | 10 | Gast | Differences between Current and 9-Month Dunning Levels |  |
| 0433 | 11 | Gast | Risk levels used when assessing Dunning Levels |  |
| 0434 | 12 | Gast | Deposits, disconnection timing, protections and payment plans by Dunning Level |  |
| 0435 | 13 | Gast | How shutoff (SNP) and default amounts and dates are set; dunning procedures |  |
| 0436 | 14 | Gast | Defaults from WPP, SPP, CARE and PIPP, by month | `U22070-UCC-CE-0436_Gast_Att_1.xlsx` |
| 0437 | 15 | Gast | How customers enrol in the Shutoff Protection Plan |  |
| 0438 | 16 | Gast | How customers enrol in the Winter Protection Plan |  |
| 0439 | 17 | Gast | Causes of erroneous disconnections and how they are mitigated |  |
| 0440 | 18 | Gast | How erroneous disconnections are resolved |  |
| 0441 | 19 | Gast | Number of erroneous disconnections; annual counts for 2025 and 2026 only |  |
| 0442 | 20 | Gast | The SNAP acronym and staff guidance documents; partly objected to |  |
| 0443 | 21 | Gast | Dunning Procedure codes and their definitions |  |
| 0444 | 22 | Gast | ASP and CO plan acronyms and status codes |  |
| 0446 | 24 | Gast | Customer charges for ASP and CO plans |  |
| 0447 | 25 | Gast | Whether customers can be disconnected for ASP or CO plan charges |  |
| 0448 | 26 | Gast | Past-due balances and payment options for dual gas and electric customers |  |
| 0449 | 27 | Gast | Efforts on long-duration and repeated disconnections |  |
| 0450 | 28 | Gast | Flex Plan default rates by risk level; not recorded |  |
| 0451 | 29 | Gast | Why Critical Peak Pricing and Peak Time Rewards are no longer promoted |  |
| 0452 | 30 | Gast | Why CPP and PTR incentive payments are paused |  |
| 0453 | 31 | Gast | What enrolling customers are told about the paused incentives |  |
| 0454 | 32 | Gast | Average savings per kWh for CPP, PTR and AC Cycling |  |
| 0455 | 33 | Gast | Low-income share of CPP, PTR and AC Cycling participants, by month | `U22070-UCC-CE-0455_Gast_Att_1.xlsx` |
| 0456 | 34 | Gast | Enrolment caps for CPP, PTR and AC Cycling |  |
| 0457 | 35 | Gast | Consumption changes and savings per participant for CPP, PTR and AC Cycling |  |
| 0458 | 36 | Gast | Why AC Cycling is closed to new participants |  |
| 0459 | 37 | Gast | Metrics for the programs in responses 0135 and 0136 |  |
| 0460 | 38 | Gast | Contacting and reconnecting disconnected customers before extreme weather |  |
| 0462 | 40 | Foster | Share of records for digitization that are more than seven years old |  |
| 0464 | 42 | Foster | Frequency and volume of retrievals from the records centre |  |
| 0466 | 44 | Foster | Whether the $10 million digitization cost reflects vendor pricing |  |
| 0467 | 45 | Duke | Share of residential customers with smart meters; answered by zip in an attachment | not received |
| 0468 | 46 | Duke | Smart meter models deployed to residential customers |  |
| 0469 | 47 | Duke | Whether the meters can limit electricity to a set wattage |  |
| 0470 | 48 | Duke | Whether IT platforms can limit electricity to a set wattage |  |
| 0471 | 49 | Duke | Residential customers with and without smart meters |  |
| 0472 | 50 | Duke | Reasons residential customers do not have smart meters |  |

### `ucc_request_3/U22070-UCC3-CE-0445.pdf`

Served 2026-08-18. 1 answer.

| Response | Q | Witness | Topic | Attachment |
|---|---|---|---|---|
| 0445 | 23 | Gast | ASP and CO plan data by tract; largely not available, with ASP enrolment for 2019-2024 |  |

### `ucc_request_3/U22070-UCC3-CE-0461.pdf`

Served 2026-08-24. 1 answer.

| Response | Q | Witness | Topic | Attachment |
|---|---|---|---|---|
| 0461 | 39 | Gast | Disconnected customers reconnected before five 2026 extreme-weather periods |  |

### `ucc_request_5/U22070-UCC5-CE-0890-0917 Batch 1.pdf`

Served 2026-09-18. 19 answers.

| Response | Q | Witness | Topic | Attachment |
|---|---|---|---|---|
| 0890 | 1 | Gast | Whether the application will be amended for the withdrawn SAP/LMI capital |  |
| 0891 | 2 | Gast | Re-serve of 0091 with 11-digit GEOIDs | `U22070-UCC-CE-0891_Gast_Att_1.xlsx` |
| 0893 | 4 | Gast | Re-serve of 0093 with 11-digit GEOIDs | `U22070-UCC-CE-0893_Gast_Att_1.xlsx` |
| 0894 | 5 | Gast | 0108 sub-parts g, h and i (payment plans and bill assistance) by tract | `U22070-UCC-CE-0894_Gast_Att_1.xlsx` |
| 0895 | 6 | Gast | EWR savings per residential customer (0108 sheet m-o) | `U22070-UCC-CE-0895_Gast_Att_1.xlsx` |
| 0903 | 14 | Breuring | How the rate and class labels in 0429 map to SA-CE-184 |  |
| 0904 | 15 | Breuring | Whether ELE_RES in 0429 is the total residential customer count |  |
| 0905 | 16 | Duke | Data behind the EJ-circuit SAIDI comparison with IEEE quartiles (Exhibit A-95) | `U22070-UCC-CE-0905_Duke_ATT_1.xlsx` |
| 0906 | 17 | Duke | Data behind the EJ and matched non-EJ tract reliability comparison (Exhibit A-95) | `U22070-UCC-CE-0906_Duke_ATT_1.xlsx` |
| 0907 | 18 | Duke | Whether the EJ tract comparison will be repeated in future cases |  |
| 0908 | 19 | Partlan | Status and spending of the 11 bridge-period VCRP projects | `U22070-UCC-CE-0908_Partlan_Attachment_1.xlsx` |
| 0909 | 20 | Partlan | Completed bridge-period VCRP projects and post-completion SAIDI; none completed |  |
| 0910 | 21 | Partlan | Type of work in the 11 VCRP projects |  |
| 0911 | 22 | Partlan | Construction start dates and delays for bridge-period VCRP projects |  |
| 0912 | 23 | Duke | Other capital projects on the VCRP circuits | `U22070-UCC-CE-0912_Duke_ATT_1.xlsx` |
| 0914 | 25 | Duke | Year-by-year VCRP spending by category, 2026-2035 |  |
| 0915 | 26 | Partlan | How EJ-serving circuits are prioritised for VCRP investment |  |
| 0916 | 27 | Duke | The VCRP goal of second-quartile SAIDI for every EJ circuit |  |
| 0917 | 28 | Partlan | Selection criteria for the 15 test-year VCRP projects |  |

### `ucc_request_5/U22070-UCC5-CE-0892, 0897-0902.pdf`

Served 2026-09-24. 7 answers.

| Response | Q | Witness | Topic | Attachment |
|---|---|---|---|---|
| 0892 | 3 | Gast | Monthly residential and low-income arrears by tract | `U22070-UCC-CE-0892_Gast_Att_1.xlsx` (cited as 0859) |
| 0897 | 8 | Gast | What the count columns on 0108 sheets j and k measure |  |
| 0898 | 9 | Gast | Corrected late-fee values for 0108 sheets j and k | `U22070-UCC-CE-0898_Gast_Att_1.xlsx` (cited as 0865) |
| 0899 | 10 | Gast | Zip and tract totals of deposits and reconnection fees | `U22070-UCC-CE-0899_Gast_Att_1.xlsx` (cited as 0866) |
| 0900 | 11 | Gast | Customers who paid reconnection fees or deposits, by zip | `U22070-UCC-CE-0900_Gast_Att_1.xlsx` (cited as 0867) |
| 0901 | 12 | Gast | The same by tract, plus customers shut off | `U22070-UCC-CE-0901_Gast_Att_1.xlsx` (cited as 0868) |
| 0902 | 13 | Gast | Why the 0107 and 0094 customer counts differ |  |

## Known issues in the served data

These describe the files as served. They are not corrections.

- **Census-tract IDs in eight original serves are not valid GEOIDs.** Consumers re-served them
  with 11-digit GEOIDs:
  - 0095, 0097, 0099, 0101, 0108 and 0110 as `… UPDATED.xlsx`
  - 0091 and 0093 as 0891 and 0893
- **Some sub-questions were not answered as asked.**
  - 0092 Q3(b)
  - 0436 Q14(e)
  - 0100: asked for low-income customers; served for all residential customers
  - 0895: asked for monthly data; served annually
- **0107 and 0108 sub-parts `g`, `h` and `i` are hidden sheets holding only the question text.**
  0894 answers them for 2023–2025.
- **0108 sheets `j` and `k` (late fees) were corrected by 0898.** 0897 explains their count
  columns.
- **0107 `total_res_ca_count`.** In 0902, Consumers says this column double counts and should
  have been excluded.
- **Small cells are suppressed.** Per 0902, any locale with fewer than 15 customers is suppressed,
  and the rule is applied differently across data sources. Zeros and gaps in the distribution
  sheets (0096–0099) are suppression, not observed absences.
- **0892 (monthly tract arrears) runs 2020-11 to 2026-06** and lacks 2025-05, 2026-01 and 2026-02.
- **0429 has negative customer counts in October 2020** on some rate rows.
- **0455 interleaves annual subtotal rows with month rows.**
- **Some rows are hidden in Excel as served.** Any parser reads them, but a spreadsheet program
  does not display them unless you unhide them. They are not the result of an active filter.
  - 0093 `a` (87 rows) and `f` (91)
  - 0094 `f` (17,571)
  - 0107 `p` (16,220)
  - 0108 UPDATED `p` (44,047)
  - the superseded 0095 `f` (23,734) and 0108 `p` (22,034)
- **0905 carries a cached external-link table** (feeder-level SAIDI/SAIFI), as served.
- **SA-CE-184 is delivered energy** ("At delivery level"), not billed sales.
- **0424's monthly consumption percentiles were served only as tables in the answer text** (UCC3
  PDF). The column header reads "AVG KWH", but each value is a percentile of that month's
  residential kWh distribution. The answer describes the values as sampled from the RSP
  population; it gives neither the sample size nor the sampling method.

## Pages removed

Two response PDFs are published with some pages removed. Nothing else on the remaining pages
was changed.

- **`ucc_request_3/U22070-UCC3-CE-0423-0444, 0446-0460, and 0462-0472.pdf`**: published without served pp. 1, 15, 16, 17, 66 and 68; 69 of 75 pages remain. SHA-256 as served `4406cede19c1b7149282be839f9dffc96c2862eecc2e10b2fd07a14ec71d0aea`, as published `6610ad70a58fd3a68bebe7dabd0d6e01d0cd1cbb58fc8004e7f81e647424a691`.
- **`ucc_request_5/U22070-UCC5-CE-0890-0917 Batch 1.pdf`**: published without served pp. 1 and 27; 29 of 31 pages remain. SHA-256 as served `1bebd804a1abb87fc8931793c5883cb0ef06f8b5f9b613279e223d22b32a6191`, as published `d59b3d9188f2ef7b99ae2c0f3421878c9a3f518480e6c51ed8cfba9816884d84`.

## Not in this repository

- **0467 Attachment 1** (smart-meter share by zip): cited in the 0467 and 0471 answers, but not
  received.
- **0896** (5th request, Q7): not yet answered when this repository was assembled.
- **The proofs of service** filed with each batch: they list the case's service contacts and
  are not responses.
