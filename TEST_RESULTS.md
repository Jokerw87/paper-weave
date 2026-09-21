# Actual verification

2026-09-22, Windows, desktop Chromium 151.0.7922.34.

- 6 engine groups PASS: all presets; explicit seam cases; exhaustive independent 4-bit cyclic reference on rows and columns; pure edit/invert invariants; input limits; bounded deterministic dependency-free SVG.
- 6 browser groups PASS: keyboard/undo; all preset sizes; actual JSON roundtrip; downloaded SVG equality and reopened PNG dimension/background; malformed/stale import protection; narrow offline UI with zero application HTTP requests and zero runtime errors.
- 4 boundary groups PASS: size/extension/schema rejection; cancel preserves work; 100-snapshot undo cap; infinite repeat reporting and every reopened PNG pixel equals SVG preview.

Desktop and 390px screenshots inspected. No Android/iOS physical device, screen-reader, physical printing, loom or fabric test. No cross-model review claimed. Only programmatic patterns used.

Source publication and portable packaging are separate steps, pending at this test checkpoint. The above does not claim completion of those steps.
