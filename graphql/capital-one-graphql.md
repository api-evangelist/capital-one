# Capital One GraphQL Schema

## Overview

Capital One is a financial services company offering credit cards, checking and savings accounts, loans, and auto financing in the United States. Through the Capital One DevExchange developer program, the bank publishes a catalog of production APIs secured with OAuth 2.0. This GraphQL schema represents a conceptual graph layer over those REST capabilities, covering accounts, transactions, rewards, credit, identity, and open banking.

## Provider

- **Name:** Capital One
- **Developer Portal:** https://developer.capitalone.com/
- **GitHub:** https://github.com/capitalone
- **Getting Started:** https://developer.capitalone.com/documentation/getting-started
- **OAuth 2.0:** https://developer.capitalone.com/documentation/o-auth
- **Sandbox:** https://developer.capitalone.com/documentation/sandbox

## Schema Design

The schema is organized around the core domains exposed by the Capital One DevExchange APIs:

### Account Domain

Account types model the full range of Capital One deposit and lending products. `Account` is the base interface; `CheckingAccount`, `SavingsAccount`, `CreditCard`, `AutoLoan`, `Mortgage`, and `PersonalLoan` implement it. Balance detail is split across `AccountBalance`, `AvailableBalance`, `PendingBalance`, and `StatementBalance` to reflect the layered nature of real-time versus posted balances.

### Transaction Domain

`Transaction` is the root event type. `TransactionDetail` carries enriched merchant and category data. Subtypes include `Purchase`, `Payment`, `Transfer`, `Zelle`, `WireTransfer`, `ACH`, `CheckDeposit`, and `StatementCredit`, matching the channel-level detail available through the Customer Transactions and Account Lookup APIs.

### Rewards Domain

`Reward` is the base reward object. `CashBack`, `Mile`, and `Points` extend it for the three main Capital One reward currencies. `RewardRedemption` records a redemption event. `Offer` and `OfferDetails` represent targeted promotions surfaced through the Credit Offers and Shop with Rewards APIs.

### Credit Domain

`CreditScore` and `FICOScore` carry score values and score factors. `CreditMonitor`, `CreditAlert`, and `IDProtection` model the monitoring and identity products (CreditWise). `SpendingLimit` and `CreditLimit` capture utilization controls on credit card accounts.

### Payment Domain

`AutoPay` configures recurring payments. `PaymentMethod` is the base for funding sources. `Card`, `CardDetails`, `CardLock`, and `VirtualCard` model card management including lock/unlock and virtual card issuance.

### Customer Domain

`Customer` and `CustomerProfile` hold identity and contact data. `Address`, `Contact`, and `Employer` capture structured personal data. `Joint` and `AuthorizedUser` represent multi-party account relationships.

### Notification and Document Domain

`Notification` and `Alert` model push and in-app alerts. `Statement` represents a billing period document. `TaxDocument` covers 1099 and other tax forms.

### Platform Domain

`APIKey` and `OAuthToken` represent developer credential objects. `Webhook` supports event-driven integrations. `Partnership` models third-party integrations via DevExchange. `OpenBanking` represents open banking data-sharing consents. `Nessie` references Capital One's open-source banking simulation API used for development and education. `DataTransparency` and `Privacy` represent consent and data-access records aligned with Capital One's privacy commitments.

## Authentication

All queries and mutations require OAuth 2.0 bearer tokens obtained through the Capital One DevExchange authorization server. Scopes control access to account, transaction, credit, and administrative data.

## References

- Account Lookup API: https://developer.capitalone.com/products/account-lookup?id=24064-1
- Authorizations API: https://developer.capitalone.com/products/authorizations?id=658618-1
- Credit Offers API: https://developer.capitalone.com/products/credit-offers?id=3105-3
- Customer Transactions: https://developer.capitalone.com/products/customer-transactions?id=3313-1
- Enhanced Decisioning Data API: https://developer.capitalone.com/products/enhanced-decisioning-data?id=23343-1
- Shop with Rewards API: https://developer.capitalone.com/products/shop-with-rewards?id=637511-1
- Partner Account Summary API: https://developer.capitalone.com/products/partner-account-summary?id=18757-1
- Real-Time Proactive Prescreen API: https://developer.capitalone.com/products/real-time-proactive-prescreen?id=320973-1
