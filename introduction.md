#1 — Design goals (brief)

Precise, reproducible placement of values on any multi-page scanned/form PDF.

Deterministic formatting (numbers, dates, padding, fonts, alignment).

Stable references into nested data using JSONPath-like expressions.

Fallback anchoring to OCR text/keypoints for variable templates.

Machine- and human-readable (JSON) with optional language bindings.

2 — Units & coordinate system

Units: PDF points (default) — 1 point = 1/72 inch. Also support "unit":"percent" for relative layout.

Coordinate origin: top-left of page (x increases right, y increases down). Pages are 1-indexed.

Rect: [x, y, width, height] in chosen unit.

DPI note: For scanned images, convert pixels → points with points = pixels * 72 / dpi.
