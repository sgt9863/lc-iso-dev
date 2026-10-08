# Design integration — 2026-10-09

The user requested a consistent DADS-inspired design across sgt9863.com. Adopted the existing textbook direction: blue #0031d8, ink #1a1a1c, white and pale blue surfaces, Japanese sans-serif text at 16px/1.8, underlined links, 44px controls, and a black/yellow focus indicator. References: https://design.digital.go.jp/dads/foundations/color/ and https://design.digital.go.jp/dads/components/button/ . This is an independent application of the guidance, not a conformance certification.

Static teaching pages share docs/dads.css and domain navigation. Existing dark preferences remain supported. Tables and display equations scroll within the narrow screen. Streamlit styling and local theme were edited in app.py and .streamlit/config.toml, then docs/app.html was regenerated with tools/build_stlite.py. Build self-checks passed (JS syntax, embedded source roundtrip and JS evaluation). Numerical scripts, input data, and teaching content were unchanged. No publication has been performed by this worker.

Browser check: Chrome loaded both generated Streamlit apps without page errors, and their domain-home link was present after Python startup. Both static teaching pages were checked at 390px with no document overflow. Existing Streamlit controls are preserved; exhaustive optimization runs, mobile Streamlit interaction and assistive-technology testing are not claimed.

User follow-up: site-specific primary colors. LC notes and optimizer use warm brown-orange #9c3b00 (white contrast6.91), with matching pale/dark surfaces. The app was rebuilt from the same source; no numerical changes.
