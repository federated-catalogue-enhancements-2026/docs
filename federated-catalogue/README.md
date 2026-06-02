# Architecture document for the GXFS Catalogue

## XFSC Federated Catalogue

The rendered architecture document (HTML site + PDF) is produced by the
[`Run docToolchain`](https://github.com/eclipse-xfsc/docs/actions/workflows/buildDocs.yml) workflow on every push to
`main` and uploaded as the `Documentation` artifact (containing
`federated-catalogue/build/pdf/architecture/catalogue-architecture.pdf` and the full `build/html5/` site).

Get the latest rendered docs:

1. Open the [latest successful `Run docToolchain` run on `main`](https://github.com/eclipse-xfsc/docs/actions/workflows/buildDocs.yml?query=branch%3Amain+is%3Asuccess).
2. Scroll to the **Artifacts** section and download `Documentation.zip`.
3. Unzip — open `catalogue-architecture.pdf` for the PDF or `html5/architecture/catalogue-architecture.html` for the website.

> Note: GitHub Actions artifacts expire after 90 days. For a permanent reference, link to the workflow run's commit SHA.

## FACIS - XFSC Catalogue Enhancements
The XFSC Federated Catalogue (CAT) manages metadata objects (typically credentials or other RDF descriptions, e.g., of Providers, their Service Offerings and Resources) throughout their life cycle and exposes them to Consumers. It enables verification of these objects against given schemas and/or trust anchors. 

This enhancement of the CAT modularizes its verification of credentials against trust anchors and generalizes its management of metadata objects beyond the former focus on credentials; thus, it will also be able to function as a Template Repository for the FACIS Digital Contract Service (DCS).

The enhanced specification document can be found here : [PDF](https://github.com/eclipse-xfsc/docs/blob/main/federated-catalogue/src/docs/CAT%20Enhancement/CAT_Enhancement_Specifications%20v1.0.pdf)

The implementation of the federated catalogue can be found here : [`implementation/federated-catalogue`](https://github.com/eclipse-xfsc/federated-catalogue)
