# Code Canvas Lite

A local-only WebGL sandbox: code on the left, live canvas on the right. Templates: a three.js spinning cube and a fragment shader. Snippets save in the browser.

Safety: user code runs in an iframe with `sandbox="allow-scripts"` (opaque origin) and a CSP of `default-src 'none'`; three.js is vendored (MIT, see vendor/THREE-LICENSE) and passed in as a data: URL through an import map, so the preview has no network, no access to the editor page and no access to saved snippets. Verified headless: localStorage, parent document and fetch are all blocked inside the preview.

Built by Claude with Gemini (spec) and Grok (art) for Ian Sparkman. Status: v0.1, UNVERIFIED on tablets and phones.
