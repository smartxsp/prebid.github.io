---
layout: bidder
title: viqeo
description: Prebid Outstream Viqeo Bidder Adaptor
biddercode: viqeo
pbjs: true
floors_supported: true
media_types: video
sidebarType: 1
---

### Note

All references to the OpenRTB spec refer to OpenRtb v2.5 (https://www.iab.com/wp-content/uploads/2016/03/OpenRTB-API-Specification-Version-2-5-FINAL.pdf)

The Viqeo Bidder Adapter requires setup and approval from Viqeo.

Please reach out to <info@viqeo.tv> for more information.


### Bid params

{: .table .table-bordered .table-striped }
| Name                        | Scope    | Description                                                                                                                | Example                  | Type      |
|-----------------------------|----------|----------------------------------------------------------------------------------------------------------------------------|--------------------------|-----------|
| `user`                      | required | The object containing user data (See OpenRTB spec)                                                                         | `user: {}`               | `object`  |
| `user.buyeruid`             | required | User id                                                                                                                    | `"12345"`                | `string`  |
| `playerOptions`             | required | The object containing Viqeo player options                                                                                 | `playerOptions: {}`      | `object`  |
| `playerOptions.profileId`   | required | Viqeo profile id                                                                                                           | `1382`                   | `number`  |
| `playerOptions.videId`      | optional | Viqeo video id                                                                                                             | `"ed584da454c7205ca7e4"` | `string`  |
| `playerOptions.playerId`    | optional | Viqeo player id                                                                                                            | `1`                      | `number`  |
| `device`                    | optional | The object containing device data (See OpenRTB spec)                                                                       | `device: {}`             | `object`  |
| `site`                      | optional | The object containing site data (See OpenRTB spec)                                                                         | `site: {}`               | `object`  |
| `app`                       | optional | The object containing app data (See OpenRTB spec)                                                                          | `app: {}`                | `object`  |
| `floor`                     | optional | Bid floor price                                                                                                            | `0.5`                    | `number`  |
| `currency`                  | optional | 3-letter ISO 4217 code defining the currency of the bid.                                                                   | `EUR`                    | `string`  |
| `test`                      | optional | Flag which will induce a sample bid response when true; only set to true for testing purposes (1 = true, 0 = false)        | `1`                      | `integer` |
| `sspId`                     | optional | For debug, request id                                                                                                      | `1`                      | `number`  |
| `renderUrl`                 | optional | For debug, script player url                                                                                               | `"https://viqeo.tv"`     | `string`  |
| `endpointUrl`               | optional | For debug, api endpoint                                                                                                    | `"https://viqeo.tv"`     | `string`  |
