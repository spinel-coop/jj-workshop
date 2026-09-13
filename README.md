# jj-workshop

by @kaspth and @indirect, for @spinel-coop

## why is jj

the jujutsu version control system, usually called `jj` after its CLI command name. jj is a new source management tool, compatible with git hosting, but a huge improvement to to actually use. With git, it's easy to dig yourself into a hole that is hard or (in some cases) impossible to get out of. jj is a powerful, simpler, and safer alternative that will help you avoid those version control traps. 

### git is powerful — it’s also complicated, and dangerous 

Git has an entire cottage industry of tools that wrap the git command. lazygit, GitTower, VisualGit, git-flow, GitHub Desktop, and more aliases and scripts than you can possibly shake a stick at. The underlying reason for its cinematic universe of "simplifying" tools is that git is extremely complex. Each command can do a lot of wildly different things, depending on the exact options you pass. On top of that complexity, git is a dangerously sharp knife. You can easily run a git command that permanently changes something about your repo, and get into a state that is hard or maybe even impossible to recover from.

Speaking from my own personal experience, it's always wise to create a complete copy of your .git directory before you do something big and scary like filter-branch or edit commits in the reflog, or do a huge rebase that creates massive conflicts throughout the history of your repo.

The biggest area where git is dangerous is editing history. git doesn't do anything to keep past versions of history around, and while you can sometimes restore past histories using reflog tricks, or even manually walking the tree of discarded commits (that aren't garbage collected yet), it's just not guaranteed.

### jj offers full safety

jj, on the other hand, makes this entire type of work fully safe with a history you can review and revert to at any time. With jj, you have total safety to make any change, including rebase, rewrite, merge, etc, knowing you can always run jj undo as many times as needed.

Git is always able to offer amending, or rebase -i, but editing history (especially if you create conflicts) is extremely messy, and can be especially difficult to undo or repair.

In contrast to git, jj offers the same power, but with clearer commands and a simpler mental model. On top of that simplicity, jj also offers full safety via undo for any command.

Finally, jj offers full compatibility with any git repo. You can personally use jj with any team that uses git. From the perspective of the team or the repo, jj is just another git client. You can gain all of the advantages of jj, without losing anything from GitHub, GitLab, or any other git host.

## what you’ll learn in our workshop

the biggest strengths of jj are clear, safe tools to:

* rebase safely and easily, without breaking your repo
* rewrite history without losing previous versions
* be fully compatible with any git host
* manage source history with confidence

In this workshop, we're going to cover the details of exactly how jj can offer this kind of safety and flexibility. We're also going to show how to use jj to accomplish common git workflows, and cover workflows in jj that are impractical or sometimes even impossible using just git. git is much more powerful than what came before, but can still feel scary and dangerous to use today, 20 years after it was introduced. jj is living proof source control doesn't need to be scary!

After this workshop, you'll have a clear grasp of the conceptual changes jj has made compared to git, and be confident as you manage changes. We'll show exactly how jj provides simplicity, understandability, and safety for your daily work.
