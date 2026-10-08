# 2026-10-09 DADS design update

Source: ../lc-method-dev/app/assets/style.css, app/streamlit_app.py, .streamlit/config.toml and tools/build_stlite.py. Consistent domain-home navigation, DADS blue #0031d8, Japanese sans-serif typography, underlined links, 44px controls and black/yellow focus indicators. Source foundation: https://design.digital.go.jp/dads/ .

The canonical local source had unpublished functional differences from this repository's previous index.html. To avoid publishing unrelated code, ../projects/lc-grad-dads-build was populated from the previous index's embedded py-files JSON and rebuilt with the updated builder and only the style/navigation changes. Comparing embedded files before/after confirms only app/streamlit_app.py and app/assets/style.css changed; numerical modules and all other embedded source files are identical. This snapshot is the build source for this design-only publication. Local canonical source also contains the design change, ready for a later functional release.

Validation: canonical Python core tests passed; generated HTML and embedded-source comparison passed. Browser verification is recorded in the sitewide parent development record. No release was pushed by the LC design worker.
