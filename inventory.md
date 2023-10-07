## Response Schema Inventory
| Name | Scope | Endpoint | Permalink | 
| -- | -- | -- | -- |
| API Description (Landing) | Root | https://data.naturalsciences.org/api | [api-landing-response.schema.json](https://github.com/ben-norton/informatics-api-response-schemas/blob/ad75f33f07fe1922ae1532c9ffc92d1bd0405be9/schemas/descriptive/api-landing-response.schema.json)|
| Data Products Description | Class | https://data.naturalsciences.org/api/v2/data-products | [data-products-response.schema.json](https://github.com/ben-norton/informatics-api-response-schemas/blob/da058784ccd66ba3885834c9fe23e5f81082fae1/schemas/data-products/data-products-response.schema.json) |
| Checklists Description | Resource Type  | https://data.naturalsciences.org/api/v2/data-products/checklists | [checklists-response.schema.json](https://github.com/ben-norton/informatics-api-response-schemas/blob/da058784ccd66ba3885834c9fe23e5f81082fae1/schemas/data-products/checklists-response.schema.json) |
| Mammal Diversity Database | Resource | https://data.naturalsciences.org/api/v2/data-products/checklists/mdd | [mdd-response.schema.json](https://github.com/ben-norton/informatics-api-response-schemas/blob/da058784ccd66ba3885834c9fe23e5f81082fae1/schemas/data-products/mdd-response.schema.json) |
| 422 Error | Root (Global) | https://data.naturalsciences.org/api/v2/vocabularies/term (example) | [422-error-response.schema.json](https://github.com/ben-norton/informatics-api-response-schemas/blob/da058784ccd66ba3885834c9fe23e5f81082fae1/schemas/metadata/422-error-response.schema.json) |
| Vocabulary* | Class | https://data.naturalsciences.org/api/v2/vocabularies | [vocabularies.schema.json](https://github.com/ben-norton/informatics-api-response-schemas/blob/da058784ccd66ba3885834c9fe23e5f81082fae1/schemas/vocabularies/vocabularies.schema.json) |
| Term Collection | Resource Collection ** | https://data.naturalsciences.org/api/v2/vocabularies/terms | [vocabulary-term-collection.schema.json](https://github.com/ben-norton/informatics-api-response-schemas/blob/da058784ccd66ba3885834c9fe23e5f81082fae1/schemas/vocabularies/vocabulary-terms-collection.schema.json) |
| Term | Resource | https://data.naturalsciences.org/api/v2/vocabularies/term?guid=[guid] | [vocabulary-term.schema.json](https://github.com/ben-norton/informatics-api-response-schemas/blob/da058784ccd66ba3885834c9fe23e5f81082fae1/schemas/vocabularies/vocabulary-term.schema.json) |

* Also referred to as data dictionaries in specific contexts

### Relationships
Resources are instances of Resource Types
Each Research belongs to a Resource Type
Each Resource Type belongs to a Class
--

Resources conditionally may belong to Resource Collections 
Condition: If a resource collection exists, then each associated resource belongs to the resource collection
Resource collections exist when a resource is not domain-specific. Example: The Mammals Diversity Database is a resource in the taxonomic checklists/bioinformatics domain. Therefore, the MDD does not belong to a Resource Collection. In contrast, terms are conceptually domain-agnostic. Therefore, the resource, term, is a member of the resource collection, term collection.






### Hierarchy
Root > (Resource) Class > Resource Type > Resource  
API > Data Products > Checklists > Mammal Diversity Database  
