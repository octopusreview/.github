<p align="center">
  <img src="https://raw.githubusercontent.com/octopusreview/octopus/db9416d102d1ee145c69711e4abe6128c69694e9/apps/web/public/octopus-logo.png" width="72" alt="Octopus" />
</p>

# Code review with your repository in context

Octopus uses indexed code, team standards and repository rules to review pull requests. Get summaries, severity-ranked findings and suggested fixes in GitHub, GitLab and Bitbucket — then explore your codebase from the terminal.

**[Try Octopus Cloud](https://octopus-review.ai/login)** · **[Self-host Octopus](https://octopus-review.ai/docs/self-hosting)** · **[Install the CLI](#review-from-your-terminal)** · **[Read the docs](https://octopus-review.ai/docs)**

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

Use the CLI to review changes and work with repository context. Follow the [CLI guide](https://octopus-review.ai/docs/cli) for authentication, commands and configuration, or [inspect the installer source](https://github.com/octopusreview/octopus/tree/master/apps/cli/install).

## Two ways to use Octopus

| Octopus Cloud | Octopus Self-hosted |
| --- | --- |
| Managed hosting. Sign in, connect your code host and select repositories. | Run Octopus on your own infrastructure with Docker Compose and your chosen AI providers. |
| [Start with Cloud](https://octopus-review.ai/docs/getting-started) · [Pricing](https://octopus-review.ai/docs/pricing) | [Self-hosting guide](https://octopus-review.ai/docs/self-hosting) · [Source and license](https://github.com/octopusreview/octopus) |

## From sign-in to your first review

1. **Sign in to Cloud** and create your organisation.
2. **Connect your code host** and choose the repositories to review.
3. **Open a pull request or merge request.** Read the findings and suggested fixes in your code host.

<p align="center">
  <a href="https://octopus-review.ai/login"><img src="https://raw.githubusercontent.com/octopusreview/octopus/db9416d102d1ee145c69711e4abe6128c69694e9/docs/screenshots/cloud-sign-in.png" width="400" alt="Octopus Cloud sign-in with Google, GitHub, Microsoft or an email magic link" /></a>
</p>

*The real Cloud sign-in screen, captured 11 September 2026. Follow the [Cloud quickstart](https://octopus-review.ai/docs/getting-started) or [self-hosting guide](https://octopus-review.ai/docs/self-hosting) for complete setup.*

## Built around your team's code

- **Context for the review:** indexed repositories, knowledge documents and repository rules.
- **Feedback where you work:** summaries, inline findings and suggested fixes in your code host.
- **Clear review scope:** category scores, severity levels and explicit coverage, including incomplete results.

## Explore and contribute

[Product website](https://octopus-review.ai) · [Documentation](https://octopus-review.ai/docs) · [Source code](https://github.com/octopusreview/octopus) · [Report a bug](https://github.com/octopusreview/octopus/issues) · [Discussions](https://github.com/octopusreview/octopus/discussions) · [What's new](https://octopus-review.ai/docs/changelog)
