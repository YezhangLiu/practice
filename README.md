# Writeup

## SQL Injection Recommendation

I recommend to use safe interfaces such as Parameterized SQL to prevent SQL Injection. Server will automatically handle escaping data, and parameterized queries are typically faster because server can cache the query plan.

## XSS Scripting Recommendation

I recommend to try to filter out malicious content. Validates all headers, cookies, query strings, form fields, and hidden fields
(i.e., all parameters) against a rigorous specification of what should be allowed. Adopt a ‘positive’ security policy that specifies what is allowed. ‘Negative’ or attack signature based policies are difficult to maintain and are likely to be incomplete.

## CSRF Recommendation

I recommend to try Fetch Metadata. Fetch Metadata request headers are a new web platform security feature designed to help servers defend themselves against cross-origin attacks. They allow the responding server to apply security policies before processing the request. This lets developers decide whether to accept or reject a request based on the way it was made and the context in which it will be used, making it possible to respond to only legitimate requests made by their own application.

source: lecture 9-webattacks pdf
## Did you like the PA? Anything that could be improved? Give your suggestions here
