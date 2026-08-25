# Graph Report - leethub  (2026-08-26)

## Corpus Check
- 30 files · ~283,573 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 299 nodes · 549 edges · 20 communities (14 shown, 6 thin omitted)
- Extraction: 95% EXTRACTED · 5% INFERRED · 0% AMBIGUOUS · INFERRED: 27 edges (avg confidence: 0.8)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `1ae88102`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- [[_COMMUNITY_jQuery Vendor Bundle|jQuery Vendor Bundle]]
- [[_COMMUNITY_LeetCode Submission Core|LeetCode Submission Core]]
- [[_COMMUNITY_Stats and Version Utilities|Stats and Version Utilities]]
- [[_COMMUNITY_package.json Build Deps|package.json Build Deps]]
- [[_COMMUNITY_README and Popup UI|README and Popup UI]]
- [[_COMMUNITY_Community 5|Community 5]]
- [[_COMMUNITY_Community 6|Community 6]]
- [[_COMMUNITY_GeeksforGeeks Support|GeeksforGeeks Support]]
- [[_COMMUNITY_Webpack Build Config|Webpack Build Config]]
- [[_COMMUNITY_Background Service Worker|Background Service Worker]]
- [[_COMMUNITY_Bug Report Issue Template|Bug Report Issue Template]]
- [[_COMMUNITY_Feature Request Issue Template|Feature Request Issue Template]]
- [[_COMMUNITY_Community 13|Community 13]]
- [[_COMMUNITY_Community 15|Community 15]]
- [[_COMMUNITY_Community 16|Community 16]]
- [[_COMMUNITY_Community 19|Community 19]]

## God Nodes (most connected - your core abstractions)
1. `$()` - 63 edges
2. `LeetCodeV2` - 22 edges
3. `LeetCodeV1` - 19 edges
4. `getBrowser()` - 17 edges
5. `githubHeaders()` - 16 edges
6. `checkElem()` - 14 edges
7. `compilerOptions` - 12 edges
8. `syncStatsFromRepo()` - 11 edges
9. `scripts` - 10 edges
10. `archiveAndResetStats()` - 9 edges

## Surprising Connections (you probably didn't know these)
- `renderStats()` --calls--> `$()`  [INFERRED]
  scripts/popup.ts → scripts/jquery-3.3.1.min.js
- `renderStats()` --calls--> `$()`  [INFERRED]
  scripts/welcome.ts → scripts/jquery-3.3.1.min.js
- `showCommitMode()` --calls--> `$()`  [INFERRED]
  scripts/welcome.ts → scripts/jquery-3.3.1.min.js
- `showHookMode()` --calls--> `$()`  [INFERRED]
  scripts/welcome.ts → scripts/jquery-3.3.1.min.js
- `checkModeType()` --calls--> `$()`  [INFERRED]
  scripts/welcome.ts → scripts/jquery-3.3.1.min.js

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **LeetHub Onboarding Flow (Auth, Hook, Commit modes shared across popup and welcome)** — popup_popup_auth_mode, popup_popup_hook_mode, popup_popup_commit_mode, welcome_welcome_auth_mode, welcome_welcome_hook_mode, welcome_welcome_commit_mode [INFERRED 0.85]
- **GitHub Issue Templates (bug and feature reporting)** — issue_template_bug_report_bug_report, issue_template_config_bug_report_form, issue_template_feature_request_feature_request, issue_template_config_issue_template_config [EXTRACTED 1.00]

## Communities (20 total, 6 thin omitted)

### Community 0 - "jQuery Vendor Bundle"
Cohesion: 0.07
Nodes (46): $(), a(), ae(), be(), C(), ce(), ct(), de() (+38 more)

### Community 1 - "LeetCode Submission Core"
Cohesion: 0.10
Nodes (28): api, createRepoReadme(), decode(), DEFAULT_STATS(), encode(), getAndInitializeStats(), getCustomCommitMessage(), getGitHubFile() (+20 more)

### Community 2 - "Stats and Version Utilities"
Cohesion: 0.06
Nodes (19): incrementStats(), questionSlugToProblemName(), addManualSubmitBtn(), createGitIcon(), createToolTip(), getSubmissionPageBtns(), setupManualSubmitBtn(), addLeadingZeros() (+11 more)

### Community 3 - "package.json Build Deps"
Cohesion: 0.06
Nodes (30): description, devDependencies, chrome-types, copy-webpack-plugin, eslint, filemanager-webpack-plugin, ignore-loader, jasmine (+22 more)

### Community 4 - "README and Popup UI"
Cohesion: 0.20
Nodes (9): Changelog, Credits, Features, Features & Settings, How does LeetHub work?, How to set up LeetHub for local development, pnpm Commands, What is LeetHub? (+1 more)

### Community 5 - "Community 5"
Cohesion: 0.25
Nodes (6): diff, emptyTree, EXCLUDED_PATHS, full, hits, PATTERNS

### Community 6 - "Community 6"
Cohesion: 0.21
Nodes (13): escapeHtml(), DEFAULT_SETTINGS, isOn(), setSwitch(), updateFolderLivePreview(), updateTimestampExample(), wireConfigsEditForm(), renderConfigsSummary() (+5 more)

### Community 8 - "Webpack Build Config"
Cohesion: 0.29
Nodes (5): __dirname, entries, __filename, folderIgnore, ignore

### Community 16 - "Community 16"
Cohesion: 0.13
Nodes (14): compilerOptions, allowJs, checkJs, esModuleInterop, module, moduleResolution, outDir, rootDir (+6 more)

### Community 19 - "Community 19"
Cohesion: 0.11
Nodes (39): loader(), archiveAndResetStats(), BrowserApi, buildProblemPath(), computeStatsFromReadmes(), encodeJsonContent(), ensureRepoReadme(), fetchRepoContent() (+31 more)

## Knowledge Gaps
- **86 isolated node(s):** `api`, `BackgroundMessage`, `DEFAULT_SETTINGS`, `api`, `welcomeUrl` (+81 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **6 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `$()` connect `jQuery Vendor Bundle` to `Community 19`, `Community 6`?**
  _High betweenness centrality (0.226) - this node is a cross-community bridge._
- **Why does `LeetCodeV2` connect `Stats and Version Utilities` to `LeetCode Submission Core`?**
  _High betweenness centrality (0.059) - this node is a cross-community bridge._
- **Why does `checkModeType()` connect `Community 19` to `jQuery Vendor Bundle`, `Community 6`?**
  _High betweenness centrality (0.059) - this node is a cross-community bridge._
- **Are the 5 inferred relationships involving `$()` (e.g. with `renderStats()` and `checkModeType()`) actually correct?**
  _`$()` has 5 INFERRED edges - model-reasoned connections that need verification._
- **What connects `api`, `BackgroundMessage`, `DEFAULT_SETTINGS` to the rest of the system?**
  _86 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `jQuery Vendor Bundle` be split into smaller, more focused modules?**
  _Cohesion score 0.07393483709273183 - nodes in this community are weakly interconnected._
- **Should `LeetCode Submission Core` be split into smaller, more focused modules?**
  _Cohesion score 0.10338680926916222 - nodes in this community are weakly interconnected._