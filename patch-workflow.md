# Patch workflow

1. BEFORE STARTING, make sure you have as much of the requirements as you need. Try to mentally work through the problem, and clear up any gaps with PM and/or UX.
2. Mark ticket as 'In Progress' on Jira. Make sure the ticket has appropriate story points, has dev team marked as DMP, and is assigned to the current sprint.
3. Implementation, with tests where appropriate.
4. Before committing, self-review, undo any irrelevant changes, and document changes in a detailed commit message with a `TESTS` statement.
5. Make sure the precommit hook passes (`eslint`). Make sure your tests pass. MAKE SURE TO RUN THE PRECOMMIT HOOK!!
6. Upload to Gerrit with `repo/rrepo/upload.sh master` (or whatever alias).
7. Add reviewers. Ping team channel and individually ping reviewers. You generally don't need more than 10 reviewers ever, try not to spam people. If the patch is part of a larger WIP feature, you can limit reviewers to the most immediately relevant people.
8. Address comments and iterate.
9. Merge. If ticket is an important feature, ping PM. If ticket is an important bugfix, ping QE. Mark ticket as 'Resolved' on JIRA, someone will verify and move it to 'Done'.
