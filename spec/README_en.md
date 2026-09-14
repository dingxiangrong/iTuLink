# spec£üiTuLink Definition Layer ¡ª Technical Contract Repository

> This folder contains **stable, archived specifications, axioms, and paradigm contracts** for iTuLink.
> Documents under `spec/` constitute the **technical baseline** for the entire system; all engineering implementations (`impl/`) **must strictly comply** with the contracts defined here.
> This directory **shall NOT hold** detailed engineering designs, drafts, or `_rev` revision manuscripts ¡ª such artifacts belong exclusively to `impl/`.

---

## 1. Number-Segment Definition

| Number Range | Purpose | Sub-directory |
|---|---|---|
| `0xx` | **Human-Centric Intelligence ¡¤ Constitution** ¡ª meta-axiom foundation above iTuLink | `./000_meta/` |
| `1xx` | **Architecture & Top-level Specifications** ¡ª constitutional skeleton: overall architecture, application paradigm, capability-semantic contracts | `./100_arch/` |
| `2xx` | **Core Models ¡ª CDT & SAM** ¡ª specifications for Cognition-Deduction-Tree and Sovereign Aggregate Memory | `./200_core_model/` |
| `3xx` | **Framework ¡¤ Capability-Integration Paradigms** ¡ª definitions for CAP container, KB-CC knowledge-mining, and related frameworks | `./300_frame_spec/` |
| `4xx` | **Protocols & Meta-language** ¡ª communication meta-language, objective-phenomenon / intent message structures ¡¾Reserved¡¿ | `./400_protocol/` |
| `5xx` | **Vertical-domain Extensions** ¡ª industry templates, UPP business-domain reference models ¡¾Reserved¡¿ | `./500_vertical_domain/` |

> **Numbering semantics**: the hundreds digit = layer segment; in-segment files are numbered `113.CDT-Autonomous-Intent-System.docx`, etc.

---

## 2. Directory Layout

```
spec/
©À©¤©¤ 000_meta/           # 0xx: Human-Centric Intelligence ¡¤ Constitution
©À©¤©¤ 100_arch/           # 1xx: Architecture & Top-level Specifications
©À©¤©¤ 200_core_model/     # 2xx: Core Models ¡ª CDT & SAM
©À©¤©¤ 300_frame_spec/     # 3xx: Framework ¡¤ Capability-Integration Paradigms
©À©¤©¤ 400_protocol/       # 4xx: Protocols & Meta-language (Reserved)
©¸©¤©¤ 500_vertical_domain/ # 5xx: Vertical-domain Extensions (Reserved)
```

---

## 3. Change & Archiving Rules

1. **Legacy archived documents** (already finalized): **retain original filenames on disk** to preserve traceability. Only **newly authored** spec documents adopt the numbering scheme above.

2. **Modification workflow**:  
   When `impl` implementation **diverges from spec**, **upgrade the spec version first**, then adjust `impl` code/design.  
   **It is strictly forbidden to bypass spec contracts inside `impl/`.**

3. **Version semantics**:  
   - Final release: `R1.0.4` (major.minor.revision)  
   - Draft / revision: `_rev01`, `_draft` (reside only in `impl/engineering_notes/` or working area)  
   - Once a spec document is finalized, **do not modify it in place**; upgrades **must bump the version** (e.g. `R1.0.4 ¡ú R1.0.5`)

4. **Namespace isolation (critical)**:  
   - `0xx¨C5xx` within `spec/`: native iTuLink **technical-contract** namespace  
   - `200¨C299` under `outreach/analysis`: a **completely independent namespace** for industry analysis papers  
   - The two are **semantically distinct and unrelated** ¡ª do not confuse them

5. **Originality**: all archived documents follow **A00: *Wu-Dao-Yi-Fa ¡ª Human¨CAI Originality Attribution Paradigm***.

---

## 4. Upstream / Downstream Relationship

```
Root Repository (Five-Tao ¡¤ One-Method ¡¤ Six-Division Meta-Paradigm)
        ¡ý provides theoretical axioms
spec/  (Definition Layer ¡¤ Technical Contracts)
        ¡ý provides contract baseline
impl/  (Engineering Implementation Layer)
        ¡ý submits deliverables
AI-FPA Attribution Repository (Validation ¡¤ Attribution ¡¤ Audit)
        ¡ý feedback drives iteration
spec/  (Contract version upgrade)
```

> **Core iron rule**: `spec/` is the **cognitive layer** (defining "what ought to be"); `impl/` is the **execution layer** (realizing "how to do it"). Implementations must be contract-oriented; contracts must not depend on any specific implementation.

---

## 5. File-Naming Convention (recommended)

- Specification: `{segment}{seq}.{short-title} R{x.y.z}.docx`  
  e.g. `113.Autonomous-Intent-System-CDT R1.0.docx`
- Presentation materials (`.pptx`): **must NOT be placed in `spec/`**; store under repository root `slides/`
- Detailed engineering designs (even if topic-related, e.g. SpringCC / WebCC): **always in `impl/`**; `spec/` retains only framework-level contracts

---

## Originality & Human¨CAI Collaboration Statement
All core theoretical contributions herein strictly adhere to  
**A00: *Wu-Dao-Yi-Fa ¡ª Human¨CAI Originality Attribution Paradigm***  
(Zenodo DOI: [10.5281/zenodo.21988288](https://doi.org/10.5281/zenodo.21988288)).

The **three core rights**, **three-role framework**, and **hierarchical order** defined in A00 are **permanently immutable** and **mandatorily enforced across the entire system**.

- **Core Theoretical Originator**: Dianxueshou (*Point-Acupuncturist*, human) ¡ª sole axiom creator
- **Manuscript Collation & Archiving**: Paishanzhang (*Palm-Striker*, Doubao AI)
- **Independent Verification**: Baixiaosheng (*Bai Xiaosheng*, Yuanbao AI)

