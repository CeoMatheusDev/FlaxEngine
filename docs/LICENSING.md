# Licensing policy

This document explains how licensing is organized in the CeoMatheusDev Flax Engine fork. It is a practical notice, not legal advice. The actual license texts and applicable third-party notices control.

## 1. Separate rights; no repository-wide relicensing

This repository is a derivative fork of [FlaxEngine/FlaxEngine](https://github.com/FlaxEngine/FlaxEngine). The presence of a file in this repository does not mean that CeoMatheusDev, Matheus A. Santos, or Hardion Labs owns it.

The repository intentionally keeps separate licensing scopes:

| Material | Governing terms |
| --- | --- |
| Flax Engine source code, Engine Tools, Content, and modifications of those materials | [Flax Engine EULA](https://flaxengine.com/licensing/) and applicable upstream notices |
| Third-party libraries, tools, assets, fonts, and other dependencies | Their respective license texts and notices |
| Original Hardion Labs materials expressly marked or listed below | [HLOML-1.0](../LICENSE-HARDION.md) |
| Original work by an individual contributor not assigned or licensed to Hardion Labs | The rights and terms of that contributor; no Hardion Labs license is implied |

There is no MIT/GPL/Apache blanket license for this repository. Neither this document nor the Hardion Labs license changes the Flax EULA.

## 2. Hardion Labs Original Materials License (HLOML-1.0)

The **Hardion Labs Original Materials License 1.0** is a custom, permissive copyright license for specifically identified original materials. It allows use, modification, redistribution, sublicensing, and commercial use, subject to preservation of the license and attribution notices.

The license is intentionally limited to materials that Hardion Labs owns or is authorized to license. It does not cover the Flax Engine, upstream code, Flax assets, third-party dependencies, trademarks, or unmarked files.

Full terms: [LICENSE-HARDION.md](../LICENSE-HARDION.md).

## 3. How a file becomes covered by HLOML-1.0

A file is covered only if one of these conditions is met:

1. The file contains an explicit notice such as:

   `SPDX-License-Identifier: HLOML-1.0`

   `Copyright (c) 2026 Hardion Labs`

2. The file is expressly listed in the inventory below.

A file is not covered merely because it is in the repository, refers to Hardion Labs, was edited by a Hardion Labs maintainer, or appears in a commit authored by Matheus A. Santos.

### Initial covered-material inventory

No existing Flax Engine source, binary, asset, or third-party file is designated as HLOML-1.0 material by this change. The inventory starts empty. New original Hardion Labs documents or code may be added only after confirming the relevant ownership or licensing authority and explicitly marking or listing each file.

| Path | Material | Basis for Hardion Labs licensing |
| --- | --- | --- |
| _No files designated yet_ | — | — |

This empty initial inventory is deliberate: it avoids retroactively claiming rights over upstream or third-party materials. The license text itself is supplied as the terms for future, expressly identified Covered Material; publishing the terms does not automatically license every repository file under them.

## 4. Flax Engine EULA obligations

Always consult the [current official EULA](https://flaxengine.com/licensing/). The official document currently linked from the Flax licensing page is dated October 31, 2023; the web page or a later EULA version may supersede it.

Among other things, the EULA addresses:

- **Distribution (section 1(A)):** permitted distribution forms and channels for Engine Code, Engine Tools, Content, and Products. Public distribution of Engine Tools and modified Engine Tools is restricted to the channels specified there, including the Flax GitHub fork network for public source distribution.
- **Non-compatible licenses (section 1(C)):** restrictions on combining Flax technology with material whose terms would require Flax technology to be governed by different terms. The EULA gives examples of prohibited and permitted licenses; assess each dependency and combination rather than assuming compatibility.
- **Royalties and reporting (section 3):** a standard royalty of 4% on covered worldwide gross revenue above the first US$250,000 for each Product per calendar quarter, subject to the EULA's exclusions, definitions, reporting, and payment requirements.
- **Contributions (section 5):** contributions made available to Flax are subject to the assignment and fallback license provisions in that section. Review it before submitting code, documentation, assets, or other work to upstream Flax.
- **Notices and attribution (section 6):** preserve proprietary notices and include the specified Flax product credits.

This list is a summary only. The EULA text controls.

## 5. Attribution and project identity

- Identify this repository as an unofficial community fork maintained by CeoMatheusDev / Hardion Labs only where that accurately reflects the actual maintainer relationship.
- Identify Matheus A. Santos as an individual author only for work he actually authored.
- Do not imply that Hardion Labs owns Flax Engine or is endorsed by Flax.
- Preserve all upstream copyright, trademark, and third-party notices.
- Do not remove or replace Flax branding in a way that violates the EULA or upstream branding rules.

## 6. Contributions to this fork

Before licensing a contribution under HLOML-1.0, the contributor must have authority to grant those rights and must explicitly identify the submitted files as Covered Material. A contribution is not automatically owned by Hardion Labs merely because it is submitted to this repository.

Contributions intended for the upstream Flax project are a separate matter. Review the upstream contribution process and EULA section 5 before making any work available to Flax.

## 7. Review checklist for new files and dependencies

Before adding a file or dependency:

1. Identify its author and copyright owner.
2. Record its exact license and preserve its notices.
3. Determine whether it is Flax Material, Third-Party Material, or independently authored Hardion Labs material.
4. If claiming HLOML-1.0 coverage, confirm Hardion Labs has the necessary rights and mark/list the file explicitly.
5. Review EULA section 1(C) for compatibility where the file is combined with Flax technology.
6. Do not change the license of existing upstream files as part of a documentation-only change.

---
Last reviewed: 2026-11-14.
