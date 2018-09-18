---
layout: post
title:  "Unification: Data liquidity protocol"
date:   2018-09-17
categories:  
image: /images/unification0.png
projecturl: https://unification.com/
---
***Note: I am an advisor for Unification.***

> Unification is a decoupled architectural framework that provides generalized state channels for data standardization and interoperability across enterprise tech stacks.

In other words, Unification is a framework that companies can use to quickly standardize and commercialize their existing databases. It uses blockchain only for settlement and metadata, while data transfers are done off-chain.

There are 3 types of users: **Data Providers** (apps/enterprise), **End Users** (you and me), and **Data Consumers** (researchers/advertisers/enterprise).

## Token metrics

**Hard Cap**: 18,000,000 USD  
**Token supply sold**: 25%  
**Go-to-market and liquidity**: 10%  
**Founding Team**: 12%  
**Future Team**: 8%  
**Advisory**: 5%  
**Community Distribution**: 5%  
**Ecosystem Development**: 35%

A **total** of **1,000,000,000** tokens are generated and **250,000,000** are **sold** during the event. The pricing of the tokens is **$0.075 per UND**.

**Team Lockup** is **3 years** vested quarterly. **Advisor lockup** is **1 or 2 years** vested quarterly.

**Current Private Round**: Private - 35,000 ETH - No Bonus - 50% released at TGE, 25% 3m, 25% 6m

## Market opportunity/Competitive analysis

To me, Unification to data is what 0x is to tokens. While 0x provides a protocol for sharing liquidity between many off-chain order books, Unification provides a protocol for sharing standardized data between many off-chain databases (eg. heartrate data can come from multiple sources). 

[Ocean Protocol](https://oceanprotocol.com/) ("A decentralized data exchange protocol to unlock data for AI"): Very similar feature set, but Ocean has its own blockchain. Ocean also allows data consumers to bring AI models to the data to generate the results without needing to see the data. However, Ocean does not offer semi-automated data standardization, or efficient onboarding for enterprise, and does not give End Users control over their data. There is no framework for permissions and consent. Ocean has a partnership with the Singapore government, but no working product yet. Ocean tokenomics is based on a staked curation market ranked by availability and usage. From my understanding, Ocean Protocol's AI backend is actually SingularityNET.

The staking model of data in Ocean is not only for availability/transfer but also for the ranking/popularity of the datasets. Unification does not incentivize staking for ranking datasets, which aligns Data Producer and Data Consumer interests.

[Datum]( https://datum.org/): Data is stored on chain.

[Streamr](https://www.streamr.com/): Focused on real-time data.

## Team/Advisors/Partnerships
- **[Neyma Jahan](https://www.linkedin.com/in/neyma/)**, (Founder)

   - Founder/board member of SmartMat, CEO of WMaker Labs.

   - Bachelor's for Business/Managerial Economics UCDavis '98

     

- **[Paul Hodgson](https://www.linkedin.com/in/codegnosis/)**, (CTO and senior developer/architect) [GitHub](https://github.com/Codegnosis)

    - CTO SmartMat
    - Founder and Senior developer for Codegnosis — Data Warehouse/BI Consultant, Web and Mobile Application Developer, Neural Network developer
    - CTO @ youbundle, senior dev @ Blue Lotus, consultant at LexisNexis
        

- **[Maziar Sadri](https://www.linkedin.com/in/mazisadri/)**, (Products & Co founder)

    - Cofounder/software architect SmartMat
    - Managing Partner at Summit Consulting
    - Marketing Team Lead @ Yahoo
    - MBA Georgetown University '05



Neyma, Paul, and Maziar worked together on SmartMat, working on integrating Machine Learning and large scale data analysis.



- **[Larry Gandt](https://www.linkedin.com/in/larrygandt/)**, (Enterprise Sales & Business Development)
  - Director Sales at Ripple — responsible for aquisition of many high profile partnerships
  - Ripple Labs, Accuity, Thomson FInancial




- **[Shawn McLean](https://www.linkedin.com/in/stackcoder/)**, (Technical Architect) [GitHub](https://github.com/Inzidious)
    - CTO of Ankorus, Founder and Architect of IvIAnalytics
    - BS Comp Sci Wichita State Univ. '00




- **[Indika Piyasena](https://www.linkedin.com/in/indikap/)**, (Integration) [Github](https://github.com/indika)
    - MSc EE and CS at Univ. of Cape Town



- **[Farshad Niayesh](https://www.linkedin.com/in/farshad-niayesh-263972149/)**, (Machine Learning) [Github](https://github.com/FarshadNiayesh)
  - MS '19 Iowa State University in Data Analytics with a focus on fraud detection on Ethereum Blockchain using advanced Deep Learning.



- **[Erica Blair](https://www.linkedin.com/in/ericablairlive/)**, (Communications)
  - Founder and CEO of Blockchain Branding

  - BA Barnard '08

    


- **[Will Mekemson](https://www.linkedin.com/in/willmekemson/)**, (Outreach)
  - Founder of Crypto Market Management: Conducted consultation, market research, analysis, ICO review and investment services
  - BA Poli Sci Univ. of Iowa '07



- **[John Justus](https://www.linkedin.com/in/john-justus-73aaa515b/)**, (Research)
  - works on user acquisition and adaption of the Unification platform by the mass market




- **[Meera Blair](https://www.linkedin.com/in/marenblair/)**, (Operations)
- **[Ryan Getz](https://www.linkedin.com/in/ryangetz/)**, (Creative)

## Competitive Advantage

Ocean Protocol seems like the closest competitor in terms of features. Unification has the advantage of go-to-market speed due to being a protocol, not a blockchain. Unification also provides an SDK with extensive documentation to make onboarding much simpler and more feasible, and the advantage of giving End Users the control of where their data can go. Ocean Protocol's beta is planned to be released Q4 2018.

## Tokenomics and Token Utility

- Data Consumers pay tokens to obtain data from Data Providers and get permissions from End Users.
- Data Providers get another revenue stream by connecting their databases to the network.
- End Users get paid and get control over their data.
- Data Providers can also act as Data Consumers.
- The token acts as a medium where different data has individual market values, to facilitate data exchange. Eg. it's much harder to directly make a deal exchanging data from multiple entities than to value the data with a token on an exchange.

## Code

There are 4 major pieces to the project:

1. **Blockchain**: The blockchain is a store of metadata, including user permissions, data schemas, Data Provider prices, UApp validity (in the "Mother" smart contract), and data provider connection data. Unification is not building a new blockchain — it's a **blockchain agnostic** protocol so as long as the smart contracts can be ported, it should work. 
2. **[Haiku](https://github.com/unification-com/haiku) Server Node Software**: Data Providers need to install this and deploy corresponding smart contracts to provide the connection between existing databases and the Unification network.
3. **[Haiku](https://github.com/unification-com/haiku) Client Software**: Data Consumers need to install this and deploy corresponding smart contracts to provide the connection between scripts and the Unification network.
4. **[Babel App](https://github.com/unification-com/babel)**: End Users and Data Consumers use this app as a wallet, keystore, and frontend for the UApp store. It can also be used by Data Consumers to initiate data transfers, and End Users to modify permissions.

----

There are 5 repos, some public some private.

![image-20180907012621354]({{site.baseurl}}/images/unification1.png)

----

**[haiku-core](https://github.com/unification-com/haiku-core)**: Private repo where most of the current active development is occuring. 

Contains the Haiku prototype code, smart contracts, as well as the ML algorithms research/development. This repo contains the daily commits, with stable PRs/Merges being pushed to following repos.

---

**[haiku-node-prototype](https://github.com/unification-com/haiku-node-prototype)** (Python, 593 commits, started Feb 25, 2018): This is the proof of concept.

There is a note stating the following:

>  This is a Prototype/Proof of Concept, and is not the final, C++ production code. The prototype has been written in Python to enable the rapid development and testing of new features and concepts, and to refine the Unification Haiku Node specification.

![image-20180907013233645]({{site.baseurl}}/images/unification2.png)

The readme has a link leading to a wiki, which contains 

1. [Instructions on how to install prerequisites](https://github.com/unification-com/haiku-node-prototype/wiki/Installing-Prerequisites) 
2. [an overview](https://github.com/unification-com/haiku-node-prototype/wiki/Interacting-with-the-demo) of all the pieces of the system.
3. [how to interact with the system](https://github.com/unification-com/haiku-node-prototype/wiki/Interacting-with-the-demo)
4. [full demo workflow](https://github.com/unification-com/haiku-node-prototype/wiki/Full-Demo-Scenario)
5. [modifying config for advanced usage](https://github.com/unification-com/haiku-node-prototype/wiki/Modifying-demo_config.json)

I like the amount of documentation for developers to get familiar with all the moving parts of the system — this is super important for gaining a non-speculator community.

The code in `/Docker` and `/bin` show that the bulk of the business logic is in `/haiku_node`, where `haiku` starts from [main.py](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/main.py), `mother` starts from [mother/cli.py](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/mother/cli.py), and `babel` starts from [babel/cli.py](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/babel/cli.py).

#### Entrypoints

**[babel](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/babel/cli.py)**: functions for users to to [display application permissions](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/babel/cli.py#L26-L59), [list data sources](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/babel/cli.py#L62-L90), [grant or revoke data access](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/babel/cli.py#L93-L147), [get UND balance](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/babel/cli.py#L150-L166), and [transfer UND](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/babel/cli.py#L169-L223). 

**[mother](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/mother/cli.py)**: functions to [validate](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/mother/cli.py#L73-L95), [invalidate](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/mother/cli.py#L98-L120), and [list UApps based on validity](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/mother/cli.py#L98-L120). 

**[haiku](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/main.py)**: [starts and serves an RPC server](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/main.py#L26-L32), and implements functions to [fetch encrypted data from a data provider](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/main.py#L76-L139) and [decrypt it](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/main.py#L110-L139). This contains both Haiku Server and Haiku Client (client.py contains more client implementation). There is also [a basic UApp Store implementation](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/main.py#L164), which is an additional method (in addition to "Fetch") to initiating a data exchange.

#### Other interesting files and notes

[rpc.py](https://github.com/unification-com/haiku-node-prototype/blob/786702197ad2f287c437959b46e31da5c159117f/haiku_node/rpc.py): This file works between the `haiku` executable and the Data Provider's data. For the proof of concept, [UnificationDataFactory](https://github.com/unification-com/haiku-node-prototype/blob/master/haiku_node/data/factory.py) looks like it only reads from a sqlite3 database. The team tells me this previously supported ODBC but was was migrated to sqlite3 for unit testing purposes, and will eventually support any ODBC connection in the future.

There are several other helper files in the repo, including those for interacting with the blockchain, encryption, and checking whether a UApp is valid.

----

**[smart-contracts](https://github.com/unification-com/smart-contracts)**: Smart contracts for the prototype.

![image-20180907030236898]({{site.baseurl}}/images/unification3.png)

[eosio.token/eosio.token.cpp](https://github.com/unification-com/smart-contracts/blob/master/eosio.token/eosio.token.cpp): UND token for the EOS version on the protocol. Pretty self explanatory.

[unification_uapp/unification_uapp.cpp](https://github.com/unification-com/smart-contracts/blob/master/unification_uapp/unification_uapp.cpp): Smart contract that defines user controlled access to data. The functions in this smart contract are pretty self explanatory from their names — `modifyperm`(modify permissions), `modifypermsg`, `addschema` (add data schema), `editschema`, `setvers` (set version), `setschedule` (set daily, weekly, or monthly schedule), `setpricesch`, `setpriceadh` (set adhoc price), `setschema`, `initreq` (initialize request), `updatereq`, and `setrsakey` (set RSA encryption key for the data).

[unification_mother/unification_mother.cpp](https://github.com/unification-com/smart-contracts/tree/master/unification_mother/unification_mother.cpp): Unification Mother contract. Has functions to register, validate, and invalidate UApps to the registry, as well as checking for UApp validity and reading the UApp registry data.

----

**[babel](https://github.com/unification-com/babel)** (Angular webapp, 62 commits, started June 24, 2018): Web version of the Babel app.

![image-20180907043939773]({{site.baseurl}}/images/unification4.png)

This is a pretty standard Angular web app. It starts at [`public/scripts/app.js`](https://github.com/unification-com/babel/blob/master/public/scripts/app.js) with a router and renders all the views in [`public/views`](https://github.com/unification-com/babel/tree/master/public/views).

----

**[haiku](https://github.com/unification-com/haiku)** (C++, 8 commits, started June 17, 2018): C++ version of functionality in the [haiku-node-prototype](https://github.com/unification-com/haiku-node-prototype) repo.

This repo is where the C++ production version will live. While the Python-based prototype is in very active development, the C++ version is still reasonably early since Python is much quicker and easier to prototype with.

---

**[whitepaper](https://github.com/unification-com/whitepaper)**: Public repo which contains the latest published PDF of the tech whitepaper

## Conclusion

Unification is currently in the stage of fleshing out their testnet, and just starting on the C++ port for the mainnet. It looks like they're getting all features prototyped and tested in the Python version before porting it to C++, which is something I do often for my personal projects as well.

There doesn't seem to be any competitors with the same amount of depth in building and testing the entire system (including onboarding tools). As an advisor, I also get to see the team's technical conversations every day in Slack — it goes much much deeper than the whitepaper. I'm comfortable with the tech.

~~What I'm waiting for currently is actually on the business side. It would be great to see some pilot programs and/or MOUs with more known companies that can play the roles of Data Provider and Data User. Not only would this be great to show traction, but it'd also help the team smooth out the onboarding process as well as test with real data and demand.~~ (updates below)

Regarding this last point, Unification recently added Larry Gandt from Ripple to lead business development. Regardless of my opinions about Ripple, there's no denying the quality of their enterprise partnerships. Looking forward to seeing similar level partnerships soon.

_Update Sept 18: Unification has signed up partners in various industries including HintChain with 8.5M users and a few other companies. Additionally, there are some in the public sector which I'm really excited about but can not yet disclose._

## Other Info

Here are some interesting things that I've seen the team research:

- Raw data is typically not super useful — data needs to be preprocessed. Machine Learning can be utilized for Ingestion and Processing, on which the team is publishing a series of articles: [https://medium.com/unificationfoundation/how-unification-standardizes-data-with-artificial-intelligence-machine-learning-b13b6c04bb76](https://medium.com/unificationfoundation/how-unification-standardizes-data-with-artificial-intelligence-machine-learning-b13b6c04bb76)
- Mappings between datasets and consumer needs vary widely. Therefore, it is not possible for reputation staking and rewards/punishment system to optimize to a single mapping. Unification is researching ML to optimize mappings instead of using ineffective tokenomics, and building a predictive model on which dataset fits best based on consumer needs.
- Popularity of a data source is not a reliable performance measure.



