# OneGov Case - Financial Management & Budgeting

## Terms
- Functional group: functions grouped together in the software designed around commonly used positions in an org
- Supporting process: activity performed as part of business process
- Guidance question: questions to guide consultants to capture specific requirements as part of the implementation
- Executive information enquiry: reporting tools used to display and analyze key financial information

## Accelerated template
- Database including product, foundation, industry driven and common practice pre-configuration and documents designed to speed implementation in certain industry sector
- Type of configuration element:
	- Foundation: configuration element that should not be changed since they have a large impact on other parts of the template which might impact other elements. Example: chart of account design - should not be changed once designed
	- Industry regulation driven: industry specific template that governs elements within a template
	- Industry common practice: common elements of the industry that helps to form a template based on proven practice processes
	- Customer specific: specific configuration for a customer

## OneGov accelerated template
- Ships software and pre-configurated to accelerated implementation within the Federal Government specifically for this market

- **System admin**:
	- Areas around user accessibility in implementation:
		- Role based
		- Users and security mapping
		- Authorization and permissions
	- Considered to be customer specific since orgs have different policies regarding customer access

## Streams
- Logical grouping of Functional Groups within Templates designed to support key business areas through implementation phases
- **Financial management**: Made up of the following group:
	- General ledger: 
		- Forms the foundation of template config with the flexible chart of accounts design with multiple subsidiary ledger reporting to the general ledger/reporting components
		- One org (example TechOne) can have unlimited ledger with the same accounts chart
	- Chart of accounts: 
		- Tools with all financial accounts in the general ledger which provides information about financial transactions conducted during a set period, often includes unique ID, names and brief description
		- Easily manage and report financial information about org financial health
	- Asset accounting
	- Taxation
	- Banking
- **Revenue management**: 
	- Made up of the following functional groups:
		- Account receivable
		- Debt management
		- Enterprise cash receipting
	- Helps manage debtors and revenue items, including generation of charges and allocation of payment to invoices
	- Provide effective management with the help of automation for a streamline collection process with the help of enquiries and report to inform an org of the customer payment
- **Business strategy and planning**:
	- Enable orgs to connect budgets to drivers such as number of employees to gain insight into performance
	- Can be devolved throughout the business allowing for real-time analysis of the performance


# OneGov Case - Procure to pay (incl. Sourcing & Contract)

## Terms
- Procure to Pay: deals with goods acquirement process with the payment from the buyer to the supplier 
- Procurement: buying supplies - first step
- Sourcing: determining the best option to secure a resource from the market place
- Contract: legally binding agreement between two parties for providing services under terms
- Purchasing: buying the resources from the supplier and immediately/defer the payment to the supplier
- Tender: an invitation to potential suppliers to provide a quote for the requirements of resources
- Submission: formal response to the tender detailing how the requirements are met and at what cost

## Procure to pay
- Key process about the "purchasing resource" aspect of a business
- Other processes: order to cash (sales), contract to claim (contracts for both purchase and sale)
- Steps:
	- Requisition: identifies the need for an item to create an internal request and sent to approval before becoming a purchase order for a supplier
	- Purchase order: legally binding contract between both parties to deal. Once the supplier receives this order, it is processed as a sale order and to be schedule to be delivery. 
	- Receipt: If the conditions are met (i.e. The buyer receives the product in good condition), the buyer needs to confirm the request as a receipt
	- Invoice: The supplier sends the buyer agreed terms of payment, which outlines the payment amount and when to pay the amount
	- Payment: the buying org makes a bulk payment on the due date for the invoice, usually through ETFs

## P 2 P in Government
- Commonwealth Procurement Rules govern how the government buys good to ensure that both the government and taxpayer get value for their money
- DOF looks after this framework and assist the government through advise and services to get the best value
- Procurement is governed by legislative to get the best value for money and the DOF maintain the procurement framework with some laws and policies
- Government can have guides and tools for workers to be compliant with the rules
- Happens either through:
	- Open tender: publishes an open invitation to the public for all who meets the requirements to submit a tender
	- Limited tender: where potential suppliers are approached for invitation to submit a tender
- Determined by a procurement thresholds with other factors - example: if expected value of purchase is < 80 k then limited, if >= 80 k then open tender
- All transactions must be accurate and concisely documented for every procurement

## P 2 P in OneGov template
- The accelerated template has been set up to support the P 2 P process in compliance with regulations
- 5 key functional groups
	- Sourcing: manages approach to market and tendering process helping to publish open/limit tender to invite submissions, evaluate them and invite the successful submission, which can then be separated into contract or purchasing groups
	- Contract
	- Purchasing
	- Accounts payable: when receiving the goods under the contract/purchase order, payments are made
	- Reviews: performance of the supplier is reviewed to evaluate future tender submission from this submission

## OneGov design elements
### Sourcing
- Depends on 3 config:
	- System: defines sourcing processes and needing only one system
	- Process: defines the number of stages in the processes
	- Categorization: classifying goods/services in reporting
- 2 supporting processes:
	- Approaches to market: select the sourcing process to approach a market to make new purchases and gaining information about the goods to be procured
	- Tenderers: maintaining submitted tenders until one is selected

### Purchasing
- Key elements:
	- System: defines integration and custom fields apart from all location data
	- Location: locations for which the purchase is carried out, make up the structure for purchasing/managing
	- Catalogue: internally maintained list of products/services that an org purchase on a routine, while other purchases are ADHOC purchases with can be done with authorization
