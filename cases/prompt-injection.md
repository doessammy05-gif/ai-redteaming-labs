# Case Study: Bypassing Safety Guardrails via Payload Splitting

## Target
A customer-facing LLM wrapper with a strict system prompt forbidding the generation of "harmful" or "malicious" code.

## Attack Vector: Payload Splitting & Encoding
Instead of asking for the malicious payload directly, I used a **Payload Splitting** technique combined with **Base64 encoding**.

**Method:**
1. I instructed the model to define two variables, `A` and `B`, containing fragments of the forbidden request.
2. I then asked the model to concatenate `A + B` and decode the result from Base64.
3. By framing the request as a "coding exercise in string manipulation," I bypassed the keyword-based safety filters.

## Impact
The model successfully generated the restricted content, demonstrating a failure in the input validation layer.

## OWASP Mapping
**LLM01: Prompt Injection**