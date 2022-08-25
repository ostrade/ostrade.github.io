# Welcome to Open Source Trading (ostrade)

Ostrade is an open source foundational set of APIs and services to allow companies engaged in trading to quickly build high value supporting applications.

## The Big Four of the Foundation
* **Instrument** - Definitions for the structures of trades
* **Counterparty** - Information on the legal entities for which transactions are executed
* **Trade** - Executed transactions between counterparties resulting in financial obligations
* **Market Data** - Prices for instruments including settlement data, real-time market data and derived curves 

## The Motivation

Trading organizations use mostly proprietary, bespoke ways to implement higher value functions. Most of these companies end up using commercial off-the-shelf software (COTS) in the form of vendor based energy trading risk management systems (ETRM) as a foundation for implementing these higher values functions. 

However, the bespoke nature of the details of the implementation results in highly customized, tightly coupled and expensive to maintain enhancements into and on top of the vendor application. These customizations can be very expensive to maintain as they usually result in extensive manual regression testing during any vendor platform updates, such as patches or version upgrades. 

The cost of regression testing and operational risks associated with updates create a natural organization aversion to updating vendor systems. The aversion can result in several unintended consequences to the organization. Not taking patches can result in an increased security threat. Additionally, it results in longer gaps in upgrades which in turn creates increased scope of change between updates. The increased scope of change actually increases the operational risk and overall costs with upgrading.

Because of these factors, the motivation of the ostrade project is to allow companies to have access to a generic, non-proprietary set of foundational building blocks for their trading systems and processes. The hypothesis being that the total cost of ownership for the system will be reduced along with other positive attributes such as the ability to source from a larger pool non-vendor-specific technical talent as well as retaining more of the actual trading and risk management business knowledge within this talent pool. The developers will know more about how the system actually works, rather than simply knowing how to interface with a block box.

The ultimate goal is to provide a point of collaboration using the open source model between trading companies to build and maintain these foundational tools which don't create any significant strategic advantage allowing them to break out of the vendor-driven implementations and reduce their total cost of ownership.

## Building on the Foundation

Using the foundational services and data structures provided by ostrade, the organization can quickly build their bespoke implementations. Here are some examples of the higher value services which can be produced. 

* **Position Management:** Aggregations of Trade data into groups
* **Profit and Loss:** Positions marked to latest settlement or market data
* **Market Risk:** Exposures combined with statistical measures calculated from settlement data
* **Credit Risk:** Trades by aggregated counterparty groupings combined with statistical measures calculated from settlement data