# Contributing upstream

In my free time I send fixes to the open-source tools I build with. Each one is reproduced, covered by a test, and kept to a single focused change. This page tracks every one of them, including the ones that did not land and why.

*Last updated 4 November 2026.*

## In review

| Project | Change | Fixes | Waiting on |
|---|---|---|---|
| [IBM · OpenAPI Validator #873](https://github.com/IBM/openapi-validator/pull/873) | Stop flagging binary file-download responses as collections | [#786](https://github.com/IBM/openapi-validator/issues/786) | A maintainer's review. Tests pass; signed off for the DCO |
| [Meta · Docusaurus #12839](https://github.com/meta/docusaurus/pull/12839) | Convert Git Bash (MSYS) paths to real Windows paths so builds work under Git Bash | [#11920](https://github.com/meta/docusaurus/issues/11920) | A maintainer to approve CI for a first-time contributor, then a review |
| [Google · Functions Framework for Node.js #811](https://github.com/GoogleCloudPlatform/functions-framework-nodejs/pull/811) | Parse `application/*+json` request bodies as JSON | [#809](https://github.com/GoogleCloudPlatform/functions-framework-nodejs/issues/809) | A maintainer to approve CI, then a review |
| [Amethystora #4](https://github.com/Arsslensoft/amethystora/pull/4) | Read the composefs digest where bootc 1.17 writes it, which unblocks every stable image | | A maintainer to approve CI, then a review |
| [Amethystora image template #1](https://github.com/Arsslensoft/amethystora-image-template/pull/1) | Apply a company policy that holds VPN connections alone, instead of dropping it silently | | A maintainer to approve CI, then a review |

## Merged

| Project | Change | Fixes | Shipped in |
|---|---|---|---|
| [IBM · OpenAPI Validator #869](https://github.com/IBM/openapi-validator/pull/869) | Validate files given with Windows separators or glob characters | [#516](https://github.com/IBM/openapi-validator/issues/516) | `ibm-openapi-validator` 1.38.6, merged 3 November 2026 |
| [IBM · OpenAPI Validator #870](https://github.com/IBM/openapi-validator/pull/870) | Fix a broken link to the Spectral OpenAPI rules | [#866](https://github.com/IBM/openapi-validator/issues/866) | `ibm-openapi-validator` 1.38.5, merged 3 November 2026 |

## Closed without merging

| Project | Change | Why it closed |
|---|---|---|
| [Supabase #52673](https://github.com/supabase/supabase/pull/52673) | Correct the description of `auth.email.secure_password_change` | Someone else's [#52552](https://github.com/supabase/supabase/pull/52552) made the same correction first, so I closed mine as a duplicate. |
| [Microsoft · TypeScript #65132](https://github.com/microsoft/TypeScript/pull/65132) | Match discriminated-union members when inferring between unions | A maintainer pointed to [#64695](https://github.com/microsoft/TypeScript/pull/64695), work already under way on the same problem, so I closed mine in its favour. |

[← Back to my profile](README.md)
