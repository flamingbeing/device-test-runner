# device-test-runner

Opens web pages in a real iPhone simulator (the actual Mobile Safari app) on a free GitHub macOS runner and returns screenshots.

- Run it from the **Actions** tab → *iOS Safari screenshots* → *Run workflow*, or with `gh workflow run ios-safari.yml -f url=... -f device="iPhone 16"`.
- Inputs: the page address (only `https://anawj.com/...` addresses are accepted), the simulator name, and the hash routes to visit.
- Output: a zip of screenshots (artifact `ios-safari-<device>`, kept 7 days).
- No secrets are used or stored, nothing is pushed anywhere, and runs are manual only.

This repository is public so that macOS runner minutes are free. Keep it free of private material.

Not covered yet: tapping, typing or the on-screen keyboard in Safari. That needs an automation driver (Appium with the XCUITest driver) and would be a second workflow.
