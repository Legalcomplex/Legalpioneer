# Data Dictionary for Legalpioneer Profiles Dataset

| Field Name       | Type     | Description                                                  | Format          | Notes                                                                                   |
|-------------------|----------|--------------------------------------------------------------|------------------|----------------------------------------------------------------------------------------|
| ID                | Integer   | Unique identifier for each company profile                    | `int`            | Must be unique across the dataset                                                       |
| Name              | String    | Official name of the company                                  | `string`         |                                                                                        |
| Description (Descr) | String    | Brief description of the company's activities and offerings     | `string`         |                                                                                        |
| Link              | URL       | Direct link to a public profile or website of the company          | `URI`            | Ensures accessibility and verifies the company's presence online                         |
| Profile           | URL    | Detailed information about the company, including history, mission, etc. | `string`         | Based on Crunchbase or Product Hunt                                |
| Linkedin          | URL       | Direct link to the company's LinkedIn profile                     | `URI`            | Provides additional insights into company operations and employee engagement             |
| Area   | String    | The market the company primarily focus on. What problem are the solving. This is the primary metric for aggregating market sizes | `string`         | Helps categorize companies by their workflow focus, currently we have 48 markets                                      |
| Industry    | String    | The industry sector that the company targets                       | `string`         | Values are LegalTech	Tax	RiskTech	CivicTech	Law                                     |
| Segment    | String    | The specific customer segment that the company targets           | `string`         | Focus on 'Legal Professionals' is Legal and GRC are 'Companies', 'Government', or 'Citizens'.     |
| Label | String | The type of technology or area the company specializes in, such as AI, Blockchain, ESG | `string`         | Indicates the focus of the company's products or services. This tag is algorithmically determined value                                    |
| Founded            | Date       | The date the company was officially established or domain was registered                 | `date`            | Format YYYY-MM-DD                                                                        |
| Stamp (Date)      | Date       | The date of the profile's last update or verification              | `date`            | Format YYYY-MM-DD                                                                        |
| City               | String    | The city where the company is headquartered or primarily operates  | `string`         |                                                                                        |
| Country             | String    | The country where the company is headquartered or primarily operates | `string`         | ISO country code recommended (e.g., 'US' for the United States)                              |
| Employee      | Integer   | Total number of employees working for the company                | `int`            | Includes full-time, part-time, and contract workers                                        |
| Raised   | Currency   | Total amount of funds raised in USD by the company through investments, debt, or grants | `decimal`        | Include details on funding rounds                                   |
