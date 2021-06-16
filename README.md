# Uber and Lyft's State-Level Lobbying Spending

This repository contains data from our story, "[Uber and Lyft Donated to Community Groups Who Then Pushed the Companies’ Agenda](https://themarkup.org/news/2021/06/17/uber-and-lyft-donated-to-community-groups-who-then-pushed-the-companies-agenda)."

## Data

### State-Level Filings

```
filings
├── illinoisans_for_independent_work
│   ├── Illinois_Sunshine_Committee_Expenditures_Illinoisans_for_Independent_Work_2021-06-03.csv
│   └── Illinois_Sunshine_Committee_Receipts_Illinoisans_for_Independent_Work_2021-06-03.csv
├── new_yorkers_for_flexible_work
│   ├── CandidateCommitteeDisclosure(1).csv
│   └── CandidateCommitteeDisclosure.csv
├── new_yorkers_for_independent_work
│   ├── CandidateCommitteeDisclosure\ copy.csv
│   ├── CandidateCommitteeDisclosure(1)\ copy.csv
│   ├── CandidateCommitteeDisclosure(1).csv
│   ├── CandidateCommitteeDisclosure(2)\ copy.csv
│   ├── CandidateCommitteeDisclosure(2).csv
│   └── CandidateCommitteeDisclosure.csv
└── washingtonians_for_independent_work
    ├── Washingtonians\ for\ Independent\ Work,\ Sponsored\ by\ Lyft,\ Inc.,\ 2020(1).csv
    └── Washingtonians\ for\ Independent\ Work,\ Sponsored\ by\ Lyft,\ Inc.,\ 2020.csv
```

The [Illinoisans for Independent Work](https://www.documentcloud.org/documents/20891103-illinoisians-for-independent-work-statement-of-organization) data was sourced from the [Illinois Sunshine Database](https://illinoissunshine.org/committees/36024/).

Both the [New Yorkers For Flexible Work](https://api.www.documentcloud.org/files/documents/20891367/new-yorkers-for-flexible-work-registration.pdf) and [New Yorkers For Independent Work](https://s3.amazonaws.com/s3.documentcloud.org/documents/20891368/new-yorkers-for-independent-work-registration.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4JBBEJ7KWPNZQB7I%2F20210616%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20210616T015756Z&X-Amz-Expires=300&X-Amz-SignedHeaders=host&X-Amz-Signature=fca531cfb78bfe869ceef5589fd28468617472a234ff6f033e7518dfc64ee3e7) were sourced from the [New York State Board of Elections Campaign Finance System](https://publicreporting.elections.ny.gov/IndependentExpenditure/IndependentExpenditure). The filer ID for New Yorkers For Flexible Work is `15595`, the filer ID for New Yorkers for Indepedent Work is `21581`. 

The [Washingtonians for Independent Work](https://www.documentcloud.org/documents/20891369-washingtonians-for-independent-work-registration) data was sourced from the [Washington Public Disclosure Commission](https://www.pdc.wa.gov/browse/campaign-explorer/committee?filer_id=WASHI--965&election_year=2020).

The [Bay Staters for Independent Work](https://www.documentcloud.org/documents/20891102-bay-staters-for-independent-work-statement-of-organization) data was reviewed on the [Massachusetts Office of Campaign and Political Finance](https://www.ocpf.us/Filers?q=Bay%20Staters%20for%20Independent%20Work&cat=A#) website. Note that records show there was no financial activity from its statement of organization on 8/17/2020 to its dissolution on 10/6/2020.

### Community Group Donations

`donations.csv`

| **Column** | **Description** |
|------------|-----------------|
| **`Recieved By`**| The organization |
| **`Address`** | The address of the organization |
| **`Amount`** | The amount donated / Date donated on |
| **`Expended By`** | The organization that spent the money |
| **`Purpose/Beneficiary`** | The stated purpose of the expenditure |

This csvfile contains the organizations that recieved money from the Lyft PAC Illinoisans for Independent Work. The data is from a [quarterly report](https://api.www.documentcloud.org/files/documents/20891087/illinoisians-for-independent-work-d-2-quarterly-report-10-1-2020-to-12-31-2020.pdf) filed by the Illinoisians for Independent Work with the Illinois Board of Elections.

### Press Releases

`press-releases.csv`

| **Column** | **Description** |
|------------|-----------------|
| **`Article`** | The link to the article page |
| **`Article (Archived Link)`** | A mirrored version of the article link|
| **`Article (Screenshot)`** | The filename of the screenshot of the article, included in the repo|
| **`Article (Publish Date)`** | The publish date on the article|
| **`Press Release`** | The link to the original press release|
| **`Press Release (Archived Link)`** | A mirrored version of the press release|
| **`Press Release (Screenshot)`** | The filename of the screenshot of the press release, included in the repo|
| **`Press Release (Publish Date)`** | The publish date on the press release|
| **`Coalition`** | The state-level coalition that published the press release|

This csvfile contains articles published in local newspapers and the corresponding press releases found on the coalition pages.

### Coalition Website Posts

`coalition-posts.csv`

| **Column** | **Description** |
|------------|-----------------|
| **`state`** | The state the coalition is located |
| **`title`** | The title of the post |
| **`url`** | The url for the post |
| **`date`** | The date of the post |

This csvfile contains a list of posts found on the coalition websites as of 6/11/21.
