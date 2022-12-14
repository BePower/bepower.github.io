---
layout: default
title: Test Environment
nav_order: 1
parent: Be Charge as CPO
grand_parent: Roaming
permalink: /docs/roaming/cpo/test
---

# Be Charge as CPO
{: .no_toc }

Test Environment
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{: toc }

---

## Details

- `country_code`: **IT**
- `party_id`: **BEC**

## Peer to peer (OCPI)

Be Charge supports OCPI integration for connection to other MSPs.

### CPO Versions URL

```
Sent during handshake phase, offline
```

### Supported Versions

| Version   | Status    |
|:----------|:----------|
| OCPI v2.1 | Supported |

### OCPI Module Support Matrix

| Module      | Direction          | Method                             | Supported? | Notes                                              |
|:------------|:-------------------|:-----------------------------------|:-----------|:---------------------------------------------------|
| Credentials | **CPO** &rarr; MSP | `POST /credentials`                | **Yes**    |                                                    |
| Credentials | **CPO** &rarr; MSP | `PUT|PATCH /credentials`           | **Yes**    |                                                    |
| Credentials | **CPO** &rarr; MSP | `DELETE /credentials`              | No         |                                                    |
| Credentials | MSP &rarr; **CPO** | `GET /credentials`                 | **Yes**    |                                                    |
| Credentials | MSP &rarr; **CPO** | `POST /credentials`                | **Yes**    |                                                    |
| Credentials | MSP &rarr; **CPO** | `PUT|PATCH /credentials`           | **Yes**    |                                                    |
| Credentials | MSP &rarr; **CPO** | `DELETE /credentials`              | No         |                                                    |
| Locations   | **CPO** &rarr; MSP | `GET /locations`                   | No         |                                                    |
| Locations   | **CPO** &rarr; MSP | `PUT /locations/:path`             | **Yes**    |                                                    |
| Locations   | **CPO** &rarr; MSP | `PATCH /locations/:path`           | **Yes**    |                                                    |
| Locations   | MSP &rarr; **CPO** | `GET /locations`                   | **Yes**    | Locations won't be available right after handshake |
| Sessions    | **CPO** &rarr; MSP | `GET /sessions/:path`              | No         |                                                    |
| Sessions    | **CPO** &rarr; MSP | `PUT /sessions/:path`              | **Yes**    | `CDR` and `Session` will have the same id          |
| Sessions    | **CPO** &rarr; MSP | `PATCH /sessions/:path`            | No         | Using `PUT` instead                                |
| Sessions    | MSP &rarr; **CPO** | `GET /sessions`                    | **Yes**    |                                                    |
| CDRs        | **CPO** &rarr; MSP | `GET /cdrs/:path`                  | No         |                                                    |
| CDRs        | **CPO** &rarr; MSP | `POST /cdrs`                       | **Yes**    | `CDR` and `Session` will have the same id          |
| CDRs        | MSP &rarr; **CPO** | `GET /cdrs`                        | **Yes**    |                                                    |
| Tariffs     | **CPO** &rarr; MSP | `GET /tariffs`                     | No         |                                                    |
| Tariffs     | **CPO** &rarr; MSP | `PUT /tariffs/:path`               | **Yes**    |                                                    |
| Tariffs     | **CPO** &rarr; MSP | `PATCH /tariffs/:path`             | **Yes**    |                                                    |
| Tariffs     | **CPO** &rarr; MSP | `DELETE /tariffs/:path`            | No         |                                                    |
| Tariffs     | MSP &rarr; **CPO** | `GET /tariffs`                     | **Yes**    |                                                    |
| Tokens      | **CPO** &rarr; MSP | `GET /tokens`                      | **Yes**    |                                                    |
| Tokens      | **CPO** &rarr; MSP | `POST /tokens/:tokenUid/authorize` | **Yes**    |                                                    |
| Tokens      | MSP &rarr; **CPO** | `GET /tokens/:path`                | **Yes**    |                                                    |
| Tokens      | MSP &rarr; **CPO** | `PUT /tokens/:path`                | **Yes**    |                                                    |
| Tokens      | MSP &rarr; **CPO** | `PATCH /tokens/:path`              | **Yes**    |                                                    |
| Commands    | MSP &rarr; **CPO** | `POST /commands/RESERVE_NOW`       | **Yes**    |                                                    |
| Commands    | MSP &rarr; **CPO** | `POST /commands/START_SESSION`     | **Yes**    |                                                    |
| Commands    | MSP &rarr; **CPO** | `POST /commands/STOP_SESSION`      | **Yes**    |                                                    |
| Commands    | MSP &rarr; **CPO** | `POST /commands/UNLOCK_CONNECTOR`  | No         |                                                    |

## Hubject (OICP)

### Supported Versions

| Version   | Status    |
|:----------|:----------|
| OICP v2.3 | Supported |
