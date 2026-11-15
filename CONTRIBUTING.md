# Contributing to BOOTCRAFT

Thank you for helping make operating-system fundamentals easier to understand and safer to practice.

## What we welcome

- Technical corrections with authoritative references
- Persian copy editing and English translations
- Clear diagrams for firmware, partitioning, boot, and recovery
- Better lab checklists and assessment rubrics
- Accessibility, responsive-design, and browser-compatibility fixes
- Disposable VM scenarios that are reproducible and safe

## Ground rules

1. Cite primary or official documentation for technical claims.
2. State the OS version, hardware assumptions, and date when a procedure is version-dependent.
3. Never add destructive commands without a prominent warning, a disposable test environment, and a documented rollback path.
4. Do not ask learners to experiment on personal devices or unknown disks.
5. Never commit passwords, BitLocker recovery keys, personal data, private device identifiers, or copyrighted installation images.
6. Keep Persian content natural and right-to-left; preserve standard command names and code in left-to-right blocks.

## Workflow

1. Open an issue describing the proposed change or correction.
2. Keep pull requests focused and explain the learner benefit.
3. Include screenshots only when they contain no personal or sensitive information.
4. Test the static site locally with `python3 -m http.server 8080`.
5. Confirm that all new links work and the page remains usable on mobile.

## Content review checklist

- [ ] The claim is supported by a primary or authoritative source.
- [ ] Version assumptions are stated.
- [ ] Safety and rollback instructions are present where needed.
- [ ] No secrets or personal information are included.
- [ ] The Persian/English language direction is correct.
