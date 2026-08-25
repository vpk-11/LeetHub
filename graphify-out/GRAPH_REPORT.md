# Graph Report - leethub  (2026-08-26)

## Corpus Check
- 22 files · ~285,308 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 230 nodes · 420 edges · 16 communities (10 shown, 6 thin omitted)
- Extraction: 95% EXTRACTED · 5% INFERRED · 0% AMBIGUOUS · INFERRED: 23 edges (avg confidence: 0.8)
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `46185efd`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- [[_COMMUNITY_jQuery Vendor Bundle|jQuery Vendor Bundle]]
- [[_COMMUNITY_LeetCode Submission Core|LeetCode Submission Core]]
- [[_COMMUNITY_Stats and Version Utilities|Stats and Version Utilities]]
- [[_COMMUNITY_package.json Build Deps|package.json Build Deps]]
- [[_COMMUNITY_README and Popup UI|README and Popup UI]]
- [[_COMMUNITY_Community 5|Community 5]]
- [[_COMMUNITY_GeeksforGeeks Support|GeeksforGeeks Support]]
- [[_COMMUNITY_Webpack Build Config|Webpack Build Config]]
- [[_COMMUNITY_Background Service Worker|Background Service Worker]]
- [[_COMMUNITY_Bug Report Issue Template|Bug Report Issue Template]]
- [[_COMMUNITY_Feature Request Issue Template|Feature Request Issue Template]]
- [[_COMMUNITY_Community 13|Community 13]]
- [[_COMMUNITY_Community 15|Community 15]]
- [[_COMMUNITY_Community 19|Community 19]]

## God Nodes (most connected - your core abstractions)
1. `$()` - 59 edges
2. `LeetCodeV2()` - 21 edges
3. `LeetCodeV1()` - 18 edges
4. `checkElem()` - 14 edges
5. `getBrowser()` - 13 edges
6. `scripts` - 9 edges
7. `Te()` - 9 edges
8. `syncStatsFromRepo()` - 9 edges
9. `updateReadmeTopicTagsWithProblem()` - 8 edges
10. `oe()` - 7 edges

## Surprising Connections (you probably didn't know these)
- `renderStats()` --calls--> `$()`  [INFERRED]
  scripts/popup.js → scripts/jquery-3.3.1.min.js
- `incrementStats()` --calls--> `getDifficulty()`  [EXTRACTED]
  scripts/leetcode/leetcode.js → scripts/leetcode/util.js
- `getAndInitializeStats()` --calls--> `isEmptyObject()`  [EXTRACTED]
  scripts/leetcode/leetcode.js → scripts/leetcode/util.js
- `updateReadmeTopicTagsWithProblem()` --calls--> `appendProblemToReadme()`  [EXTRACTED]
  scripts/leetcode/leetcode.js → scripts/leetcode/readmeTopics.js
- `updateReadmeTopicTagsWithProblem()` --calls--> `sortTopicsInReadme()`  [EXTRACTED]
  scripts/leetcode/leetcode.js → scripts/leetcode/readmeTopics.js

## Import Cycles
- None detected.

## Hyperedges (group relationships)
- **LeetHub Onboarding Flow (Auth, Hook, Commit modes shared across popup and welcome)** — popup_popup_auth_mode, popup_popup_hook_mode, popup_popup_commit_mode, welcome_welcome_auth_mode, welcome_welcome_hook_mode, welcome_welcome_commit_mode [INFERRED 0.85]
- **GitHub Issue Templates (bug and feature reporting)** — issue_template_bug_report_bug_report, issue_template_config_bug_report_form, issue_template_feature_request_feature_request, issue_template_config_issue_template_config [EXTRACTED 1.00]

## Communities (16 total, 6 thin omitted)

### Community 0 - "jQuery Vendor Bundle"
Cohesion: 0.07
Nodes (46): $(), a(), ae(), be(), C(), ce(), ct(), de() (+38 more)

### Community 1 - "LeetCode Submission Core"
Cohesion: 0.12
Nodes (24): api, createRepoReadme(), decode(), encode(), getAndInitializeStats(), getCustomCommitMessage(), getGitHubFile(), getLastCommitMessage() (+16 more)

### Community 2 - "Stats and Version Utilities"
Cohesion: 0.07
Nodes (10): incrementStats(), questionSlugToProblemName(), addLeadingZeros(), checkElem(), convertToSlug(), formatStats(), getDifficulty(), languages (+2 more)

### Community 3 - "package.json Build Deps"
Cohesion: 0.08
Nodes (25): description, devDependencies, chrome-types, copy-webpack-plugin, filemanager-webpack-plugin, ignore-loader, jasmine, prettier (+17 more)

### Community 4 - "README and Popup UI"
Cohesion: 0.22
Nodes (8): Changelog, Credits, Features, How does LeetHub work?, How to set up LeetHub for local development, NPM Commands, What is LeetHub?, Why LeetHub?

### Community 5 - "Community 5"
Cohesion: 0.43
Nodes (5): addManualSubmitBtn(), createGitIcon(), createToolTip(), getSubmissionPageBtns(), setupManualSubmitBtn()

### Community 8 - "Webpack Build Config"
Cohesion: 0.29
Nodes (5): __dirname, entries, __filename, folderIgnore, ignore

### Community 19 - "Community 19"
Cohesion: 0.14
Nodes (29): loader(), archiveAndResetStats(), buildProblemPath(), computeStatsFromReadmes(), encodeJsonContent(), ensureRepoReadme(), fetchRepoContent(), getBrowser() (+21 more)

## Knowledge Gaps
- **46 isolated node(s):** `name`, `version`, `private`, `description`, `type` (+41 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **6 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `$()` connect `jQuery Vendor Bundle` to `Community 19`?**
  _High betweenness centrality (0.303) - this node is a cross-community bridge._
- **Why does `renderStats()` connect `Community 19` to `jQuery Vendor Bundle`?**
  _High betweenness centrality (0.251) - this node is a cross-community bridge._
- **Why does `LeetCodeV2()` connect `Stats and Version Utilities` to `LeetCode Submission Core`, `Community 5`?**
  _High betweenness centrality (0.076) - this node is a cross-community bridge._
- **What connects `name`, `version`, `private` to the rest of the system?**
  _46 weakly-connected nodes found - possible documentation gaps or missing edges._
- **Should `jQuery Vendor Bundle` be split into smaller, more focused modules?**
  _Cohesion score 0.07393483709273183 - nodes in this community are weakly interconnected._
- **Should `LeetCode Submission Core` be split into smaller, more focused modules?**
  _Cohesion score 0.11827956989247312 - nodes in this community are weakly interconnected._
- **Should `Stats and Version Utilities` be split into smaller, more focused modules?**
  _Cohesion score 0.07419712070874862 - nodes in this community are weakly interconnected._