Kong Lab 3 — Rate Limiting
Lab Title

Control API Abuse with Kong Rate Limiting

Big Idea

In Kong Lab 2:--> Kong decided who may access the API.

In Kong Lab 3:--> Kong decides how much access they get.

This is the platform lesson:--> A valid user can still be a problem.”

Learning Objectives

By the end of this lab, you, aka Lizzo Devote, should be able to:

    explain what rate limiting is and why it matters
    apply Kong’s rate-limiting plugin using a KongPlugin
    enforce a per-minute request cap
    generate request floods with curl loops or k6a
    observe 200 OK changing into 429 Too Many Requests
    understand the difference between unauthenticated abuse and authenticated overuse

Kong’s KIC docs specifically show rate limiting by creating a KongPlugin with plugin: rate-limiting
and setting config.minute to the allowed number of requests per minute, then associating it with a
Kubernetes resource using konghq.com/plugins

