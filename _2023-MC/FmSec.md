---
title: "Exchanging FMUs in a secure manner"
author: "Christian Wolf ([EKS InTec GmbH](https://www.eks-intec.de))"
category: "excluded"
---

The current FMI standard is mainly created from research groups in cooperation with industry partners.
While the general structure is well-known and well-suited in order to exchange simulation models between partners, some aspects from current industries are not addressed in depth:
the required security features are not included by design.

For the real-world usage of FMUs this is a significant drawback.
The exchange of FMUs in the current state falls back to the typical measurements to establish trust between the involved parties.
Such measures are encrypted/signed mails, harsh contracts, and quite some trust in the persons/companies involved.
In fact, there is no automatic way to guarantee the trustworthiness of a simulation model in an end-to-end fashion.

The FmSec project aims at establishing such a trust model.
Different approaches are presented in order to establish a certification scheme for exchanging FMUs.
The solutions shown are focused on a decentralized structure to avoid single points of failure.
Accountability is guaranteed by state-of-the-art cryptography methods.
Extensions (like custom licensing and expiry date) can be implemented as well.

More information can will be presented at [our contribution at the Modelica conference](https://www.conftool.com/modelica2023/index.php?page=browseSessions&form_session=39#paperID184).
