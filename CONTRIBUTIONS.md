# Contributing upstream

In my free time I send fixes to the open-source tools I build with. Each one is reproduced and kept to a single focused change, with a test wherever the project has a place for one. This page tracks every one of them, including the ones that did not land and why.

_Last updated 10 November 2026: 5 merged, 4 in review, 3 closed._

## In review

| Project | Change | Fixes | Build | Review |
|---|---|---|---|---|
| [Avalonia #22781](https://github.com/AvaloniaUI/Avalonia/pull/22781) | Bring the XamlX fix below into Avalonia, with a test for the reported case, at a maintainer's request | [#22778](https://github.com/AvaloniaUI/Avalonia/issues/22778) | The new test fails on the current submodule and passes with the update; all 639 XAML tests pass (1 skipped). The full CI waits for a maintainer to start it | Waiting for a maintainer |
| [Meta · Docusaurus #12839](https://github.com/meta/docusaurus/pull/12839) | Convert MSYS Git paths to real Windows paths so builds work with MSYS2's Git | [#11920](https://github.com/meta/docusaurus/issues/11920) | A new CI job runs a real `docusaurus build` with MSYS2's Git: it fails without the fix and passes with it, on my fork. CLA, security scans and the preview deploy pass; the full CI waits for a maintainer to approve it | CodeRabbit reviewed it. Waiting for a maintainer |
| [Google · Functions Framework for Node.js #811](https://github.com/GoogleCloudPlatform/functions-framework-nodejs/pull/811) | Parse `application/*+json` request bodies as JSON | [#809](https://github.com/GoogleCloudPlatform/functions-framework-nodejs/issues/809) | CLA and commit-message checks pass; the full CI waits for a maintainer to approve it | Waiting for a maintainer |
| [Amethystora image template #1](https://github.com/Arsslensoft/amethystora-image-template/pull/1) | Apply a company policy that holds VPN connections alone, instead of dropping it silently | | The image build waits for a maintainer to approve it | Waiting for the maintainer |

## Merged

| Project | Change | Fixes | Shipped in |
|---|---|---|---|
| [Avalonia · XamlX #150](https://github.com/kekekeks/XamlX/pull/150) | Accept an enum value written with surrounding whitespace, as `[Flags]` values already were | [AvaloniaUI/Avalonia#22778](https://github.com/AvaloniaUI/Avalonia/issues/22778) | XamlX `master`, merged by an Avalonia maintainer on 10 November 2026, the day it was opened |
| [Amethystora #4](https://github.com/Arsslensoft/amethystora/pull/4) | Read the composefs digest where bootc 1.17 writes it, which unblocks every stable image | | [stable-20261107](https://github.com/Arsslensoft/amethystora/releases/tag/stable-20261107), approved and merged 6 November 2026 |
| [IBM · OpenAPI Validator #873](https://github.com/IBM/openapi-validator/pull/873) | Stop flagging binary file-download responses as collections | [#786](https://github.com/IBM/openapi-validator/issues/786) | `@ibm-cloud/openapi-ruleset` 1.33.17 and `ibm-openapi-validator` 1.38.8, approved and merged 4 November 2026 |
| [IBM · OpenAPI Validator #869](https://github.com/IBM/openapi-validator/pull/869) | Validate files given with Windows separators or glob characters | [#516](https://github.com/IBM/openapi-validator/issues/516) | `ibm-openapi-validator` 1.38.6, approved and merged 3 November 2026 |
| [IBM · OpenAPI Validator #870](https://github.com/IBM/openapi-validator/pull/870) | Fix a broken link to the Spectral OpenAPI rules | [#866](https://github.com/IBM/openapi-validator/issues/866) | `ibm-openapi-validator` 1.38.5, approved and merged 3 November 2026 |

## Closed without merging

| Project | Change | Why it closed |
|---|---|---|
| [Amethystora #10](https://github.com/Arsslensoft/amethystora/pull/10) | Refresh the Security app's UI instantly after switching or turning off a profile | The maintainer approved it, then fixed [#9](https://github.com/Arsslensoft/amethystora/issues/9) more broadly on `main` ([f15eec4](https://github.com/Arsslensoft/amethystora/commit/f15eec4)): every app now shows a change the moment it is made, from any source. I closed mine in its favour on 10 November. |
| [Supabase #52673](https://github.com/supabase/supabase/pull/52673) | Correct the description of `auth.email.secure_password_change` | Someone else's [#52552](https://github.com/supabase/supabase/pull/52552) made the same correction first, so I closed mine as a duplicate. |
| [Microsoft · TypeScript #65132](https://github.com/microsoft/TypeScript/pull/65132) | Match discriminated-union members when inferring between unions | A maintainer pointed to [#64695](https://github.com/microsoft/TypeScript/pull/64695), work already under way on the same problem, so I closed mine in its favour. |

[← Back to my profile](README.md)
