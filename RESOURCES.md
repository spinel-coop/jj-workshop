- [jj for my workflow](https://matthewkmayer.github.io/blag/public/post/jj-for-my-workflow/)
- [Git comparison](https://docs.jj-vcs.dev/latest/git-comparison/)

For more about jj’s design, concepts, and why they are interesting, check out the blog posts [jj strategy](https://reasonablypolymorphic.com/blog/jj-strategy/), [What I’ve Learned From JJ](https://zerowidth.com/2025/what-ive-learned-from-jj/), [jj init](https://v5.chriskrycho.com/essays/jj-init/), and [jj is great for the wrong reason](https://www.felesatra.moe/blog/2024/12/23/jj-is-great-for-the-wrong-reason). For a quick reference you can refer to later, there’s a single page summary in the [jj cheat sheet PDF](https://justinpombrio.net/src/jj-cheat-sheet.pdf).

For a full review of everything that’s possible with revsets, check out [the revset documentation](https://jj-vcs.github.io/jj/latest/revsets/) and the blog post [Understanding Revsets for a Better JJ Log Output](https://willhbr.net/2024/08/18/understanding-revsets-for-a-better-jj-log-output/).

For more detail comparing and contrasting bookmarks to branches, I recommend the post [Understanding Jujutsu bookmarks](https://neugierig.org/software/blog/2025/08/jj-bookmarks.html).


The previously mentioned [jj cheat sheet PDF](https://justinpombrio.net/src/jj-cheat-sheet.pdf) has a second page, containing a quick summary of each command, what it does, and the arguments it accepts.

If you want to work on multiple branches at once, you will probably also find the articles [Jujutsu Merge Workflow](https://ofcr.se/jujutsu-merge-workflow) and [Jujutsu Megamerges and `jj absorb`](https://v5.chriskrycho.com/journal/jujutsu-megamerges-and-jj-absorb/) interesting.

https://isaaccorbrey.com/notes/jujutsu-megamerges-for-fun-and-profit

There are many new workflows that jj users have already developed, and this brief overview is just the tip of the iceberg. The jj docs include a section on [using jj with GitHub or GitLab](https://jj-vcs.github.io/jj/latest/github/), and there are some great reflections on different workflows in the blog posts  [Jujutsu VCS Introduction and Patterns](https://kubamartin.com/posts/introduction-to-the-jujutsu-vcs/), [Git experts should try Jujutsu](https://pksunkara.com/thoughts/git-experts-should-try-jujutsu/), and [jj tips and tricks](https://zerowidth.com/2025/jj-tips-and-tricks/).

While the [jj template docs](https://jj-vcs.github.io/jj/latest/templates/) are a great reference, they don’t do very much to show off what’s possible by using templates, so we’ll show some examples.

Try out the various [documented template properties](https://jj-vcs.github.io/jj/latest/templates/) yourself! Once you’re happy with a template that you’ve tested, you can add it to your config with a name, and then use it by name.

https://andre.arko.net/2025/10/15/jj-part-4-configuration/

For another perspective on jj configuration, partly overlapping with this post, check out my JJ Con talk, [stupid jj tricks](/2025/09/28/stupid-jj-tricks/).

You can also try reading some jj config files directly, like [my jj config](https://github.com/indirect/dotfiles/blob/main/private_dot_config/private_jj/config.toml), or [thoughtpolice's jj config](https://gist.github.com/thoughtpolice/8f2fd36ae17cd11b8e7bd93a70e31ad6), or [pksunkara's jj config](https://gist.github.com/pksunkara/622bc04242d402c4e43c7328234fd01c).


## Changeset/interdiff code review

- [Reorient GitHub Pull Requests Around Changesets](https://mitchellh.com/writing/github-changesets)
- [Why some of us like "interdiff" code review](https://gist.github.com/thoughtpolice/9c45287550a56b2047c6311fbadebed2)

## Forges

Tangled.sh has shipped [jujutsu on tangled](https://blog.tangled.sh/stacking), allowing pull requests to be reviewed directly as stacked diffs.
GitHub has shipped "stacked PRs", which is more support for the idea of allowing stacked diffs.
