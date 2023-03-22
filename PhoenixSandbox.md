---
layout: default
title: Fusion Phoenix
nav_order: 3
---


# Fusion Phoenix Sandbox

## OVERVIEW
The Fusion Phoenix sandbox environment is available to developers registered on [FusionFabric.cloud](https://developer.fusionfabric.cloud/) platform to perform Fusion Phoenix API calls. Both Fusion Phoenix Product Integration API calls (SDK) and Fusion Phoenix US Core Banking API calls (BaaS) can be tested in this sandbox.  The environment is a fully capable product and therefore it is possible to execute and test real use cases and end-to-end scenarios.

The documentation on building Applications in the platform to access sandboxes is available here: [Get Started with FusionCreator.](https://developer.preprod.fusionfabric.cloud/documentation/get-started/index)

## SANDBOXES
The sandbox URLs are:

| Resource  | URL |
| ------------- | ------------- |
| Access Token  | [https://api.fusionfabric.cloud/login/v1/sandbox/oidc/token](https://api.fusionfabric.cloud/login/v1/sandbox/oidc/token)|
| Base BaaS  | [https://api.fusionfabric.cloud/retail-us/](https://api.fusionfabric.cloud/retail-us/)|
| Base SDK  | [https://api.fusionfabric.cloud/phoenix-sdk/](https://api.fusionfabric.cloud/phoenix-sdk/)|


Form an API resource URL by using the BaaS or SDK base URL plus the resource URL.

#### For example:


| API Type  | Resource  | URL |
| ------------- | ------------- | ------------- |
|BaaS|US Core Banking Customer<br/>(Retrieve Customer List of Accounts)| [https://api.fusionfabric.cloud/retail-us/customer/v1/customers/{customerId}/accounts](https://api.fusionfabric.cloud/retail-us/customer/v1/customers/{customerId}/accounts)|
|SDK| Fusion Phoenix Product Integration Customers<br/>(Create New Customer/Member Address) | [https://api.fusionfabric.cloud/phoenix-sdk/customer/v1/customers/{encId}/addresses](https://api.fusionfabric.cloud/phoenix-sdk/customer/v1/customers/{encId}/addresses)|

#### Sandbox Considerations:

- The generated token is only valid against the sandbox environment.
- The token will expire after a short period of time and will need to be renewed.
- The sandbox is shared by multiple FinTechs, please do not enter any confidential information. Note also that sandbox data/content may be erased by Finastra for a daily or weekly clean-up.

## Sandbox Data
Data in the grid below is available to be used in the sandbox environment.  Feel free to use it for your testing purposes.  In addition, the Postman collections available for downlowd from the FFDC API Reference cards can be imported into Postman and executed against the sandbox.  The data contained within them is actual Sandbox data.
> Note:

-  Fusion Phoenix Product Integration APIs (SDK) utilize the encId as the unique resource id.
-  Fusion Phoenix US Core Banking APIs (BaaS) utilize the customerId and accountId as the unique resource id.
-  When working with both SDK and BaaS APIs consider the customerId and customer encId as equal and interchangable values.
-  When working with both SDK and BaaS APIs consider the accountId and account encId as equal and interchangable values.

| Last Name | First Name | Title 1       | Title 2       | Account Type | Account Number | customerId/encId                                                                      | accountId/encId                                                                           |
| --------- | ---------- | ---------------- | ------------- | ------------ | -------------- | ------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| Prince    | Diana      | N/A              | N/A           | RIM          |                | ~ew0KICAicmltUmVjb3JkSWQiOiAiNzc3ODliZmUtNjJkYi00NDUxLTllODctZTI2NDYwYzcxNGFkIg0KfQ-- |                                                                                           |
| Prince    | Diana      | Diana Prince     | N/A           | IL           | 0070000742     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjk5ZmJlMjZkLTc4NTQtNDAwNi04MmY0LTQ5MmM1MDk4MDg0MH5MTiINCn0- |
| Prince    | Diana      | Diana Prince     | N/A           | ML           | 0010001048     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjVlOWEwMjFhLWI5ZGYtNDRjNS05MWMxLWVjMTcyM2Q1ZmQyZH5MTiINCn0- |
| Prince    | Diana      | Diana Prince     | N/A           | CK           | 0020028818     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogImI1NzUwMDljLTFkMmUtNGJiOS1hYjJkLWU1NmFmNTkyYTk5OX5EUCINCn0- |
| Prince    | Diana      | Diana Prince     | N/A           | SV           | 0040037096     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjczNGQ2OGM5LTFhNjEtNGNhYi05ODExLTA1MzVkMTM5M2JhMX5EUCINCn0- |
| Prince    | Diana      | Diana Prince     | N/A           | CD           | 0060305841     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjY2YzYyYzkzLTJkZGYtNDNjZS1hMWQxLTgyYjhhM2IzMDgxM35EUCINCn0- |
| Prince    | Diana      | Diana Prince     | N/A           | CD           | 0060305857     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjc4OTFlOTIzLWJjMTMtNDM1Ny04NGRkLWIyYjRlNGFiNTA2NH5EUCINCn0- |
| Lane      | Lois       | N/A              | N/A           | RIM          |                | ~ew0KICAicmltUmVjb3JkSWQiOiAiMWE2MGZmZmUtOTc0ZC00OTFkLWE1M2UtMjA3MmY5ZWU5ZjUyIg0KfQ-- |                                                                                           |
| Lane      | Lois       | Lois Lane        | N/A           | IL           | 0082000001     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogImU2YTY5YjFhLWFjMDMtNDEwOS1iZGFjLThmNzdhNjlkYzk3YX5MTiINCn0- |
| Wayne     | Bruce      | N/A              | N/A           | RIM          |                | ~ew0KICAicmltUmVjb3JkSWQiOiAiMGY0ZTkzMzUtMWRjNy00NmU1LWFmNDMtOTQzNTNkNTdmOGFiIg0KfQ-- |                                                                                           |
| Wayne     | Bruce      | Bruce Wayne      | N/A           | CK           | 0010023086     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjAxNjI1ZTRjLTgxZDMtNDk5OS1hZjFkLTNjY2M0ODhmN2YzYn5EUCINCn0- |
| Wayne     | Bruce      | Bruce Wayne      | N/A           | CK           | 0020026667     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogImU2M2Y1NDA4LTI5ODEtNGY0Ny05NmE4LTJmM2E4YmIwZGUzOX5EUCINCn0- |
| Wayne     | Bruce      | Bruce Wayne      | N/A           | LOC          | 0080000098     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogImIwZDc1Y2QwLWRiOTMtNGFiNy1hOWU2LTdjYjNiNmQ0OTkxNX5MTiINCn0- |
| Watson    | Mary Jane  | N/A              | N/A           | RIM          |                | ~ew0KICAicmltUmVjb3JkSWQiOiAiYjkwMjQ3NmMtNzI3MC00MTMwLThmODMtNWU1ZTcyNDkyZDAwIg0KfQ-- |                                                                                           |
| Watson    | Mary Jane  | Mary Jane Watson | N/A           | LOC          | 0080000019     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogImYwZmI1YzJhLWI5MWMtNDNjMy1hNTFjLWEzOTk5ZDJhODIwNX5MTiINCn0- |
| Watson    | Mary Jane  | Mary Jane Watson | N/A           | CK           | 0020024327     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjE1YjIzMjU2LWFjYTQtNDY1YS05OGI1LTQ2MTJmMGViZjIzNX5EUCINCn0- |
| Stark     | Tony       | N/A              | N/A           | RIM          |                | ~ew0KICAicmltUmVjb3JkSWQiOiAiNTIzMjQyYWUtYTZlYi00MzI1LThhZjQtZGQ5ZGJmNmIxNjE1Ig0KfQ-- |                                                                                           |
| Stark     | Tony       | Tony Stark       | N/A           | CK           | 0020025272     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjJiZTA2OTdmLWNiYmEtNGEwOS1iYTFhLWU4MjliZDk3OTgzMX5EUCINCn0- |
| Stark     | Tony       | Tony Stark       | N/A           | LOC          | 0080000066     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjQ2YTY3NTkxLTk4OTgtNDY5Yy1iNjdiLWQ2MzIyZDgzNzI0MX5MTiINCn0- |
| Parker    | Peter      | N/A              | N/A           | RIM          |                | ~ew0KICAicmltUmVjb3JkSWQiOiAiODA1YzkzZjAtYjNjMC00ZjM3LWJjZDItNDVhMWQ5NTEzNmI4Ig0KfQ-- |                                                                                           |
| Parker    | Peter      | Peter Parker     | N/A           | CK           | 0020024408     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjMyOGFhYWIyLWJlZDMtNGFjMS1hYTdmLWU5MjI0MTQ2OGQxY35EUCINCn0- |
| Parker    | Peter      | Peter Parker     | N/A           | LOC          | 0080000020     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjIyZTE0NzhkLWE5MmMtNDc5Ni1iMWY1LTAwNWI3OGFiYjMzOX5MTiINCn0- |
| Kent      | Clark      | N/A              | N/A           | RIM          |                | ~ew0KICAicmltUmVjb3JkSWQiOiAiMDJkMmExYTktMjNhMy00OTVkLWEyOGYtMGE5MWQ4NzM3ZTljIg0KfQ-- |                                                                                           |
| Kent      | Clark      | Clark Kent       | N/A           | CK           | 0020024975     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjdkNjQyN2E3LTBkZDQtNDY4Yy05MDQ4LTQyODljYjNhODJlNn5EUCINCn0- |
| Kent      | Clark      | Clark Kent       | N/A           | LOC          | 0080000029     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjU4ZDNiYjAzLTcxZGUtNDk2Yy1hN2Q1LTVhZTkwYmRmMmUzNn5MTiINCn0- |
| Lee       | Stan       | N/A              | N/A           | RIM          |                | ~ew0KICAicmltUmVjb3JkSWQiOiAiOTc2ZTM1YzktYTAyMy00MWY4LWExZTMtMDA1M2ZmNDE1MjJkIg0KfQ-- |                                                                                           |
| Lee       | Stan       | Stan Lee         | Steve  Rogers | CK           | 0020025596     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjEyNzU0NzJlLTFmZmMtNDVhYS05MTRkLWZjYzcxMTViZjUyYn5EUCINCn0- |
| Lee       | Stan       | Stan Lee         | Steve  Rogers | LOC          | 0080000065     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogIjg2N2IyZWFhLWYxYWEtNGQzNi05Yzc5LTQ5MjYwYWRlOGMxYn5MTiINCn0- |
| Rogers    | Steve      | N/A              | N/A           | RIM          |                | ~ew0KICAicmltUmVjb3JkSWQiOiAiZmM4ZGYzZTUtYzYyMi00NWU4LWI0YjQtMGJhMDA2ZDI5OGRiIg0KfQ-- |                                                                                           |
| Rogers    | Steve      | Steve Rogers     | N/A           | CK           | 0010022701     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogImFkOTcxYmE4LWIxYzgtNGQ3MC05Nzc5LTJkNDdhOGY4YjlhOX5EUCINCn0- |
| Kyle      | Selina     | N/A              | N/A           | RIM          |                | ~ew0KICAicmltUmVjb3JkSWQiOiAiN2I5NjMxM2UtYzk3ZC00NWMwLTgyYzgtMmMwYTgxYzNkMGQ1Ig0KfQ-- |                                                                                           |
| Kyle      | Selina     | Selina Kyle      | N/A           | CK           | 0020024885     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogImQ3ZGI0NjIwLWE3NGEtNDZmYy1iYzMzLWE5MTk3NGIyMDEyOX5EUCINCn0- |
| Kyle      | Selina     | Selina Kyle      | N/A           | LOC          | 0080000038     |                                                                                       | ~ew0KICAiYWNjdFJlY29yZElkIjogImQ3ZTNmMzBhLTEzOTQtNGMxOS1hZTA3LTg2NjE3YjI0MjgwMn5MTiINCn0- |