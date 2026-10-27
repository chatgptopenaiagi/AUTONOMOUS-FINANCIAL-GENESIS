# Contributing

Documentation corrections, clearer explanations and focused technical proposals are welcome.

1. Read the [README](README.md), [architecture](ARCHITECTURE.md) and relevant [knowledge-index](KNOWLEDGE-INDEX.md) entries.
2. Open an issue or make a small pull request explaining the problem and the proposed improvement.
3. Label historical evidence, new verification and future ideas clearly. For technical claims, include the source, date, tested scope and limitations.
4. Check relative links, Markdown formatting and any edited JSON before submitting.

Keep changes lightweight. Documentation contributions do not require installing the financial platform or running its regression suites. If Python is already available, `python -m json.tool verification-summary.json` can check the summary's JSON syntax; it does not reverify historical results.

Never include credentials, account identifiers, private configuration, operational databases or confidential logs. Historical source paths are references, not instructions to copy private environments. Do not turn documentation examples into financial execution commands.

Implementation proposals should explain which existing component they extend, what source access is available, the smallest necessary dependency set and how the change could be verified. See the [continuation guide](CONTINUATION-GUIDE.md). This repository does not distribute the complete platform; upstream source and licensing requirements remain separate.
