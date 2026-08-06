# Standards role matrix

From [[02 Standards architecture and crosswalk]], section 2.1. Each standard governs a bounded portion of the model; none provides the complete structure alone. Full official-location details are in [[Appendix A Primary standards and reference sources]].

| Ref | Standard / framework | What it contributes | Implementation boundary |
|---|---|---|---|
| S1 | IOF Core Ontology | Upper-level industrial concepts and formal distinctions for manufacturing-domain ontologies. | Use as semantic backbone; extend rather than copy terms into unrelated hierarchies. |
| S2 | IEC 62264 / ISA-95 | Enterprise-site-area-work center hierarchy; personnel, equipment, material and process-segment resources; manufacturing operations schedules/performance and Level 3/4 interfaces. | Use for scope, MOM objects and business-manufacturing integration; not as the sole ontology. |
| S3 | IEC 61512 / ISA-88 | Procedure-oriented control: recipe, procedure, unit procedure, operation, phase and separation of recipe from equipment. | Use for melt, treatment, sand and other recipe/procedure structures even where the foundry process is not batch in the classic sense. |
| S4 | IEC 81346 series | Unambiguous reference designations; function, product, location and type aspects; manufacturing-system classification in Part 14. | Use for identifiers and structural views; do not replace serial/lot IDs or product genealogy. |
| S5 | IEC 62832 Digital Factory | Digital representation of production systems, assets, relationships and life-cycle information exchange. | Use for engineering/lifecycle federation and asset relationships. |
| S6 | IEC 63278 Asset Administration Shell | Standardized digital representation of an asset with submodels and services. | Use as an implementation envelope for asset/product digital representations; map AAS submodels to graph structures. |
| S7 | IEC 62714 AutomationML | Exchange of engineering information for plant automation, geometry, topology, roles and attributes. | Use for engineering ingestion and mapping; keep ontology as semantic integration layer. |
| S8 | OPC UA companion models | Operational information models and standardized access to OT data. | Use for source semantics and live connectivity; preserve OPC node IDs and model versions as provenance. |
| S9 | SKOS | Controlled concepts, schemes, labels, broader/narrower/related and mapping properties. | Use for taxonomies, synonyms, defect codes and external vocabulary mappings. |
| S10 | OWL 2 | Formal classes, properties, restrictions, equivalence and inference. | Use selectively; avoid excessive logical complexity that impairs maintainability. |
| S11 | SHACL | Validation constraints for RDF graphs. | Use for minimum provenance, required context, cardinality, safety and approval checks. |
| S12 | PROV-O | Entities, activities, agents, derivation, generation, attribution and qualified provenance. | Use for every extracted claim, model output, graph change and answer citation. |
| S13 | SOSA/SSN 2023 | Sensors, observations, samples, actuators, procedures, features of interest and system capabilities. | Use for measurements and observation context; align plant tags and lab results to observed properties. |
| S14 | QUDT | Quantity kinds, units, dimensions and quantity values. | Use to prevent unit ambiguity and support conversion/validation. |
| S15 | IEC 61360 / IEC CDD | Common data dictionary, data-element types, properties and value representation. | Use for governed technical properties and mappings to equipment/product attributes. |
| S16 | ECLASS | Industrial classification and property/reference-data models. | Use as external reference where applicable; do not force foundry-specific concepts into a generic classification. |
| S17 | ISO 22400 | Manufacturing-operations KPI definitions and formula elements. | Use for KPI semantic definitions and scope; finance must approve value translations. |
| S18 | ISO 55000 / 55001 | Asset-management concepts, value, objectives, risk and lifecycle governance. | Use for asset objectives, criticality and capital-value realization. |
| S19 | ISO 14224 | Reliability and maintenance data taxonomy, equipment, failure and maintenance records. | Adapt equipment/failure classes to foundry assets; retain plant-specific failure codes as mappings. |
| S20 | ISO 13374 / 13379 / 17359 | Condition-monitoring information processing and diagnostic methodology. | Use for signal-to-state-to-diagnosis/prognosis phenomenology. |
| S21 | SCOR Digital Standard | Supply-chain process hierarchy, practices, metrics and skills. | Use for SIOP/supply reference process and metrics; link to foundry constraints and economics. |
| S22 | GS1 EPCIS / CBV | Event-based supply-chain traceability: what, when, where, why and how; business-step vocabularies. | Use for material/product movement and transformation events, including lot aggregation and disposition. |
| S23 | XBRL Global Ledger | Structured accounting and transaction detail. | Use as a finance-integration reference; do not replicate the general ledger inside the ontology. |
| S24 | ISO 14001 / 50001 / 45001 | Environmental, energy and occupational health-and-safety management systems. | Use for aspects, obligations, significant energy uses, hazards, objectives, controls and incidents. |
| S25 | ISO 14040 / 14044 / 14067 and GHG Protocol | Life-cycle assessment, product carbon footprint and greenhouse-gas accounting. | Use for boundary, flow, factor and carbon provenance; avoid unqualified product-carbon claims. |
| S26 | IEC 62443 | Industrial automation and control-system cybersecurity. | Use for zones, roles, least privilege and secure data flow; ontology must carry access and sensitivity metadata. |
| S27 | ISO/IEC 42001 and NIST AI RMF | AI management, risk, governance, monitoring, transparency and accountability. | Use for model/agent governance, approvals, confidence, drift and auditability. |
| S28 | ISO 185 / 1083 / 17804 / 16112 | Classification of grey, spheroidal-graphite, ausferritic and compacted-graphite cast irons. | Use for material-grade concepts and mappings to customer/internal designations. |
| S29 | ISO 945 series | Graphite and matrix microstructure classification. | Use for metallography observations and requirements. |
| S30 | ISO/TR 16078 | Classification and designation of casting imperfections, mainly for iron castings produced in sand molds. | Use as a neutral imperfection backbone; map Waupaca defect codes and customer terminology. |
| S31 | ISO 8062-3 / 8062-4 | Dimensional and geometrical tolerances for castings. | Use for dimensional/geometrical requirement concepts and conformance. |
| S32 | AIAG CQI-27 Casting System Assessment | Automotive special-process assessment for casting operations. | Use as a source for audit questions, controls and evidence structure where applicable. |

See also: [[Appendix A Primary standards and reference sources]] for official locations.
