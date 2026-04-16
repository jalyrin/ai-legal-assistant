# Functional Specification
## AI Legal Assistant Platform

---

## 1. Core Use Cases

### Use Case 1 — Ask About Firm Documents

User:
"Asks a question about prior documents"

System:
- Searches firm documents
- Retrieves relevant content
- Generates answer with citations

---

### Use Case 2 — Draft Email Response

User:
Selects an email and asks for a reply

System:
- Reads email
- Applies firm tone
- Generates draft response
- User reviews before sending

---

### Use Case 3 — Draft Legal Document

User:
"Draft a probate notice for this matter"

System:
- Pulls matter data
- Retrieves template
- Generates draft
- Outputs formatted document

---

## 2. Core Workflows

### Workflow 1 — Document Retrieval (RAG)

1. User enters query
2. System embeds query
3. System searches vector DB
4. System retrieves relevant chunks
5. System sends to LLM
6. System returns answer

---

### Workflow 2 — Document Ingestion

1. User uploads or syncs document
2. System extracts text
3. System chunks text
4. System generates embeddings
5. System stores in database

---

### Workflow 3 — Email Drafting

1. User selects email
2. System extracts content
3. System retrieves relevant prior examples
4. System generates draft
5. User reviews

---

## 3. System Capabilities (Mapped to Build)

| Capability | Status |
|----------|--------|
| API | Built |
| Database | Built |
| Documents Table | Built |
| Embeddings | Not built |
| Retrieval (RAG) | Not built |
| Email Integration | Not built |
| Drafting Engine | Not built |

---

## 4. MVP Definition

MVP is complete when:

- User can upload documents
- User can ask questions about documents
- System returns grounded answers
- Basic drafting works

---

## 5. Constraints

- No autonomous actions
- Human approval required
- Must use firm data only (no hallucination)

---