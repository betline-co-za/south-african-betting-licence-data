# South African Betting Licence Data

Structured company and bookmaker licence information for locally licensed South African betting sites, maintained by Betline.co.za.

**Dataset last updated:** 08 November 2026

## About

This repository provides machine-readable information about locally licensed South African betting sites and the legal companies and bookmaker licences associated with them.

The dataset is maintained by Betline.co.za as part of its research and verification of betting sites operating under South African bookmaker licences.

## Dataset

The main dataset is available in:

`betting-sites.json`

Each betting site record can include:

- Betting site name
- Legal company name
- Company registration number
- Province
- Provincial gambling authority
- Bookmaker licence number
- Betline operator profile URL

The dataset records the main legal company identified for each betting site together with its associated bookmaker licence information.

A URL to the corresponding operator profile on Betline.co.za is provided for each betting site. The operator profile provides further information about the betting site, including information about the company and licence under which it operates.

## Scope

This dataset is limited to betting sites identified by Betline as operating under bookmaker licences issued by South African provincial gambling authorities.

Offshore betting sites that are not licensed by a South African provincial gambling authority are not included.

The dataset is intended to provide structured reference information about the main legal company and bookmaker licence associated with each listed betting site. It is not intended to provide a complete corporate record of every company associated with a betting brand.

## Data Structure

```json
{
  "bettingSite": "ExampleBet",
  "companies": [
    {
      "companyName": "Example Betting (Pty) Ltd",
      "companyRegistrationNumber": "2026/000000/07",
      "licences": [
        {
          "province": "Western Cape",
          "gamblingBoard": "Western Cape Gambling and Racing Board",
          "licenceNumber": "00000000-000"
        }
      ]
    }
  ],
  "betlineProfile": "https://betline.co.za/compare-betting-sites/examplebet/"
}
```

## Sources and Verification

Betline compiles and checks information using relevant South African regulatory and public sources.

Bookmaker licence information is checked against information published by South African provincial gambling authorities and the National Gambling Board's Verified Operators Portal.

Legal company names and company registration numbers are checked against records available through the Companies and Intellectual Property Commission (CIPC).

Licence number formats vary between provincial gambling authorities. In some regulatory records, the identifier used for a bookmaker may correspond with the legal entity's company registration number rather than a separate traditional licence number.

Information published by the betting site or legal entity may also be used when identifying the company and bookmaker licence associated with a betting site.

Licence, company and regulatory information can change. Information in this repository should therefore not be treated as a substitute for confirmation from the relevant South African gambling authority or CIPC.

## Betline Operator Profiles

Each record includes a `betlineProfile` URL linking to the corresponding operator profile on Betline.co.za.

These profiles provide additional information about individual betting sites beyond the structured company and licence information contained in this dataset.

## A Note from the Publisher

I maintain this public GitHub dataset as a courtesy to anyone interested in South African betting licence information. It is a separate reference resource and is not the same dataset used for other projects, tools or internal research.

Although I make every effort to keep the information accurate and up to date, this GitHub dataset is reviewed and updated periodically, not in real time.

Company details, bookmaker licences and regulatory information can change between updates. For this reason, anyone using or relying on this dataset should independently verify the information with the relevant provincial gambling authority, the National Gambling Board or CIPC before using it.

The information is provided in good faith as a public reference resource, but I cannot guarantee that every record will be accurate or current at the time it is accessed.

## Publisher

This dataset is maintained by [Betline.co.za](https://betline.co.za/), an independent South African betting information and comparison website founded and operated by Fanie Zevgolis.

Betline.co.za is operated under [ZEVGOSA](https://zevgosa.co.za/) and is a member of Proudly South African.

**Publisher:** Betline.co.za  
**Founder and operator:** [Fanie Zevgolis](https://www.linkedin.com/in/faniezevgolis/)  
**Operated under:** ZEVGOSA  
**Proudly South African:** [View membership certificate](https://zevgosa.co.za/wp-content/uploads/2026/04/zevgosa-proudly-south-african-certificate.pdf)  
**Country:** South Africa  

## Licence  

This dataset is licensed under the Creative Commons Attribution 4.0 International (CC BY 4.0) licence.  

When using or redistributing this dataset, attribution should be given to Betline.co.za as the source.  

See the [LICENSE](LICENSE) file for the full licence terms.
