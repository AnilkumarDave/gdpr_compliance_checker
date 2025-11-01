# ⚠️ Risk & Issues Log — GDPR Compliance Checker (Academic Project)

This log documents risks and issues identified during the project along with their impact, mitigation strategies, owners, and status.

| ID  | Risk / Issue                                      | Impact                        | Mitigation                                                     | Owner   | Status |
|-----|--------------------------------------------------|-------------------------------|----------------------------------------------------------------|---------|--------|
| R1  | HTTPS request timeout on some websites          | Incomplete scan results       | Implement retry logic and longer timeout; limit crawl depth    | Dev     | Closed |
| R2  | False detection of personal data (emails/forms) | Incorrect compliance scoring  | Refined regex filters and HTML parsing accuracy                | Dev     | Closed |
| R3  | Lack of access to live organizational websites  | Limited real-world validation | Used dummy/test websites for ethical testing                  | Dev     | Closed |
| R4  | Limited understanding of full GDPR legal scope  | Misinterpretation of compliance checks | Focused on core GDPR principles (data collection, consent, security) | Student | Closed |
| R5  | Report formatting inconsistency (CSV output errors) | Unclear final report      | Added pandas-based CSV export with structured headers          | Dev     | Closed |
