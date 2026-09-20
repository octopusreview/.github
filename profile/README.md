<p align="center">
  <img src="https://raw.githubusercontent.com/octopusreview/octopus/db9416d102d1ee145c69711e4abe6128c69694e9/apps/web/public/octopus-logo.png" width="72" alt="Octopus" />
</p>

# Give your AI this prompt. Let it handle the rest.

Paste the prompt below into the AI coding session you already use for your project. Your agent handles Octopus setup: installing `octp`, indexing the repository and running the analysis. It brings you the links for any approvals it needs along the way.

Octopus reviews pull requests using indexed code, team standards and repository rules. Findings and suggested fixes appear in GitHub, GitLab, Bitbucket and Forgejo.

For Forgejo, [choose your connection](https://octopus-review.ai/docs/integrations#forgejo): Octopus Cloud with public HTTPS, Octopus Cloud with a local connector for private LAN/VPN access, or self-hosted Octopus with direct network access. Both Cloud options send code and review context to Octopus Cloud and your configured AI services. The native agent setup below is for GitHub repositories.

**[Copy the AI prompt](#give-this-prompt-to-your-ai)** · **[Install the CLI](#review-from-your-terminal)** · **[Octopus Cloud](https://octopus-review.ai/login)** · **[Self-host](https://octopus-review.ai/docs/self-hosting)**

## Give this prompt to your AI

Paste this into Codex, Claude Code or another coding agent with terminal access, inside the repository you want to work on:

```text
Set up Octopus for this repository and use its CLI to do the work.

Read https://octopus-review.ai/docs/cli for the current instructions.
Install the standalone octp CLI for this machine if it is missing.
Check octp --help and octp whoami, and use the existing account when available.
If sign-in is needed, run octp login and give me its approval URL.
Guide me through any required GitHub App installation, organisation
authorisation and repository access. Use the setup URLs returned by octp;
if a required link is not available, use the official setup guide.
At each step, give me the exact link and the action I need to take.
After I complete it, recheck access and continue from where you left off.

Identify this repository from its git remote and check octp repo status.
Use octp repo index to index it, wait for completion, then run octp repo analyze.
Check the final status and summarise the architecture and any reported issues.

Use octp commands for indexing, analysis and status checks instead of opening
browser pages to click buttons. Complete each available step yourself.
Ask me only when you need access or a decision you cannot infer.
Report what completed and any remaining blocker.
```

For example, paste this prompt into your existing Codex session and let it set up Octopus for the current project. The agent brings you the links for sign-in, GitHub App authorisation and repository access when needed. Complete the approval, then let it continue with indexing and analysis. You should not have to find settings pages or relay commands between tools.

## See the review, then the fix

[![An Octopus inline review showing the finding, explanation and suggested code change](https://raw.githubusercontent.com/octopusreview/octopus/db9416d102d1ee145c69711e4abe6128c69694e9/docs/screenshots/pr-finding.png)](https://github.com/octopusreview/octopus/pull/744#discussion_r3775719896)

*A real review from [public PR #744](https://github.com/octopusreview/octopus/pull/744#discussion_r3775719896), with the [fix confirmed by the author](https://github.com/octopusreview/octopus/pull/744#discussion_r3775726260). Screenshot captured 11 September 2026.*

### Scores with the reasoning attached

[![Octopus review category scores with notes explaining each score and an overall score of 4 out of 5](https://raw.githubusercontent.com/octopusreview/.github/6860715ee2af85f2de7f73476196df4910c24f40/profile/images/review-scores.png)](https://github.com/octopusreview/octopus/pull/744#issuecomment-5281010601)

*Category scores from the same [public review](https://github.com/octopusreview/octopus/pull/744#issuecomment-5281010601), captured 11 September 2026.*

## Review from your terminal

Install the standalone `octp` binary for macOS, Linux or Windows. No Node.js or npm installation required.

**macOS / Linux**

```bash
curl -fsSL https://octopus-review.ai/install.sh | bash
```

**Windows (PowerShell)**

```powershell
irm https://octopus-review.ai/install.ps1 | iex
```

From your repository directory, your agent can run:

```bash
octp whoami
octp repo status
octp repo index
octp repo analyze
octp repo status
```

To request a pull request review, use `octp review --pr <number-or-url>`.

Follow the [CLI guide](https://octopus-review.ai/docs/cli) for authentication, commands and configuration, or [inspect the installer source](https://github.com/octopusreview/octopus/tree/master/apps/cli/install).

## Two ways to use Octopus

| Octopus Cloud | Octopus Self-hosted |
| --- | --- |
| Managed hosting for Octopus. Give your agent the setup prompt above. | Run Octopus on your own infrastructure with Docker Compose and your chosen AI providers. |
| [Start with Cloud](https://octopus-review.ai/docs/getting-started) · [Pricing](https://octopus-review.ai/docs/pricing) | [Self-hosting guide](https://octopus-review.ai/docs/self-hosting) · [Source and license](https://github.com/octopusreview/octopus) |

## Built around your team's code

- **Context for the review:** indexed repositories, knowledge documents and repository rules.
- **Feedback where you work:** summaries, inline findings and suggested fixes in your code host.
- **Clear review scope:** category scores, severity levels and explicit coverage, including incomplete results.

## Explore and contribute

[Product website](https://octopus-review.ai) · [Documentation](https://octopus-review.ai/docs) · [Source code](https://github.com/octopusreview/octopus) · [Report a bug](https://github.com/octopusreview/octopus/issues) · [Discussions](https://github.com/octopusreview/octopus/discussions) · [What's new](https://octopus-review.ai/docs/changelog)
