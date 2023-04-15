# Comparing `tmp/mkdocs_terminal-4.2.0.tar.gz` & `tmp/mkdocs_terminal-4.3.0.tar.gz`

## Comparing `mkdocs_terminal-4.2.0.tar` & `mkdocs_terminal-4.3.0.tar`

### file list

```diff
@@ -1,77 +1,79 @@
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/package.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/requirements.txt
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/404.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/__init__.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/base.html
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/main.html
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/mkdocs_theme.yml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/theme_version.html
--rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/normalize.css
--rw-r--r--   0        0        0    17724 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/terminal.css
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/theme.css
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/theme.tile_grid.css
--rw-r--r--   0        0        0   113333 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/fontawesome/css/fontawesome.css
--rw-r--r--   0        0        0    80761 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/fontawesome/css/fontawesome.min.css
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/fontawesome/css/solid.css
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/fontawesome/css/solid.min.css
--rw-r--r--   0        0        0   397420 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/fontawesome/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150516 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/fontawesome/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/palettes/dark.css
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/palettes/default.css
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/palettes/gruvbox_dark.css
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/palettes/pink.css
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/palettes/sans.css
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/palettes/sans_dark.css
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/css/search/bootstrap-modal.css
--rw-r--r--   0        0        0   131637 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/js/bootstrap/bootstrap.js
--rw-r--r--   0        0        0   250568 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/js/bootstrap/bootstrap.js.map
--rw-r--r--   0        0        0    58072 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/js/bootstrap/bootstrap.min.js
--rw-r--r--   0        0        0   190253 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/js/bootstrap/bootstrap.min.js.map
--rw-r--r--   0        0        0   143611 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/js/jquery/jquery-1.10.1.min.js
--rw-r--r--   0        0        0   171718 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/js/jquery/jquery-1.10.1.min.js.map
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/js/mkdocs/LICENSE
--rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/js/mkdocs/base.js
--rw-r--r--   0        0        0    11159 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/legal/legal.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/macros/toc.j2
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/macros/side-nav/section-index-page-title.j2
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/macros/side-nav/side-nav-item-class.j2
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/macros/side-nav/side-nav-item.j2
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/macros/top-nav/search-button.j2
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/favicon.html
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/footer.html
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/html-title.html
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/page-base.html
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/page.html
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/styles.html
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/page-content/after-content.html
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/page-content/before-content.html
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/page-content/content.html
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/page-content/revision.html
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/search/modal.html
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/search/scripts.html
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/search/mkdocs/LICENSE
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/search/mkdocs/search-modal.html
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/side-nav/side-nav-item.html
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/side-nav/side-nav.html
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/side-panel/side-panel.html
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/side-panel/side-toc.html
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/top-nav/menu.html
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/top-nav/search-button.html
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/partials/top-nav/top.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/plugins/md_to_html/__init__.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/plugins/md_to_html/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/pluglets/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/__init__.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/macro.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/main.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/util.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/templates/j2-macros/tile-image.j2
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/templates/j2-macros/tile-link.j2
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/templates/j2-macros/tile-util.j2
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/templates/j2-macros/tile.j2
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/templates/j2-partials/tiles.html
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/LICENSE
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/README.md
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 mkdocs_terminal-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/package.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/requirements.txt
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/404.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/__init__.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/base.html
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/main.html
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/mkdocs_theme.yml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/theme_version.html
+-rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/normalize.css
+-rw-r--r--   0        0        0    17724 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/terminal.css
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/theme.css
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/theme.footer.css
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/theme.tile_grid.css
+-rw-r--r--   0        0        0   113333 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/fontawesome/css/fontawesome.css
+-rw-r--r--   0        0        0    80761 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/fontawesome/css/fontawesome.min.css
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/fontawesome/css/solid.css
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/fontawesome/css/solid.min.css
+-rw-r--r--   0        0        0   397420 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/fontawesome/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150516 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/fontawesome/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/palettes/dark.css
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/palettes/default.css
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/palettes/gruvbox_dark.css
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/palettes/pink.css
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/palettes/sans.css
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/palettes/sans_dark.css
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/css/search/bootstrap-modal.css
+-rw-r--r--   0        0        0   131637 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/js/bootstrap/bootstrap.js
+-rw-r--r--   0        0        0   250568 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/js/bootstrap/bootstrap.js.map
+-rw-r--r--   0        0        0    58072 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/js/bootstrap/bootstrap.min.js
+-rw-r--r--   0        0        0   190253 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/js/bootstrap/bootstrap.min.js.map
+-rw-r--r--   0        0        0   143611 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/js/jquery/jquery-1.10.1.min.js
+-rw-r--r--   0        0        0   171718 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/js/jquery/jquery-1.10.1.min.js.map
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/js/mkdocs/LICENSE
+-rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/js/mkdocs/base.js
+-rw-r--r--   0        0        0    11159 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/legal/legal.md
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/macros/prev-next.j2
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/macros/toc.j2
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/macros/side-nav/section-index-page-title.j2
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/macros/side-nav/side-nav-item-class.j2
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/macros/side-nav/side-nav-item.j2
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/macros/top-nav/search-button.j2
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/favicon.html
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/footer.html
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/html-title.html
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/page-base.html
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/page.html
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/styles.html
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/page-content/after-content.html
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/page-content/before-content.html
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/page-content/content.html
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/page-content/revision.html
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/search/modal.html
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/search/scripts.html
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/search/mkdocs/LICENSE
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/search/mkdocs/search-modal.html
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/side-nav/side-nav-item.html
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/side-nav/side-nav.html
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/side-panel/side-panel.html
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/side-panel/side-toc.html
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/top-nav/menu.html
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/top-nav/search-button.html
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/partials/top-nav/top.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/plugins/md_to_html/__init__.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/plugins/md_to_html/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/pluglets/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/__init__.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/macro.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/main.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/util.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/templates/j2-macros/tile-image.j2
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/templates/j2-macros/tile-link.j2
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/templates/j2-macros/tile-util.j2
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/templates/j2-macros/tile.j2
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/templates/j2-partials/tiles.html
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/LICENSE
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/README.md
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 mkdocs_terminal-4.3.0/PKG-INFO
```

### Comparing `mkdocs_terminal-4.2.0/package.json` & `mkdocs_terminal-4.3.0/package.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'4.3.0'"}*

```diff
@@ -20,9 +20,9 @@
     "name": "mkdocs-terminal",
     "private": true,
     "repository": {
         "type": "git",
         "url": "https://github.com/ntno/mkdocs-terminal.git"
     },
     "scripts": {},
-    "version": "4.2.0"
+    "version": "4.3.0"
 }
```

### Comparing `mkdocs_terminal-4.2.0/terminal/base.html` & `mkdocs_terminal-4.3.0/terminal/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/normalize.css` & `mkdocs_terminal-4.3.0/terminal/css/normalize.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/terminal.css` & `mkdocs_terminal-4.3.0/terminal/css/terminal.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/theme.css` & `mkdocs_terminal-4.3.0/terminal/css/theme.css`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 .terminal-mkdocs-main-grid {
     display: grid;
     grid-column-gap: 1.4em;
     grid-template-columns: auto;
     grid-template-rows: auto;
 }
 
-/* place main content under side nav when screen is too narrow */
+/* place main content to the right of side nav when screen wide enough for two columns */
 @media only screen and (min-width: 70em) {
     .terminal-mkdocs-main-grid {
         grid-template-columns: 4fr 9fr;
     }
 }
 
 .terminal-mkdocs-side-nav-item--active {
```

### Comparing `mkdocs_terminal-4.2.0/terminal/css/theme.tile_grid.css` & `mkdocs_terminal-4.3.0/terminal/css/theme.tile_grid.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/fontawesome/css/fontawesome.css` & `mkdocs_terminal-4.3.0/terminal/css/fontawesome/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/fontawesome/css/fontawesome.min.css` & `mkdocs_terminal-4.3.0/terminal/css/fontawesome/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/fontawesome/css/solid.css` & `mkdocs_terminal-4.3.0/terminal/css/fontawesome/css/solid.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/fontawesome/css/solid.min.css` & `mkdocs_terminal-4.3.0/terminal/css/fontawesome/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/fontawesome/webfonts/fa-solid-900.ttf` & `mkdocs_terminal-4.3.0/terminal/css/fontawesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/fontawesome/webfonts/fa-solid-900.woff2` & `mkdocs_terminal-4.3.0/terminal/css/fontawesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/palettes/dark.css` & `mkdocs_terminal-4.3.0/terminal/css/palettes/dark.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/palettes/default.css` & `mkdocs_terminal-4.3.0/terminal/css/palettes/default.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/palettes/gruvbox_dark.css` & `mkdocs_terminal-4.3.0/terminal/css/palettes/gruvbox_dark.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/palettes/pink.css` & `mkdocs_terminal-4.3.0/terminal/css/palettes/pink.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/palettes/sans.css` & `mkdocs_terminal-4.3.0/terminal/css/palettes/sans.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/palettes/sans_dark.css` & `mkdocs_terminal-4.3.0/terminal/css/palettes/sans_dark.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/css/search/bootstrap-modal.css` & `mkdocs_terminal-4.3.0/terminal/css/search/bootstrap-modal.css`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/js/bootstrap/bootstrap.js` & `mkdocs_terminal-4.3.0/terminal/js/bootstrap/bootstrap.js`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/js/bootstrap/bootstrap.js.map` & `mkdocs_terminal-4.3.0/terminal/js/bootstrap/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/js/bootstrap/bootstrap.min.js` & `mkdocs_terminal-4.3.0/terminal/js/bootstrap/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/js/bootstrap/bootstrap.min.js.map` & `mkdocs_terminal-4.3.0/terminal/js/bootstrap/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/js/jquery/jquery-1.10.1.min.js` & `mkdocs_terminal-4.3.0/terminal/js/jquery/jquery-1.10.1.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/js/jquery/jquery-1.10.1.min.js.map` & `mkdocs_terminal-4.3.0/terminal/js/jquery/jquery-1.10.1.min.js.map`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/js/mkdocs/LICENSE` & `mkdocs_terminal-4.3.0/terminal/js/mkdocs/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/js/mkdocs/base.js` & `mkdocs_terminal-4.3.0/terminal/js/mkdocs/base.js`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/legal/legal.md` & `mkdocs_terminal-4.3.0/terminal/legal/legal.md`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/macros/side-nav/side-nav-item-class.j2` & `mkdocs_terminal-4.3.0/terminal/macros/side-nav/side-nav-item-class.j2`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/macros/side-nav/side-nav-item.j2` & `mkdocs_terminal-4.3.0/terminal/macros/side-nav/side-nav-item.j2`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/partials/favicon.html` & `mkdocs_terminal-4.3.0/terminal/partials/favicon.html`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/partials/page-base.html` & `mkdocs_terminal-4.3.0/terminal/partials/page-base.html`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/partials/styles.html` & `mkdocs_terminal-4.3.0/terminal/partials/styles.html`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 {% set palette = "css/palettes/" ~ palette_name ~ ".css" %}
 <link href="{{ 'css/fontawesome/css/fontawesome.min.css' | url }}" rel="stylesheet">
 <link href="{{ 'css/fontawesome/css/solid.min.css' | url }}" rel="stylesheet">
 <link href="{{ 'css/normalize.css' | url }}" rel="stylesheet">
 <link href="{{ 'css/terminal.css' | url }}" rel="stylesheet">
 <link href="{{ 'css/theme.css' | url }}" rel="stylesheet">
 <link href="{{ 'css/theme.tile_grid.css' | url }}" rel="stylesheet">
+<link href="{{ 'css/theme.footer.css' | url }}" rel="stylesheet">
 <!-- {{ palette_name }} color palette-->
 <link href="{{ palette | url }}" rel="stylesheet">
 {% if 'navigation.top.cursor_animation.hide' in features -%}
 <!-- cursor_animation override -->
 <style>
   #mkdocs-terminal-site-name.terminal-prompt::after {
       display: none;
```

#### html2text {}

```diff
@@ -3,10 +3,11 @@
 palette_name ~ ".css" %}
 
 
 
 
 
 
+
  {% if 'navigation.top.cursor_animation.hide' in features -%}
  {%- endif -%} {% if 'style.links.underline.hide' in features -%}
  {%- endif -%}
```

### Comparing `mkdocs_terminal-4.2.0/terminal/partials/page-content/revision.html` & `mkdocs_terminal-4.3.0/terminal/partials/page-content/revision.html`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/partials/search/mkdocs/LICENSE` & `mkdocs_terminal-4.3.0/terminal/partials/search/mkdocs/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/partials/search/mkdocs/search-modal.html` & `mkdocs_terminal-4.3.0/terminal/partials/search/mkdocs/search-modal.html`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/partials/side-nav/side-nav-item.html` & `mkdocs_terminal-4.3.0/terminal/partials/side-nav/side-nav-item.html`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/partials/top-nav/menu.html` & `mkdocs_terminal-4.3.0/terminal/partials/top-nav/menu.html`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/partials/top-nav/top.html` & `mkdocs_terminal-4.3.0/terminal/partials/top-nav/top.html`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/plugins/md_to_html/plugin.py` & `mkdocs_terminal-4.3.0/terminal/plugins/md_to_html/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/macro.py` & `mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/macro.py`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/util.py` & `mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/util.py`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/templates/j2-macros/tile-util.j2` & `mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/templates/j2-macros/tile-util.j2`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/templates/j2-macros/tile.j2` & `mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/templates/j2-macros/tile.j2`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/terminal/pluglets/tile_grid/templates/j2-partials/tiles.html` & `mkdocs_terminal-4.3.0/terminal/pluglets/tile_grid/templates/j2-partials/tiles.html`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/.gitignore` & `mkdocs_terminal-4.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/LICENSE` & `mkdocs_terminal-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/README.md` & `mkdocs_terminal-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/pyproject.toml` & `mkdocs_terminal-4.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mkdocs_terminal-4.2.0/PKG-INFO` & `mkdocs_terminal-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-terminal
-Version: 4.2.0
+Version: 4.3.0
 Summary: Terminal.css theme for MkDocs
 Project-URL: Repository, https://github.com/ntno/mkdocs-terminal.git
 Author: Natan Organick
 License-Expression: MIT
 License-File: LICENSE
 Keywords: documentation,mkdocs,theme
 Classifier: Development Status :: 4 - Beta
```

