# Rightway

Rightway Healthcare is a New York-based healthcare navigation and pharmacy benefit management (PBM) company. It pairs clinical care navigation — licensed pharmacists, nurses and care guides reachable by phone and in-app — with a fully transparent, 100% pass-through PBM whose revenue comes from a single administrative fee rather than rebate spread. Rightway serves employers, health systems and public-sector plans covering roughly three million members.

- Website — https://www.rightwayhealthcare.com/
- Member portal — https://member.rightwayhealthcare.com/
- Status — https://status.rightwayhealthcare.com/
- GitHub — https://github.com/roadmaphealthcare
- Secondary market listing — https://forgeglobal.com/rightway_stock/

## API posture

Rightway publishes **no public developer program**: no developer portal, no API
documentation, no OpenAPI/GraphQL/AsyncAPI contract, no SDKs, no MCP server and no
A2A agent card. Contract discovery was run against every host on 2026-08-02 and every
probe missed.

One real API surface was observed and recorded: `api.rightwayhealthcare.com`, the
undocumented private HTTP/JSON backend for the Rightway member mobile and web apps.
It answers unauthenticated JSON on `/` (minimum supported client versions) and
`/health` (dependency readiness); everything functional is member-authenticated.

## Artifacts

| Artifact | File | Method |
|---|---|---|
| Conformance | `conformance/rightway-conformance.yml` | searched |
| Lifecycle / status page | `lifecycle/rightway-lifecycle.yml` | searched |
| llms.txt | `llms/rightway-llms.txt` | generated |
| Domain security | `security/rightway-domain-security.yml` | probed |
| Well-known probe results | `well-known/rightway-well-known.yml` | probed (all misses) |
