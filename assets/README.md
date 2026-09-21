# Profile Graphics

`profile-header.svg` and `section-divider.svg` are standalone CSS-animated SVGs. They run as images inside GitHub's README renderer, without JavaScript or external fonts. Their traces are illustrative, not investment-performance charts. Both respect the browser's reduced-motion preference.

The contribution animation is generated with [Platane/snk](https://github.com/Platane/snk). The activity and language cards use [GitHub Stats Extended](https://github.com/stats-organization/github-stats-extended) through its [GitHub Action](https://github.com/stats-organization/github-readme-stats-action). Each project is MIT-licensed.

The [profile graphics workflow](../.github/workflows/profile-graphics.yml) refreshes the six data-driven SVGs daily at 01:23 UTC (09:23 Singapore), when its configuration changes, or on manual dispatch. It uses the repository's built-in `GITHUB_TOKEN`; no personal access token or additional secret is required. Generation failures leave the last committed graphics intact.

The cards show public activity. Language shares use byte counts in owned, non-fork repositories, including notebooks; they are not a proficiency measure and exclude most work in other organizations. The contribution graphic animates the account's GitHub calendar.

The first cards were generated through the same project's public endpoint. Subsequent refreshes run inside GitHub Actions and commit the generated assets here.

The technology badges in `badges/` are static SVGs generated with [Shields.io](https://shields.io/badges/static-badge), using its `for-the-badge` style and [Simple Icons](https://simpleicons.org/) logos where available. They are stored locally so the tools section does not depend on an external badge service at page load. The technologies are drawn from the profile and CV; the badges do not imply certifications or endorsements.
