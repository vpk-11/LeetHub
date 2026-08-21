# Graph Report - leethub  (2026-08-21)

## Corpus Check
- 21 files · ~280,769 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 215 nodes · 359 edges · 20 communities (18 shown, 2 thin omitted)
- Extraction: 92% EXTRACTED · 8% INFERRED · 0% AMBIGUOUS · INFERRED: 28 edges (avg confidence: 0.8)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `f1f5b567`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- [[_COMMUNITY_jQuery Vendor Bundle|jQuery Vendor Bundle]]
- [[_COMMUNITY_LeetCode Submission Core|LeetCode Submission Core]]
- [[_COMMUNITY_Stats and Version Utilities|Stats and Version Utilities]]
- [[_COMMUNITY_package.json Build Deps|package.json Build Deps]]
- [[_COMMUNITY_README and Popup UI|README and Popup UI]]
- [[_COMMUNITY_WelcomeSetup Flow (welcome.js)|Welcome/Setup Flow (welcome.js)]]
- [[_COMMUNITY_Submit Button DOM Hook|Submit Button DOM Hook]]
- [[_COMMUNITY_GeeksforGeeks Support|GeeksforGeeks Support]]
- [[_COMMUNITY_Webpack Build Config|Webpack Build Config]]
- [[_COMMUNITY_Bug Report Issue Template|Bug Report Issue Template]]
- [[_COMMUNITY_Feature Request Issue Template|Feature Request Issue Template]]
- [[_COMMUNITY_Community 13|Community 13]]
- [[_COMMUNITY_Community 14|Community 14]]
- [[_COMMUNITY_Community 15|Community 15]]
- [[_COMMUNITY_Community 16|Community 16]]
- [[_COMMUNITY_Community 17|Community 17]]
- [[_COMMUNITY_Community 18|Community 18]]
- [[_COMMUNITY_Community 19|Community 19]]

## God Nodes (most connected - your core abstractions)
1. `$()` - 63 edges
2. `LeetCodeV2()` - 19 edges
3. `LeetCodeV1()` - 16 edges
4. `checkElem()` - 14 edges
5. `scripts` - 9 edges
6. `Te()` - 9 edges
7. `updateReadmeTopicTagsWithProblem()` - 8 edges
8. `oe()` - 7 edges
9. `ce()` - 7 edges
10. `G()` - 7 edges

## Surprising Connections (you probably didn't know these)
- `option()` --calls--> `$()`  [INFERRED]
  scripts/welcome.js → scripts/jquery-3.3.1.min.js
- `repositoryName()` --calls--> `$()`  [INFERRED]
  scripts/welcome.js → scripts/jquery-3.3.1.min.js
- `handleRepoCreateError()` --calls--> `$()`  [INFERRED]
  scripts/welcome.js → scripts/jquery-3.3.1.min.js
- `createRepo()` --calls--> `$()`  [INFERRED]
  scripts/welcome.js → scripts/jquery-3.3.1.min.js
- `handleLinkRepoError()` --calls--> `$()`  [INFERRED]
  scripts/welcome.js → scripts/jquery-3.3.1.min.js

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **LeetHub Onboarding Flow (Auth, Hook, Commit modes shared across popup and welcome)** — popup_popup_auth_mode, popup_popup_hook_mode, popup_popup_commit_mode, welcome_welcome_auth_mode, welcome_welcome_hook_mode, welcome_welcome_commit_mode [INFERRED 0.85]
- **GitHub Issue Templates (bug and feature reporting)** — issue_template_bug_report_bug_report, issue_template_config_bug_report_form, issue_template_feature_request_feature_request, issue_template_config_issue_template_config [EXTRACTED 1.00]

## Communities (20 total, 2 thin omitted)

### Community 0 - "jQuery Vendor Bundle"
Cohesion: 0.15
Nodes (6): $(), de(), Je(), le(), Qe(), W()

### Community 1 - "LeetCode Submission Core"
Cohesion: 0.14
Nodes (23): api, createRepoReadme(), decode(), encode(), getAndInitializeStats(), getGitHubFile(), getPath(), LeetHubNetworkError (+15 more)

### Community 2 - "Stats and Version Utilities"
Cohesion: 0.09
Nodes (5): incrementStats(), checkElem(), getDifficulty(), LeetCodeV1(), LeetCodeV2()

### Community 3 - "package.json Build Deps"
Cohesion: 0.08
Nodes (25): description, devDependencies, chrome-types, copy-webpack-plugin, filemanager-webpack-plugin, ignore-loader, jasmine, prettier (+17 more)

### Community 4 - "README and Popup UI"
Cohesion: 0.40
Nodes (5): LeetHub 2.0 (Project), LeetHub v1 (original extension), Local Development Setup Instructions, npm Build Commands (format, lint, build), Why LeetHub Was Built (Rationale)

### Community 5 - "Welcome/Setup Flow (welcome.js)"
Cohesion: 0.17
Nodes (9): api, createRepo(), getCreateErrorString(), getLinkErrorString(), handleLinkRepoError(), handleRepoCreateError(), linkRepo(), option() (+1 more)

### Community 6 - "Submit Button DOM Hook"
Cohesion: 0.29
Nodes (4): addManualSubmitBtn(), api, getSubmissionPageBtns(), setupManualSubmitBtn()

### Community 8 - "Webpack Build Config"
Cohesion: 0.29
Nodes (5): __dirname, entries, __filename, folderIgnore, ignore

### Community 10 - "Bug Report Issue Template"
Cohesion: 0.67
Nodes (3): Bug Report Issue Template (Markdown), Bug Report Form (YAML issue form), Issue Template Config

### Community 13 - "Community 13"
Cohesion: 0.21
Nodes (12): be(), Ee(), ge(), he(), I(), N(), ne(), oe() (+4 more)

### Community 14 - "Community 14"
Cohesion: 0.36
Nodes (8): ce(), Ie(), m(), me(), Re(), ve(), xe(), ye()

### Community 15 - "Community 15"
Cohesion: 0.40
Nodes (6): ae(), ct(), et(), fe(), lt(), Ze()

### Community 16 - "Community 16"
Cohesion: 0.40
Nodes (5): a(), k(), t(), ut(), xt()

### Community 17 - "Community 17"
Cohesion: 0.50
Nodes (5): ft(), G(), j(), pt(), st()

### Community 18 - "Community 18"
Cohesion: 0.50
Nodes (4): C(), jt(), R(), x()

### Community 19 - "Community 19"
Cohesion: 0.16
Nodes (11): addLeadingZeros(), convertToSlug(), debounce(), DIFFICULTY, formatStats(), getBrowser(), isObject(), languages (+3 more)

## Knowledge Gaps
- **39 isolated node(s):** `api`, `api`, `name`, `version`, `private` (+34 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **2 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `$()` connect `jQuery Vendor Bundle` to `Welcome/Setup Flow (welcome.js)`, `Community 13`, `Community 14`, `Community 15`, `Community 16`, `Community 17`, `Community 18`?**
  _High betweenness centrality (0.315) - this node is a cross-community bridge._
- **Why does `LeetCodeV2()` connect `Stats and Version Utilities` to `LeetCode Submission Core`, `Community 19`?**
  _High betweenness centrality (0.073) - this node is a cross-community bridge._
- **Why does `getBrowser()` connect `Community 19` to `LeetCode Submission Core`, `Welcome/Setup Flow (welcome.js)`, `Submit Button DOM Hook`?**
  _High betweenness centrality (0.070) - this node is a cross-community bridge._
- **Are the 5 inferred relationships involving `$()` (e.g. with `createRepo()` and `handleLinkRepoError()`) actually correct?**
  _`$()` has 5 INFERRED edges - model-reasoned connections that need verification._
- **What connects `api`, `api`, `name` to the rest of the system?**
  _40 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `jQuery Vendor Bundle` be split into smaller, more focused modules?**
  _Cohesion score 0.14705882352941177 - nodes in this community are weakly interconnected._
- **Should `LeetCode Submission Core` be split into smaller, more focused modules?**
  _Cohesion score 0.14285714285714285 - nodes in this community are weakly interconnected._