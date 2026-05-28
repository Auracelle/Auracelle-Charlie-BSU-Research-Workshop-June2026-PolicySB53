# Contributing to Auracelle Charlie

Thank you for your interest in Auracelle Charlie. This is an active doctoral research
instrument at Bath Spa University. Contributions are welcome subject to the guidelines below.

---

## What contributions are welcome

### Bug reports
If you encounter a technical issue — JavaScript errors, layout problems, broken
functionality — please open a GitHub Issue with:
- Browser and version (Chrome/Firefox version number)
- Operating system
- Which tab and action triggered the issue
- Screenshot if possible
- The exact error message from the browser console (F12 → Console)

### Scenario and use-case suggestions
If you have domain expertise in AI governance, cybersecurity, nuclear policy, or
autonomous systems and would like to suggest a new governance scenario or validation
case, please open an Issue tagged `enhancement` with a brief description of the
policy instrument and why it merits inclusion.

### Actor pool additions
If you work in a professional sector not currently represented in the actor pools
and can provide accurate governance stances for that sector, please open an Issue
tagged `actor-pool`.

### Translation
If you would like to provide a translated version of the participant instructions
document, please open an Issue tagged `translation` before beginning work.

---

## What contributions are NOT accepted

- Changes to the E-AGPO-HT scoring methodology, BGC domain weights, or NOF taxonomy —
  these are proprietary and under active doctoral research
- Changes to the PSTOA rubric or g-GWC formula
- Commercial feature additions
- Modifications to the Auracelle brand, naming, or visual identity

---

## How to submit a contribution

1. Fork the repository
2. Create a branch: `git checkout -b fix/describe-your-fix`
3. Make your changes
4. Test in Chrome and Firefox
5. Submit a Pull Request with a clear description of what changed and why

---

## Code style

The simulation is a single-file HTML application. When editing:
- Keep JavaScript in the existing `<script>` block
- Do not introduce external dependencies (no npm, no CDN imports)
- Use `safeLocalGet` / `safeLocalSet` / `safeLocalRemove` wrappers for all
  localStorage access (required for Blob URL context compatibility)
- Run `node --check` on the extracted JS before submitting

---

## Research data

Do not commit participant session data (JSON or CSV exports) to this repository.
The `data/` directory is gitignored. Session data should be submitted directly
to the PI per the workshop instructions.

---

## Contact

Grace-Alice Evans — grace-alice.evans@bathspa.ac.uk
