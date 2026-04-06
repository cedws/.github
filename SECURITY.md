If you have a security concern or believe you have found a vulnerability in this project, please read out to the email in my GitHub profile.

I take supply chain security very seriously and have implemented measures to protect downstream users. This includes but is not limited to:

* Enabled [Immutable Releases](https://docs.github.com/en/code-security/concepts/supply-chain-security/immutable-releases) (from March 2026)
* Enabled [`Require actions to be pinned to a full-length commit SHA`](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/enabling-features-for-your-repository/managing-github-actions-settings-for-a-repository#managing-github-actions-permissions-for-your-repository)
* Enabled [Secret Protection](https://docs.github.com/en/code-security/how-tos/secure-at-scale/configure-organization-security/configure-specific-tools/protect-your-secrets) in all repositories
* Disabled [`Allow GitHub Actions to create and approve pull requests`](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/enabling-features-for-your-repository/managing-github-actions-settings-for-a-repository#preventing-github-actions-from-creating-or-approving-pull-requests) in all repositories
* Set [default workflow permissions](https://docs.github.com/en/actions/tutorials/authenticate-with-github_token#modifying-the-permissions-for-the-github_token) to read-only in all repositories
* Set up container image signing using [Cosign](https://github.com/sigstore/cosign) keyless signing via Sigstore
* Set up [SLSA provenance](https://docs.github.com/en/actions/concepts/security/artifact-attestations) for binaries and container images via GitHub Artifact Attestations
* Created a ruleset in all repositories requiring signed commits (from March 2026)
