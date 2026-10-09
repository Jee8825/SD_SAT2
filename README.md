# SD SAT2 — Loop

An animated social media website demo for the **Round 2 low-level design challenge**.

The project is in [`social-round2-demo`](social-round2-demo). See its [README](social-round2-demo/README.md) for the requested features, API-design coverage, and demo limitations.

## Run

```sh
cd social-round2-demo
python3 -m http.server 4174 --bind 127.0.0.1 --directory dist
```

Open http://127.0.0.1:4174.

This is a frontend demo: REST calls and notifications are simulated, and demo data is saved in the browser.
