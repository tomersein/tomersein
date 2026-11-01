### Hi, I'm Tomer

I work on open-source tools for software supply chain security, mostly in Go.

My main project is [zanadir](https://github.com/MustacheCase/zanadir). It grades whether a repository's CI can actually fail the build: it finds the checks that are missing (security scanning, linting, tests and so on) and the ones wired so they can never block a merge, then suggests open-source tools to close the gaps. You can [scan a repository in your browser](https://mustachecase.github.io/scan/) with nothing to install, or run it in CI with the [GitHub Action](https://github.com/MustacheCase/zanadir-action).

[![zanadir: scan this CI](https://img.shields.io/badge/zanadir-scan_this_CI-b4441f)](https://mustachecase.github.io/scan/) [![GitHub stars](https://img.shields.io/github/stars/MustacheCase/zanadir?style=flat)](https://github.com/MustacheCase/zanadir)

I also contribute to Anchore's tools, usually when I hit something I need myself:

- **[syft](https://github.com/anchore/syft)**: I added the [`deep-squashed` scope](https://github.com/anchore/syft/pull/3138), which shows every layer a package lives in and not just the final one. Also a [layer size limit](https://github.com/anchore/syft/pull/3464) and support for [`.kar` files](https://github.com/anchore/syft/pull/3113).
- **[grype](https://github.com/anchore/grype)**: I wrote the first version of [`grype db search`](https://github.com/anchore/grype/pull/2031), because I was tired of opening the database in a SQL client just to see if a CVE was in there. Later came [suggested fix versions](https://github.com/anchore/grype/pull/2271) and [end-of-life warnings based on the distro's own `SUPPORT_END` date](https://github.com/anchore/grype/pull/3787).
- **[vunnel](https://github.com/anchore/vunnel)**: I wrote the [end-of-life provider](https://github.com/anchore/vunnel/pull/973), which is where grype's EOL warnings get their data.

If something in zanadir is wrong or missing, open an issue.
