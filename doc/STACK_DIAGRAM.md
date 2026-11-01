# Architecture diagrams with stack-diagram

This checkout includes the [stack-diagram](https://github.com/caru-ini/stack-diagram)
agent skill. From this repository, ask:

```text
$stack-diagram Draw an architecture diagram of this repository as HTML and PNG.
```

The skill builds a self-contained HTML file and derives light and dark PNGs
from it. Python 3.9+ and network access to download logos are required.
For PNG export, install Playwright and Chromium in a Python environment:

```sh
python3 -m venv "$HOME/.local/share/stack-diagram/venv"
"$HOME/.local/share/stack-diagram/venv/bin/python" -m pip install playwright
"$HOME/.local/share/stack-diagram/venv/bin/python" -m playwright install chromium
```

Use that environment's Python when running the skill's scripts. The skill
becomes available on the next turn after installation.

The files in `.agents/skills/stack-diagram/` are copied without changes from
[`caru-ini/stack-diagram` at `188f43b7c4f1725a0948feef8b94a199d07e6e0d`](https://github.com/caru-ini/stack-diagram/tree/188f43b7c4f1725a0948feef8b94a199d07e6e0d/skills/stack-diagram).
Keep its MIT license and the bundled fonts' SIL Open Font License notices
when updating the copy.
