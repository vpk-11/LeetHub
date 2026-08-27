# Graph Report - leethub  (2026-08-27)

## Corpus Check
- 32 files · ~267,519 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 295 nodes · 570 edges · 17 communities (13 shown, 4 thin omitted)
- Extraction: 94% EXTRACTED · 6% INFERRED · 0% AMBIGUOUS · INFERRED: 32 edges (avg confidence: 0.8)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `0f315719`
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
- [[_COMMUNITY_Feature Request Issue Template|Feature Request Issue Template]]
- [[_COMMUNITY_Community 12|Community 12]]
- [[_COMMUNITY_Community 13|Community 13]]

## God Nodes (most connected - your core abstractions)
1. `$()` - 68 edges
2. `LeetCodeV2` - 22 edges
3. `getBrowser()` - 19 edges
4. `LeetCodeV1` - 18 edges
5. `githubHeaders()` - 17 edges
6. `checkElem()` - 15 edges
7. `compilerOptions` - 12 edges
8. `syncStatsFromRepo()` - 11 edges
9. `scripts` - 10 edges
10. `wireConfigsEditForm()` - 9 edges

## Surprising Connections (you probably didn't know these)
- `renderStats()` --calls--> `$()`  [INFERRED]
  scripts/popup.ts → scripts/jquery-3.3.1.min.js
- `setSyncStatus()` --calls--> `$()`  [INFERRED]
  scripts/welcome.ts → scripts/jquery-3.3.1.min.js
- `updateFolderLivePreview()` --calls--> `$()`  [INFERRED]
  scripts/configsEdit.ts → scripts/jquery-3.3.1.min.js
- `updateTimestampExample()` --calls--> `$()`  [INFERRED]
  scripts/configsEdit.ts → scripts/jquery-3.3.1.min.js
- `wireConfigsEditForm()` --calls--> `$()`  [INFERRED]
  scripts/configsEdit.ts → scripts/jquery-3.3.1.min.js

## Import Cycles
- None detected.

## Communities (17 total, 4 thin omitted)

### Community 0 - "jQuery Vendor Bundle"
Cohesion: 0.09
Nodes (49): Stats, archiveAndResetStats(), BrowserApi, computeStatsFromReadmes(), encodeJsonContent(), ensureRepoReadme(), escapeHtml(), fetchRepoContent() (+41 more)

### Community 1 - "LeetCode Submission Core"
Cohesion: 0.07
Nodes (46): $(), a(), ae(), be(), C(), ce(), ct(), de() (+38 more)

### Community 2 - "Stats and Version Utilities"
Cohesion: 0.06
Nodes (16): incrementStats(), addManualSubmitBtn(), createGitIcon(), createToolTip(), getSubmissionPageBtns(), setupManualSubmitBtn(), checkElem(), formatStats() (+8 more)

### Community 3 - "package.json Build Deps"
Cohesion: 0.09
Nodes (34): api, createRepoReadme(), decode(), DEFAULT_STATS(), encode(), getAndInitializeStats(), getCustomCommitMessage(), getGitHubFile() (+26 more)

### Community 4 - "README and Popup UI"
Cohesion: 0.06
Nodes (30): description, devDependencies, chrome-types, copy-webpack-plugin, eslint, filemanager-webpack-plugin, ignore-loader, jasmine (+22 more)

### Community 5 - "Community 5"
Cohesion: 0.13
Nodes (14): compilerOptions, allowJs, checkJs, esModuleInterop, module, moduleResolution, outDir, rootDir (+6 more)

### Community 6 - "Community 6"
Cohesion: 0.20
Nodes (9): Changelog, Credits, Features, Features & Settings, How does LeetHub work?, How to set up LeetHub for local development, pnpm Commands, What is LeetHub? (+1 more)

### Community 7 - "GeeksforGeeks Support"
Cohesion: 0.25
Nodes (6): diff, emptyTree, EXCLUDED_PATHS, full, hits, PATTERNS

### Community 8 - "Webpack Build Config"
Cohesion: 0.33
Nodes (4): __dirname, __filename, folderIgnore, ignore

## Knowledge Gaps
- **81 isolated node(s):** `name`, `version`, `private`, `description`, `type` (+76 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **4 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `$()` connect `LeetCode Submission Core` to `jQuery Vendor Bundle`?**
  _High betweenness centrality (0.233) - this node is a cross-community bridge._
- **Why does `getBrowser()` connect `jQuery Vendor Bundle` to `package.json Build Deps`?**
  _High betweenness centrality (0.069) - this node is a cross-community bridge._
- **Why does `LeetCodeV2` connect `Stats and Version Utilities` to `package.json Build Deps`?**
  _High betweenness centrality (0.064) - this node is a cross-community bridge._
- **Are the 10 inferred relationships involving `$()` (e.g. with `updateFolderLivePreview()` and `updateTimestampExample()`) actually correct?**
  _`$()` has 10 INFERRED edges - model-reasoned connections that need verification._
- **What connects `name`, `version`, `private` to the rest of the system?**
  _81 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `jQuery Vendor Bundle` be split into smaller, more focused modules?**
  _Cohesion score 0.09316394434361766 - nodes in this community are weakly interconnected._
- **Should `LeetCode Submission Core` be split into smaller, more focused modules?**
  _Cohesion score 0.07393483709273183 - nodes in this community are weakly interconnected._