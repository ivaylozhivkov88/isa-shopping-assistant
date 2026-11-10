<div align="center">

<img src="assets/banner.svg" alt="ISA - Intelligent Shopping Assistant" width="100%"/>

<br/>

![Android](https://img.shields.io/badge/Android-0B8F75?style=for-the-badge&logo=android&logoColor=white)
![Kotlin](https://img.shields.io/badge/Kotlin-0B8F75?style=for-the-badge&logo=kotlin&logoColor=white)
![Compose](https://img.shields.io/badge/Jetpack_Compose-0B8F75?style=for-the-badge&logo=jetpackcompose&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-0B8F75?style=for-the-badge&logo=firebase&logoColor=white)
![Languages](https://img.shields.io/badge/BG_%7C_EN-D2F4EC?style=for-the-badge&labelColor=0B8F75&color=D2F4EC)

**An Android app that compares grocery prices across Bulgaria's biggest retail chains.**

</div>

> **Showcase repository.** This page presents the product and the engineering behind it. The source code is private.

---

## Screens

<div align="center">
<img src="assets/screens/welcome.png" width="200" alt="Welcome"/>
<img src="assets/screens/chains.png" width="200" alt="Choose your chains"/>
<img src="assets/screens/offers.png" width="200" alt="Offers"/>
<img src="assets/screens/catalog.png" width="200" alt="Product catalog"/>
</div>

## What it does

| | |
|---|---|
| **Price comparison** | Prices from the brochures of six chains side by side, so you see where a basket is cheapest |
| **Shopping list** | Smart list with barcode scanning and a per-chain basket comparison |
| **Offers** | Latest offers, top deals and full brochures, refreshed automatically |
| **Receipts and savings** | Scan a receipt to tick off what you bought and track the discounts you caught |
| **Recipes, budget, loyalty cards** | Everything around the weekly shop in one place |
| **In-store mode** | Screen stays on, with items left and an estimated total at the top |
| **Sync** | Optional Google sign-in keeps your lists on all your devices |
| **PRO** | Subscription unlocks the full catalogue with store and category filters |

Bilingual (Bulgarian / English), prices in euro.

## Engineering

| Area | Approach |
|---|---|
| App | Kotlin, Jetpack Compose, Hilt, Room, DataStore, clean layering (UI, ViewModel, use case, repository) |
| Backend | Firebase: Firestore, Auth, Cloud Functions (TypeScript), Cloud Messaging, Storage, Hosting |
| Data pipeline | Scheduled Python pipeline that downloads brochures, extracts products with a vision model, normalises and matches them to a product catalogue, and computes price statistics and top promotions |
| Security | Firestore security rules with a dedicated rules test suite, secrets kept out of the repository |
| Monetisation | Google Play Billing subscription and AdMob |
| Privacy | Analytics are opt-in, with a clear explanation of exactly what is collected |

## Design language

<table>
<tr>
<td bgcolor="#0B8F75" width="130" align="center"><b><font color="#FFFFFF">#0B8F75</font></b><br/><sub><font color="#FFFFFF">teal</font></sub></td>
<td bgcolor="#D2F4EC" width="130" align="center"><b>#D2F4EC</b><br/><sub>mint</sub></td>
<td bgcolor="#F6F8F7" width="130" align="center"><b>#F6F8F7</b><br/><sub>paper</sub></td>
<td bgcolor="#0F1A17" width="130" align="center"><b><font color="#FFFFFF">#0F1A17</font></b><br/><sub><font color="#FFFFFF">ink</font></sub></td>
</tr>
</table>

A calm, friendly look: a single teal accent, generous spacing and large readable prices.

---

<div align="center">

Built by [@ivaylozhivkov88](https://github.com/ivaylozhivkov88)

</div>
