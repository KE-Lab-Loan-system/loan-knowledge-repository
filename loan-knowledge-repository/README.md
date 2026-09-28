# 🏦 Loan Eligibility & Credit Risk Knowledge Repository

A knowledge repository on how banks in India decide whether to give a loan. It supports the **Loan Eligibility & Credit Risk Assessment Expert System** (Knowledge Engineering Lab, IGDTUW).

**Access:** 🌐 Public (read-only). Internal decision rules and past cases are kept in a separate **private** repository with controlled access.

## 📂 How the knowledge is organized

The repository is organized by **type of knowledge**:

### 1. Declarative knowledge (facts) – [`declarative/`](declarative/)
| Topic | File |
|---|---|
| Loan types | [loan-types.csv](declarative/loan-types.csv) |
| Eligibility criteria | [eligibility-criteria.csv](declarative/eligibility-criteria.csv) |
| Documents required | [documents-required.csv](declarative/documents-required.csv) |
| Credit score knowledge | [credit-score-knowledge.md](declarative/credit-score-knowledge.md) |
| Regulations & policies (RBI) | [regulations-and-policies.md](declarative/regulations-and-policies.md) |
| Glossary | [glossary.csv](declarative/glossary.csv) |
| FAQs | [faqs.md](declarative/faqs.md) |

### 2. Procedural knowledge (how things are done) – [`procedural/`](procedural/)
| Topic | File |
|---|---|
| Loan application process (with flowchart) | [loan-application-process.md](procedural/loan-application-process.md) |

### 3. Heuristic knowledge (expert rules of thumb)
Stored in the **private** repository `internal-credit-decision-knowledge` (decision rules + case library). Access is given only to authorised members.

## 🔗 How topics connect
- Each **eligibility criterion**, **document** and **decision rule** has a `Loan Type` column that links it to an entry in [loan-types.csv](declarative/loan-types.csv).
- The [process](procedural/loan-application-process.md) shows *when* each piece of knowledge is used: documents → KYC → credit score → eligibility → decision.

## 📚 Sources
See [references.md](references.md).

## 👥 Contributors
Ritu Prabhat · Riya Mishra
