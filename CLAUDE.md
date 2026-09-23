# Global preferences

- Don't add code comments by default. Only add a comment when I explicitly ask for one, or when the code makes a very specific, non-obvious choice that wouldn't be clear from reading it. In particular, never write comments that justify why one tool, library, or approach was chosen over another (unless I explicitly ask). When you think such comment would be valuable, propose adding it and wait for confirmation.

- When a comment is warranted, keep it short and write it in plain natural language. Avoid AI-sounding phrasing like "this is the crux", "the real blocker", "what actually matters", or constructions like "doing this, never that" — those belong in the trash, not in code or prose. A comment should convey intent, or for genuinely complex pieces, a high-level overview. Don't write comments that narrate history (e.g. "increased x from y", "previously this did z") — that narrative belongs in the PR description if it's useful for review, not in the code. 

- PR descriptions should be concise and describe the change itself, not the process of discovering or debugging it. Don't narrate how the issue was found, what was tried, or dead ends along the way.

- When presenting findings, analysis, or review results, lead directly with the result. Do not prefix with framing sentences like "Here's the crux", "Here's the real issue", "The key finding is", etc. Just state the finding.

## Working with git

- When I ask you to **implement** something in a repo, fetch the latest `origin/main` first, then create a fresh branch off it in the existing clone and write the changes there. Never modify existing files or branches I'm already working on unless I explicitly say so. If there are changes needed for files that have already been staged, do not stash and instead ask how to proceed.

- When I ask you to **look for / read** something in the code, use a dedicated clone named `read-only`. Never make changes in it. Before reading, always fetch and update it to the latest `origin/main` so I'm looking at current code. Create it if it doesn't exist yet.
