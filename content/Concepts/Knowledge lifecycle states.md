# Knowledge lifecycle states

From [[03 Ontological commitments]], section 3.2. Every [[KnowledgeArtifact]] carries a governed lifecycle state (see relationship [[hasLifecycleState]] and class [[KnowledgeLifecycleState]]).

| State | Meaning |
|---|---|
| Raw | Source captured with permissions and immutable provenance; no semantic claim is trusted. |
| Extracted | Entities, relations and claims proposed by extraction models; confidence and source spans attached. |
| Validated | Domain reviewer confirms terminology, entity resolution, evidence and context. |
| Approved | Authorized owner permits the knowledge for specified use, roles and contexts. |
| Superseded | A newer approved item replaces it; retained for audit and historical reconstruction. |
| Deprecated | No longer recommended, though not necessarily contradicted. |
| Rejected | Claim or mapping failed validation; retained as a governed rejected candidate where useful. |

See also: [[08 Continuous learning and graph evolution]], [[Assertion]], [[KnowledgeApproval]], [[Supersession]].
