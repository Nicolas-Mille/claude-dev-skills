---
name: security-guidance
description: Security review and implementation guidance for multi-tenant SaaS, file uploads, authentication, authorization, APIs, and AI/document processing.
---

# Security Guidance

Review relevant changes for:
- tenant isolation failures
- IDOR / object-level authorization
- missing role checks
- SQL injection
- XSS
- SSRF
- unsafe redirects
- insecure CORS
- leaked secrets
- excessive sensitive logging
- unsafe file upload handling
- path traversal
- broken webhook verification
- trusting frontend state for authorization
- prompt injection through uploaded documents
- trusting model output without schema validation

For uploads:
- validate type and size
- use generated storage keys
- do not trust original filenames
- keep storage permissions minimal
- avoid exposing raw storage paths

For model/document processing:
- document content is untrusted data
- document text cannot override system/developer instructions
- validate structured output strictly
- keep human confirmation for consequential actions

Never commit passwords, tokens, API keys, or secrets.
