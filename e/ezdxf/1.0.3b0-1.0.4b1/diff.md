# Comparing `tmp/ezdxf-1.0.3b0.zip` & `tmp/ezdxf-1.0.4b1.zip`

## zipinfo {}

```diff
@@ -1,800 +1,821 @@
-Zip file size: 2036488 bytes, number of entries: 798
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/LICENSE
--rw-rw-rw-  2.0 fat      302 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/MANIFEST.in
--rw-rw-rw-  2.0 fat    99043 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/NEWS.md
--rw-rw-rw-  2.0 fat    66793 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/PKG-INFO
--rw-rw-rw-  2.0 fat     5974 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/README.md
--rw-rw-rw-  2.0 fat       37 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/requirements.txt
--rw-rw-rw-  2.0 fat       74 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/setup.cfg
--rw-rw-rw-  2.0 fat     5541 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/
--rw-rw-rw-  2.0 fat      567 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/check_disable_c_ext_by_config_file.py
--rw-rw-rw-  2.0 fat      541 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/check_disable_c_ext_by_env_var.py
--rw-rw-rw-  2.0 fat     1054 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_acad_table.py
--rw-rw-rw-  2.0 fat     4686 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_all_dimline_styles.py
--rw-rw-rw-  2.0 fat     4133 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_all_ellipse_transformations.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_anonymous_blocks.py
--rw-rw-rw-  2.0 fat      871 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_audit_critical_dxf_files.py
--rw-rw-rw-  2.0 fat     1603 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_audit_layouts.py
--rw-rw-rw-  2.0 fat     1726 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_complex_line_type_2.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_create_basic_graphics.py
--rw-rw-rw-  2.0 fat     1921 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_document_guid.py
--rw-rw-rw-  2.0 fat     1832 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_document_page_setup.py
--rw-rw-rw-  2.0 fat      698 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_drawing_matplotlib_backend.py
--rw-rw-rw-  2.0 fat      829 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_drawing_qt_backend.py
--rw-rw-rw-  2.0 fat      998 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_dxf_info_scanning.py
--rw-rw-rw-  2.0 fat     1558 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_entities_iterator.py
--rw-rw-rw-  2.0 fat      934 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_fix_dulicate_handles.py
--rw-rw-rw-  2.0 fat     1901 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_geo.py
--rw-rw-rw-  2.0 fat     1250 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_groups.py
--rw-rw-rw-  2.0 fat      630 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_ignore_junk_beyond_EOF.py
--rw-rw-rw-  2.0 fat     1155 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_launcher.py
--rw-rw-rw-  2.0 fat      631 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_leica_disto_r12.py
--rw-rw-rw-  2.0 fat      737 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_load_dxf_unicode_notation.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_mapbox_earcut.py
--rw-rw-rw-  2.0 fat     1062 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_matplotlib_font_support.py
--rw-rw-rw-  2.0 fat     2230 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_mtext_columns.py
--rw-rw-rw-  2.0 fat     2310 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_mtext_explode_addon.py
--rw-rw-rw-  2.0 fat     1846 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_mtext_text_frame.py
--rw-rw-rw-  2.0 fat     1053 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_new_table_entries.py
--rw-rw-rw-  2.0 fat      887 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_none_ascii_read_write.py
--rw-rw-rw-  2.0 fat     3435 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_odafc.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_open_binary_DXF_files.py
--rw-rw-rw-  2.0 fat      751 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_open_coord_order_issue.py
--rw-rw-rw-  2.0 fat     3842 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_open_exotic_dxf_files.py
--rw-rw-rw-  2.0 fat      879 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_open_R13_R14.py
--rw-rw-rw-  2.0 fat     3152 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_polyline_entity.py
--rw-rw-rw-  2.0 fat     1749 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_preserve_binary_data_in_xrecords.py
--rw-rw-rw-  2.0 fat     6892 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_r12export.py
--rw-rw-rw-  2.0 fat     6256 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_r12strict.py
--rw-rw-rw-  2.0 fat     3410 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_r12writer.py
--rw-rw-rw-  2.0 fat      567 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_read_file_without_handles.py
--rw-rw-rw-  2.0 fat     1121 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_read_write_modern_entites.py
--rw-rw-rw-  2.0 fat     5375 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_recover.py
--rw-rw-rw-  2.0 fat     1959 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_redraw_order.py
--rw-rw-rw-  2.0 fat     1819 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_rotated_block_attributes.py
--rw-rw-rw-  2.0 fat      774 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_surface_entities.py
--rw-rw-rw-  2.0 fat      928 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_write_fixed_meta_data.py
--rw-rw-rw-  2.0 fat     1806 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/test_write_without_handles.py
--rw-rw-rw-  2.0 fat     3060 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/AC1003_LINE_Example.dxf
--rw-rw-rw-  2.0 fat   179505 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/acad_table_with_blk_ref.dxf
--rw-rw-rw-  2.0 fat     7956 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/ASCII_R12.dxf
--rw-rw-rw-  2.0 fat     3761 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/bin_dxf_r12.dxf
--rw-rw-rw-  2.0 fat    20914 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/bin_dxf_r13.dxf
--rw-rw-rw-  2.0 fat    21137 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/bin_dxf_r14.dxf
--rw-rw-rw-  2.0 fat    11564 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/bin_dxf_r2000.dxf
--rw-rw-rw-  2.0 fat     6424 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/cc_dxflib.dxf
--rw-rw-rw-  2.0 fat   173753 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/custom_blocks.dxf
--rw-rw-rw-  2.0 fat    32203 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/duplicate_handles.dxf
--rw-rw-rw-  2.0 fat    18554 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/dxf_unicode.dxf
--rw-rw-rw-  2.0 fat     1592 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/empty_handles.dxf
--rw-rw-rw-  2.0 fat    97103 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/groups.dxf
--rw-rw-rw-  2.0 fat     9146 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/Leica_Disto_S910.dxf
--rw-rw-rw-  2.0 fat    17986 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/MODEL.dxf
--rw-rw-rw-  2.0 fat    25799 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/mtext_columns_R2007.dxf
--rw-rw-rw-  2.0 fat    23927 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/mtext_columns_R2018.dxf
--rw-rw-rw-  2.0 fat    98230 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/mtext_framed_columns.dxf
--rw-rw-rw-  2.0 fat   106574 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/mtext_text_frame.dxf
--rw-rw-rw-  2.0 fat    12001 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/no_layouts.dxf
--rw-rw-rw-  2.0 fat    28788 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/POLI-ALL210_12.DXF
--rw-rw-rw-  2.0 fat      144 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
--rw-rw-rw-  2.0 fat   212407 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/recover01.dxf
--rw-rw-rw-  2.0 fat   115423 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/recover02.dxf
--rw-rw-rw-  2.0 fat    21178 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/small_r13.dxf
--rw-rw-rw-  2.0 fat    10326 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/small_r14.dxf
--rw-rw-rw-  2.0 fat    11286 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/XRECORD_0.bin
--rw-rw-rw-  2.0 fat    11662 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/XRECORD_1.bin
--rw-rw-rw-  2.0 fat    15337 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/integration_tests/data/XRECORD_2.bin
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acis/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/path/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/pp/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/sections/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/
--rw-rw-rw-  2.0 fat     4710 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/appsettings.py
--rw-rw-rw-  2.0 fat    19812 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/audit.py
--rw-rw-rw-  2.0 fat     5912 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/bbox.py
--rw-rw-rw-  2.0 fat     7888 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/blkrefs.py
--rw-rw-rw-  2.0 fat    13157 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/colors.py
--rw-rw-rw-  2.0 fat    31789 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/commands.py
--rw-rw-rw-  2.0 fat     1549 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/comments.py
--rw-rw-rw-  2.0 fat    22095 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/disassemble.py
--rw-rw-rw-  2.0 fat    52604 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/document.py
--rw-rw-rw-  2.0 fat      832 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/dwginfo.py
--rw-rw-rw-  2.0 fat    16248 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entitydb.py
--rw-rw-rw-  2.0 fat     7495 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/enums.py
--rw-rw-rw-  2.0 fat    13948 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/explode.py
--rw-rw-rw-  2.0 fat     1653 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/eztypes.py
--rw-rw-rw-  2.0 fat    10289 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/filemanagement.py
--rw-rw-rw-  2.0 fat    12157 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/gfxattribs.py
--rw-rw-rw-  2.0 fat   107500 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/graphicsfactory.py
--rw-rw-rw-  2.0 fat     3416 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/groupby.py
--rw-rw-rw-  2.0 fat     2567 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/protocols.py
--rw-rw-rw-  2.0 fat    32672 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/proxygraphic.py
--rw-rw-rw-  2.0 fat       95 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/py.typed
--rw-rw-rw-  2.0 fat    22499 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/query.py
--rw-rw-rw-  2.0 fat     2780 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/queryparser.py
--rw-rw-rw-  2.0 fat     9580 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/r12strict.py
--rw-rw-rw-  2.0 fat    30769 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/recover.py
--rw-rw-rw-  2.0 fat     3515 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/reorder.py
--rw-rw-rw-  2.0 fat    30244 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/shapefile.py
--rw-rw-rw-  2.0 fat     5648 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/units.py
--rw-rw-rw-  2.0 fat     8280 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/upright.py
--rw-rw-rw-  2.0 fat     9875 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/urecord.py
--rw-rw-rw-  2.0 fat     1024 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/version.py
--rw-rw-rw-  2.0 fat    62062 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/xref.py
--rw-rw-rw-  2.0 fat     2853 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/zoom.py
--rw-rw-rw-  2.0 fat    12060 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/_options.py
--rw-rw-rw-  2.0 fat     2667 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/__init__.py
--rw-rw-rw-  2.0 fat     2781 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/__main__.py
--rw-rw-rw-  2.0 fat     6072 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/bezier3p.pyx
--rw-rw-rw-  2.0 fat     9983 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/bezier4p.pyx
--rw-rw-rw-  2.0 fat    12964 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/bspline.pyx
--rw-rw-rw-  2.0 fat       90 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/construct.pxd
--rw-rw-rw-  2.0 fat     6584 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/construct.pyx
--rw-rw-rw-  2.0 fat     3113 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/linetypes.pyx
--rw-rw-rw-  2.0 fat    23989 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/mapbox_earcut.pyx
--rw-rw-rw-  2.0 fat      381 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/matrix44.pxd
--rw-rw-rw-  2.0 fat    20892 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/matrix44.pyx
--rw-rw-rw-  2.0 fat     2014 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/vector.pxd
--rw-rw-rw-  2.0 fat    23705 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/vector.pyx
--rw-rw-rw-  2.0 fat     1784 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_cubic_bezier.cpp
--rw-rw-rw-  2.0 fat      599 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_cubic_bezier.hpp
--rw-rw-rw-  2.0 fat      424 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_cubic_bezier.pxd
--rw-rw-rw-  2.0 fat      960 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_quad_bezier.cpp
--rw-rw-rw-  2.0 fat      464 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_quad_bezier.hpp
--rw-rw-rw-  2.0 fat      407 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_quad_bezier.pxd
--rw-rw-rw-  2.0 fat     2135 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_vec3.hpp
--rw-rw-rw-  2.0 fat      572 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_vec3.pxd
--rw-rw-rw-  2.0 fat     1265 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acc/__init__.py
--rw-rw-rw-  2.0 fat     6393 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acis/abstract.py
--rw-rw-rw-  2.0 fat      884 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acis/api.py
--rw-rw-rw-  2.0 fat     5484 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acis/const.py
--rw-rw-rw-  2.0 fat     6726 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acis/dbg.py
--rw-rw-rw-  2.0 fat     2980 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acis/dxf.py
--rw-rw-rw-  2.0 fat    28991 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acis/entities.py
--rw-rw-rw-  2.0 fat     4088 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acis/hdr.py
--rw-rw-rw-  2.0 fat    12823 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acis/mesh.py
--rw-rw-rw-  2.0 fat    18690 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acis/sab.py
--rw-rw-rw-  2.0 fat    13184 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acis/sat.py
--rw-rw-rw-  2.0 fat      115 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/acis/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/acisbrowser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/browser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/dwg/
--rw-rw-rw-  2.0 fat    26402 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/acadctb.py
--rw-rw-rw-  2.0 fat    22229 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/binpacking.py
--rw-rw-rw-  2.0 fat    27692 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/dimlines.py
--rw-rw-rw-  2.0 fat    31371 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/dxf2code.py
--rw-rw-rw-  2.0 fat    22037 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/genetic_algorithm.py
--rw-rw-rw-  2.0 fat    36445 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/geo.py
--rw-rw-rw-  2.0 fat     2674 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/gerber_D6673.py
--rw-rw-rw-  2.0 fat    25472 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/importer.py
--rw-rw-rw-  2.0 fat    17355 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/iterdxf.py
--rw-rw-rw-  2.0 fat     8940 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/menger_sponge.py
--rw-rw-rw-  2.0 fat    24787 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/meshex.py
--rw-rw-rw-  2.0 fat      492 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/mixins.py
--rw-rw-rw-  2.0 fat     6211 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/mtextsurrogate.py
--rw-rw-rw-  2.0 fat    13494 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/mtxpl.py
--rw-rw-rw-  2.0 fat    16449 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/odafc.py
--rw-rw-rw-  2.0 fat     9456 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/openscad.py
--rw-rw-rw-  2.0 fat    15878 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/pycsg.py
--rw-rw-rw-  2.0 fat    22496 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/r12export.py
--rw-rw-rw-  2.0 fat    27198 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/r12writer.py
--rw-rw-rw-  2.0 fat     7615 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/sierpinski_pyramid.py
--rw-rw-rw-  2.0 fat    33167 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/tablepainter.py
--rw-rw-rw-  2.0 fat    13174 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/text2path.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/xqt.py
--rw-rw-rw-  2.0 fat      453 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/__init__.py
--rw-rw-rw-  2.0 fat    10023 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/acisbrowser/browser.py
--rw-rw-rw-  2.0 fat     1907 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/acisbrowser/data.py
--rw-rw-rw-  2.0 fat       64 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/acisbrowser/__init__.py
--rw-rw-rw-  2.0 fat      820 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/browser/bookmarks.py
--rw-rw-rw-  2.0 fat    29403 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/browser/browser.py
--rw-rw-rw-  2.0 fat    14891 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/browser/data.py
--rw-rw-rw-  2.0 fat    10993 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/browser/find_dialog.py
--rw-rw-rw-  2.0 fat     1281 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/browser/loader.py
--rw-rw-rw-  2.0 fat    20974 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/browser/model.py
--rw-rw-rw-  2.0 fat     2214 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/browser/tags.py
--rw-rw-rw-  2.0 fat     1382 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/browser/views.py
--rw-rw-rw-  2.0 fat      133 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/browser/__init__.py
--rw-rw-rw-  2.0 fat     9960 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/backend.py
--rw-rw-rw-  2.0 fat     6737 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/config.py
--rw-rw-rw-  2.0 fat     2058 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/debug_backend.py
--rw-rw-rw-  2.0 fat      503 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/debug_utils.py
--rw-rw-rw-  2.0 fat    39832 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/frontend.py
--rw-rw-rw-  2.0 fat     1823 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/gfxproxy.py
--rw-rw-rw-  2.0 fat    15999 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/matplotlib.py
--rw-rw-rw-  2.0 fat     5477 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/mpl_text_renderer.py
--rw-rw-rw-  2.0 fat     9840 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/mtext_complex.py
--rw-rw-rw-  2.0 fat    14024 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/pillow.py
--rw-rw-rw-  2.0 fat    38021 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/properties.py
--rw-rw-rw-  2.0 fat    13449 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/pyqt.py
--rw-rw-rw-  2.0 fat    16757 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/qtviewer.py
--rw-rw-rw-  2.0 fat     5119 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/qt_text_renderer.py
--rw-rw-rw-  2.0 fat    13658 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/text.py
--rw-rw-rw-  2.0 fat     1132 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/text_renderer.py
--rw-rw-rw-  2.0 fat      344 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/type_hints.py
--rw-rw-rw-  2.0 fat      171 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/drawing/__init__.py
--rw-rw-rw-  2.0 fat     3112 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/dwg/classes_section.py
--rw-rw-rw-  2.0 fat      763 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/dwg/const.py
--rw-rw-rw-  2.0 fat     6091 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/dwg/crc.py
--rw-rw-rw-  2.0 fat     3160 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/dwg/fileheader.py
--rw-rw-rw-  2.0 fat    14851 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/dwg/header_section.py
--rw-rw-rw-  2.0 fat     2976 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/dwg/loader.py
--rw-rw-rw-  2.0 fat      141 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/addons/dwg/__init__.py
--rw-rw-rw-  2.0 fat     4757 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/acad_proxy_entity.py
--rw-rw-rw-  2.0 fat    18315 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/acad_table.py
--rw-rw-rw-  2.0 fat    25923 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/acis.py
--rw-rw-rw-  2.0 fat     4890 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/appdata.py
--rw-rw-rw-  2.0 fat     1954 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/appid.py
--rw-rw-rw-  2.0 fat     4942 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/arc.py
--rw-rw-rw-  2.0 fat    26138 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/attrib.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/block.py
--rw-rw-rw-  2.0 fat    10536 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/blockrecord.py
--rw-rw-rw-  2.0 fat    50143 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/boundary_paths.py
--rw-rw-rw-  2.0 fat     7961 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/circle.py
--rw-rw-rw-  2.0 fat    23664 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/dictionary.py
--rw-rw-rw-  2.0 fat    48743 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/dimension.py
--rw-rw-rw-  2.0 fat    35012 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/dimstyle.py
--rw-rw-rw-  2.0 fat    23829 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/dimstyleoverride.py
--rw-rw-rw-  2.0 fat     4399 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/dxfclass.py
--rw-rw-rw-  2.0 fat    42404 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/dxfentity.py
--rw-rw-rw-  2.0 fat    26923 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/dxfgfx.py
--rw-rw-rw-  2.0 fat    15279 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/dxfgroups.py
--rw-rw-rw-  2.0 fat    23699 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/dxfns.py
--rw-rw-rw-  2.0 fat    13746 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/dxfobj.py
--rw-rw-rw-  2.0 fat    11197 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/ellipse.py
--rw-rw-rw-  2.0 fat     4170 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/factory.py
--rw-rw-rw-  2.0 fat    23785 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/geodata.py
--rw-rw-rw-  2.0 fat     4020 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/gradient.py
--rw-rw-rw-  2.0 fat    12263 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/hatch.py
--rw-rw-rw-  2.0 fat     3944 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/helix.py
--rw-rw-rw-  2.0 fat     4747 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/idbuffer.py
--rw-rw-rw-  2.0 fat    26057 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/image.py
--rw-rw-rw-  2.0 fat    27932 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/insert.py
--rw-rw-rw-  2.0 fat    27834 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/layer.py
--rw-rw-rw-  2.0 fat    14252 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/layout.py
--rw-rw-rw-  2.0 fat    12978 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/leader.py
--rw-rw-rw-  2.0 fat     4718 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/light.py
--rw-rw-rw-  2.0 fat     3718 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/line.py
--rw-rw-rw-  2.0 fat     9677 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/ltype.py
--rw-rw-rw-  2.0 fat    18878 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/lwpolyline.py
--rw-rw-rw-  2.0 fat    19653 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/material.py
--rw-rw-rw-  2.0 fat    18435 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/mesh.py
--rw-rw-rw-  2.0 fat    56877 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/mleader.py
--rw-rw-rw-  2.0 fat    37144 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/mline.py
--rw-rw-rw-  2.0 fat     8385 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/mpolygon.py
--rw-rw-rw-  2.0 fat    47689 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/mtext.py
--rw-rw-rw-  2.0 fat     4351 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/mtext_columns.py
--rw-rw-rw-  2.0 fat     5958 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/objectcollection.py
--rw-rw-rw-  2.0 fat     2111 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/oleframe.py
--rw-rw-rw-  2.0 fat     4332 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/pattern.py
--rw-rw-rw-  2.0 fat     5238 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/point.py
--rw-rw-rw-  2.0 fat    16416 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/polygon.py
--rw-rw-rw-  2.0 fat    40087 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/polyline.py
--rw-rw-rw-  2.0 fat     4822 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/shape.py
--rw-rw-rw-  2.0 fat    10443 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/solid.py
--rw-rw-rw-  2.0 fat    24085 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/spline.py
--rw-rw-rw-  2.0 fat     8246 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/subentity.py
--rw-rw-rw-  2.0 fat     5196 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/sun.py
--rw-rw-rw-  2.0 fat     2449 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/table.py
--rw-rw-rw-  2.0 fat    17602 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/text.py
--rw-rw-rw-  2.0 fat     9105 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/textstyle.py
--rw-rw-rw-  2.0 fat     3597 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/tolerance.py
--rw-rw-rw-  2.0 fat     2703 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/ucs.py
--rw-rw-rw-  2.0 fat    14366 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/underlay.py
--rw-rw-rw-  2.0 fat     6040 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/view.py
--rw-rw-rw-  2.0 fat    27893 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/viewport.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/visualstyle.py
--rw-rw-rw-  2.0 fat     9970 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/vport.py
--rw-rw-rw-  2.0 fat    17024 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/xdata.py
--rw-rw-rw-  2.0 fat     8495 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/xdict.py
--rw-rw-rw-  2.0 fat     3062 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/xline.py
--rw-rw-rw-  2.0 fat     3127 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/entities/__init__.py
--rw-rw-rw-  2.0 fat    16696 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/layouts/base.py
--rw-rw-rw-  2.0 fat     4198 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/layouts/blocklayout.py
--rw-rw-rw-  2.0 fat    29014 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/layouts/layout.py
--rw-rw-rw-  2.0 fat    15314 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/layouts/layouts.py
--rw-rw-rw-  2.0 fat      232 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/layouts/__init__.py
--rw-rw-rw-  2.0 fat     8327 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/attributes.py
--rw-rw-rw-  2.0 fat    16500 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/const.py
--rw-rw-rw-  2.0 fat     1614 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/encoding.py
--rw-rw-rw-  2.0 fat    17013 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/extendedtags.py
--rw-rw-rw-  2.0 fat     5363 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/fileindex.py
--rw-rw-rw-  2.0 fat      727 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/hdrvars.py
--rw-rw-rw-  2.0 fat     5469 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/loader.py
--rw-rw-rw-  2.0 fat     7447 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/packedtags.py
--rw-rw-rw-  2.0 fat     6355 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/repair.py
--rw-rw-rw-  2.0 fat    13058 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/tagger.py
--rw-rw-rw-  2.0 fat    14336 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/tags.py
--rw-rw-rw-  2.0 fat     8952 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/tagwriter.py
--rw-rw-rw-  2.0 fat    12064 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/types.py
--rw-rw-rw-  2.0 fat    17069 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/validator.py
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/lldxf/__init__.py
--rw-rw-rw-  2.0 fat    19193 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/arc.py
--rw-rw-rw-  2.0 fat    16272 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/bbox.py
--rw-rw-rw-  2.0 fat     9318 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/bezier.py
--rw-rw-rw-  2.0 fat     2452 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/bezier_interpolation.py
--rw-rw-rw-  2.0 fat     8730 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/box.py
--rw-rw-rw-  2.0 fat    53488 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/bspline.py
--rw-rw-rw-  2.0 fat     5608 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/bulge.py
--rw-rw-rw-  2.0 fat     9002 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/circle.py
--rw-rw-rw-  2.0 fat    24003 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/clipping.py
--rw-rw-rw-  2.0 fat     4319 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/clustering.py
--rw-rw-rw-  2.0 fat    12228 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/construct2d.py
--rw-rw-rw-  2.0 fat    26265 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/construct3d.py
--rw-rw-rw-  2.0 fat     1283 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/cspline.py
--rw-rw-rw-  2.0 fat     9114 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/curvetools.py
--rw-rw-rw-  2.0 fat    22048 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/ellipse.py
--rw-rw-rw-  2.0 fat     4406 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/eulerspiral.py
--rw-rw-rw-  2.0 fat    38883 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/linalg.py
--rw-rw-rw-  2.0 fat    10231 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/line.py
--rw-rw-rw-  2.0 fat     3053 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/offset2d.py
--rw-rw-rw-  2.0 fat     8256 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/parametrize.py
--rw-rw-rw-  2.0 fat    15602 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/perlin.py
--rw-rw-rw-  2.0 fat    15921 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/polyline.py
--rw-rw-rw-  2.0 fat    11867 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/rtree.py
--rw-rw-rw-  2.0 fat     3910 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/shape.py
--rw-rw-rw-  2.0 fat     2568 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/surfaces.py
--rw-rw-rw-  2.0 fat    12155 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/transformtools.py
--rw-rw-rw-  2.0 fat     3631 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/triangulation.py
--rw-rw-rw-  2.0 fat    16971 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/ucs.py
--rw-rw-rw-  2.0 fat     7253 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/_bezier3p.py
--rw-rw-rw-  2.0 fat    12957 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/_bezier4p.py
--rw-rw-rw-  2.0 fat     9440 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/_bspline.py
--rw-rw-rw-  2.0 fat     7272 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/_construct.py
--rw-rw-rw-  2.0 fat     2261 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/_ctypes.py
--rw-rw-rw-  2.0 fat    24954 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    24783 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/_matrix44.py
--rw-rw-rw-  2.0 fat    25912 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/_vector.py
--rw-rw-rw-  2.0 fat     2003 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/math/__init__.py
--rw-rw-rw-  2.0 fat     1229 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/path/commands.py
--rw-rw-rw-  2.0 fat    38526 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/path/converter.py
--rw-rw-rw-  2.0 fat     6663 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/path/nesting.py
--rw-rw-rw-  2.0 fat    16984 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/path/path.py
--rw-rw-rw-  2.0 fat    10140 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/path/shapes.py
--rw-rw-rw-  2.0 fat    33861 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/path/tools.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/path/__init__.py
--rw-rw-rw-  2.0 fat     2987 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/pp/dxfpp.css
--rw-rw-rw-  2.0 fat     1148 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/pp/dxfpp.html
--rw-rw-rw-  2.0 fat    11304 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/pp/dxfpp.js
--rw-rw-rw-  2.0 fat    17144 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/pp/dxfpp.py
--rw-rw-rw-  2.0 fat     3770 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/pp/pprint.py
--rw-rw-rw-  2.0 fat      812 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/pp/rawpp.css
--rw-rw-rw-  2.0 fat      316 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/pp/rawpp.html
--rw-rw-rw-  2.0 fat     2545 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/pp/rawpp.py
--rw-rw-rw-  2.0 fat     6896 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/pp/reflinks.py
--rw-rw-rw-  2.0 fat      123 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/pp/__init__.py
--rw-rw-rw-  2.0 fat    10070 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/abstract_mtext_renderer.py
--rw-rw-rw-  2.0 fat    20495 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/arrows.py
--rw-rw-rw-  2.0 fat    17749 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/curves.py
--rw-rw-rw-  2.0 fat     4041 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/dimension.py
--rw-rw-rw-  2.0 fat    52028 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/dim_base.py
--rw-rw-rw-  2.0 fat    35702 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/dim_curved.py
--rw-rw-rw-  2.0 fat     6894 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/dim_diameter.py
--rw-rw-rw-  2.0 fat    24751 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/dim_linear.py
--rw-rw-rw-  2.0 fat     8084 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/dim_ordinate.py
--rw-rw-rw-  2.0 fat    20295 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/dim_radius.py
--rw-rw-rw-  2.0 fat    47170 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/forms.py
--rw-rw-rw-  2.0 fat    24198 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/hatching.py
--rw-rw-rw-  2.0 fat     4728 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/leader.py
--rw-rw-rw-  2.0 fat      664 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/linetypes.py
--rw-rw-rw-  2.0 fat    64121 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/mesh.py
--rw-rw-rw-  2.0 fat    60923 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/mleader.py
--rw-rw-rw-  2.0 fat     8437 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/mline.py
--rw-rw-rw-  2.0 fat     2964 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/point.py
--rw-rw-rw-  2.0 fat     8736 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/polyline.py
--rw-rw-rw-  2.0 fat     7886 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/r12spline.py
--rw-rw-rw-  2.0 fat    22541 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/trace.py
--rw-rw-rw-  2.0 fat     2881 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/_linetypes.py
--rw-rw-rw-  2.0 fat      778 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/render/__init__.py
--rw-rw-rw-  2.0 fat     1050 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/16x16.png
--rw-rw-rw-  2.0 fat     1420 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/24x24.png
--rw-rw-rw-  2.0 fat    10638 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/256x256.png
--rw-rw-rw-  2.0 fat     1758 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/32x32.png
--rw-rw-rw-  2.0 fat     2335 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/48x48.png
--rw-rw-rw-  2.0 fat     3050 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/64x64.png
--rw-rw-rw-  2.0 fat     2090 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/icon-copy-64px.png
--rw-rw-rw-  2.0 fat     3109 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/icon-find-64px.png
--rw-rw-rw-  2.0 fat     2388 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/icon-goto-bookmark-64px.png
--rw-rw-rw-  2.0 fat     2519 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/icon-goto-handle-64px.png
--rw-rw-rw-  2.0 fat     2409 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/icon-goto-line-64px.png
--rw-rw-rw-  2.0 fat     2231 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/icon-left-arrow-64px.png
--rw-rw-rw-  2.0 fat     2322 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/icon-next-entity-64px.png
--rw-rw-rw-  2.0 fat     2320 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/icon-prev-entity-64px.png
--rw-rw-rw-  2.0 fat     2244 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/icon-right-arrow-64px.png
--rw-rw-rw-  2.0 fat     2553 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/icon-show-in-tree-64px.png
--rw-rw-rw-  2.0 fat     2373 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/resources/icon-store-bookmark-64px.png
--rw-rw-rw-  2.0 fat    10650 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/sections/acdsdata.py
--rw-rw-rw-  2.0 fat    16508 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/sections/blocks.py
--rw-rw-rw-  2.0 fat    11639 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/sections/classes.py
--rw-rw-rw-  2.0 fat     4137 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/sections/entities.py
--rw-rw-rw-  2.0 fat    11953 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/sections/header.py
--rw-rw-rw-  2.0 fat    60696 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/sections/headervars.py
--rw-rw-rw-  2.0 fat    27009 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/sections/objects.py
--rw-rw-rw-  2.0 fat    26581 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/sections/table.py
--rw-rw-rw-  2.0 fat     5270 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/sections/tables.py
--rw-rw-rw-  2.0 fat       67 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/sections/__init__.py
--rw-rw-rw-  2.0 fat    19711 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/analyze.py
--rw-rw-rw-  2.0 fat    20434 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/binarydata.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/codepage.py
--rw-rw-rw-  2.0 fat     7645 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/complex_ltype.py
--rw-rw-rw-  2.0 fat     1782 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/crypt.py
--rw-rw-rw-  2.0 fat     1511 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/debug.py
--rw-rw-rw-  2.0 fat     2341 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/difftags.py
--rw-rw-rw-  2.0 fat    19686 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/fonts.py
--rw-rw-rw-  2.0 fat    59833 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/font_face_cache.json
--rw-rw-rw-  2.0 fat    75485 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/font_measurement_cache.json
--rw-rw-rw-  2.0 fat     1235 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/handle.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/indexing.py
--rw-rw-rw-  2.0 fat     2145 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/juliandate.py
--rw-rw-rw-  2.0 fat     6166 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/pattern.py
--rw-rw-rw-  2.0 fat     1256 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/rawloader.py
--rw-rw-rw-  2.0 fat   129174 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/standards.py
--rw-rw-rw-  2.0 fat     6049 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/strip.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/test.py
--rw-rw-rw-  2.0 fat    63396 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/text.py
--rw-rw-rw-  2.0 fat    54234 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/text_layout.py
--rw-rw-rw-  2.0 fat     6916 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/text_size.py
--rw-rw-rw-  2.0 fat     3077 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/zipmanager.py
--rw-rw-rw-  2.0 fat   142734 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/_iso_pattern.py
--rw-rw-rw-  2.0 fat     4232 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/_matplotlib_font_support.py
--rw-rw-rw-  2.0 fat     3564 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf/tools/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       47 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf.egg-info/entry_points.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat    66793 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      310 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf.egg-info/requires.txt
--rw-rw-rw-  2.0 fat    30449 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/src/ezdxf.egg-info/top_level.txt
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_09_cython_acceleration/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_10_issues/
--rw-rw-rw-  2.0 fat     2336 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
--rw-rw-rw-  2.0 fat     2599 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
--rw-rw-rw-  2.0 fat     1124 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
--rw-rw-rw-  2.0 fat     5456 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
--rw-rw-rw-  2.0 fat      582 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
--rw-rw-rw-  2.0 fat      473 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
--rw-rw-rw-  2.0 fat    11593 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
--rw-rw-rw-  2.0 fat     1191 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
--rw-rw-rw-  2.0 fat     1033 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
--rw-rw-rw-  2.0 fat     4792 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
--rw-rw-rw-  2.0 fat      989 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
--rw-rw-rw-  2.0 fat     1383 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_018_handle.py
--rw-rw-rw-  2.0 fat     5518 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
--rw-rw-rw-  2.0 fat     8168 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
--rw-rw-rw-  2.0 fat     3787 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
--rw-rw-rw-  2.0 fat      401 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
--rw-rw-rw-  2.0 fat      539 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
--rw-rw-rw-  2.0 fat     2092 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_040_tags.py
--rw-rw-rw-  2.0 fat     3073 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
--rw-rw-rw-  2.0 fat     6419 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
--rw-rw-rw-  2.0 fat     1632 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
--rw-rw-rw-  2.0 fat    11265 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
--rw-rw-rw-  2.0 fat     3363 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
--rw-rw-rw-  2.0 fat     1974 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
--rw-rw-rw-  2.0 fat     2321 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
--rw-rw-rw-  2.0 fat      568 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
--rw-rw-rw-  2.0 fat     8682 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
--rw-rw-rw-  2.0 fat     1051 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
--rw-rw-rw-  2.0 fat     1500 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
--rw-rw-rw-  2.0 fat    11689 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
--rw-rw-rw-  2.0 fat     2893 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_102_appdata.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_103_reactors.py
--rw-rw-rw-  2.0 fat     4001 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_104_extension_dict.py
--rw-rw-rw-  2.0 fat    20860 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_105_xdata.py
--rw-rw-rw-  2.0 fat    14169 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_110_dxfentity.py
--rw-rw-rw-  2.0 fat     2433 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
--rw-rw-rw-  2.0 fat     6781 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
--rw-rw-rw-  2.0 fat      695 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_112b_dxfobj.py
--rw-rw-rw-  2.0 fat     2431 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_113_dxfclass.py
--rw-rw-rw-  2.0 fat     4044 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_114_factory.py
--rw-rw-rw-  2.0 fat     2256 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
--rw-rw-rw-  2.0 fat    15794 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_116_dictionary.py
--rw-rw-rw-  2.0 fat     4999 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
--rw-rw-rw-  2.0 fat     3003 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_120_style_table_entry.py
--rw-rw-rw-  2.0 fat     2943 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
--rw-rw-rw-  2.0 fat      379 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
--rw-rw-rw-  2.0 fat     1113 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_123_view_table_entry.py
--rw-rw-rw-  2.0 fat     8757 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
--rw-rw-rw-  2.0 fat     1698 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_125_image_def.py
--rw-rw-rw-  2.0 fat     1312 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
--rw-rw-rw-  2.0 fat     1430 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_127_raster_variables.py
--rw-rw-rw-  2.0 fat     1540 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_128_pdf_definition.py
--rw-rw-rw-  2.0 fat     2778 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_129_xrecord.py
--rw-rw-rw-  2.0 fat     2423 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_130_id_buffer.py
--rw-rw-rw-  2.0 fat     2470 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_131_field_list.py
--rw-rw-rw-  2.0 fat     2435 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_132_layer_filter.py
--rw-rw-rw-  2.0 fat     2153 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_133_sun.py
--rw-rw-rw-  2.0 fat      852 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_134_material.py
--rw-rw-rw-  2.0 fat    11497 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_135_geo_data.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_136_vba_project.py
--rw-rw-rw-  2.0 fat     3099 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_137_sortentstable.py
--rw-rw-rw-  2.0 fat      704 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
--rw-rw-rw-  2.0 fat     7570 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_139_user_record.py
--rw-rw-rw-  2.0 fat      714 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_140_block_record.py
--rw-rw-rw-  2.0 fat     9153 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
--rw-rw-rw-  2.0 fat     2231 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/conftest.py
--rw-rw-rw-  2.0 fat     6532 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_200_line.py
--rw-rw-rw-  2.0 fat     4273 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_201_point.py
--rw-rw-rw-  2.0 fat     6827 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_202_circle.py
--rw-rw-rw-  2.0 fat     8949 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_203_arc.py
--rw-rw-rw-  2.0 fat     2852 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_204_shape.py
--rw-rw-rw-  2.0 fat     8242 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_205_solid.py
--rw-rw-rw-  2.0 fat     8476 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_206_text.py
--rw-rw-rw-  2.0 fat     4947 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_207_attdef.py
--rw-rw-rw-  2.0 fat     6312 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_208_attrib.py
--rw-rw-rw-  2.0 fat     2671 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_209_vertex.py
--rw-rw-rw-  2.0 fat     5930 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_210_polyline_1.py
--rw-rw-rw-  2.0 fat    13489 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_210_polyline_2.py
--rw-rw-rw-  2.0 fat     6650 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
--rw-rw-rw-  2.0 fat     1780 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
--rw-rw-rw-  2.0 fat     7847 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_211_viewport.py
--rw-rw-rw-  2.0 fat    12629 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_212_insert.py
--rw-rw-rw-  2.0 fat     6024 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_213_minsert.py
--rw-rw-rw-  2.0 fat     3284 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_214_block.py
--rw-rw-rw-  2.0 fat     6882 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_215_dimension.py
--rw-rw-rw-  2.0 fat     4907 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
--rw-rw-rw-  2.0 fat    13186 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
--rw-rw-rw-  2.0 fat     6471 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
--rw-rw-rw-  2.0 fat     5535 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
--rw-rw-rw-  2.0 fat     3056 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
--rw-rw-rw-  2.0 fat     7181 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
--rw-rw-rw-  2.0 fat     2066 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
--rw-rw-rw-  2.0 fat     3615 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
--rw-rw-rw-  2.0 fat     6919 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_221_ellipse.py
--rw-rw-rw-  2.0 fat     2223 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_222_xline.py
--rw-rw-rw-  2.0 fat     1493 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_223_ray.py
--rw-rw-rw-  2.0 fat     2176 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_224_group.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_225_mtext.py
--rw-rw-rw-  2.0 fat    12020 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_226_spline.py
--rw-rw-rw-  2.0 fat     5529 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
--rw-rw-rw-  2.0 fat    10893 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
--rw-rw-rw-  2.0 fat    15116 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_228_mesh.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
--rw-rw-rw-  2.0 fat    21421 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
--rw-rw-rw-  2.0 fat     6587 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
--rw-rw-rw-  2.0 fat     3140 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
--rw-rw-rw-  2.0 fat    12486 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
--rw-rw-rw-  2.0 fat     2274 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_231_underlay.py
--rw-rw-rw-  2.0 fat     5243 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_231_underlay_2.py
--rw-rw-rw-  2.0 fat     2294 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_232_acis.py
--rw-rw-rw-  2.0 fat     6799 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_232_acis_2.py
--rw-rw-rw-  2.0 fat     1854 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_232_surface.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_233_helix.py
--rw-rw-rw-  2.0 fat     2040 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_234_light.py
--rw-rw-rw-  2.0 fat     3806 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_235_leader.py
--rw-rw-rw-  2.0 fat    20392 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_236_multileader.py
--rw-rw-rw-  2.0 fat    10992 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_237_mline.py
--rw-rw-rw-  2.0 fat     2356 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_238_tolerance.py
--rw-rw-rw-  2.0 fat    27392 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
--rw-rw-rw-  2.0 fat     4347 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
--rw-rw-rw-  2.0 fat     1069 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_241_hyperlink.py
--rw-rw-rw-  2.0 fat    11313 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_242_random_transform.py
--rw-rw-rw-  2.0 fat     3725 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_243_replace_entity.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
--rw-rw-rw-  2.0 fat     4456 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_245_wipeout.py
--rw-rw-rw-  2.0 fat     6175 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_246_spline_audit.py
--rw-rw-rw-  2.0 fat     8165 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
--rw-rw-rw-  2.0 fat     6003 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_248_mpolygon.py
--rw-rw-rw-  2.0 fat    13682 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
--rw-rw-rw-  2.0 fat     5713 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
--rw-rw-rw-  2.0 fat     8331 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
--rw-rw-rw-  2.0 fat     7331 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_251_upright.py
--rw-rw-rw-  2.0 fat     4795 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
--rw-rw-rw-  2.0 fat     2082 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_253_ole2frame.py
--rw-rw-rw-  2.0 fat      821 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_254_get_font_name.py
--rw-rw-rw-  2.0 fat     5149 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_300_layout.py
--rw-rw-rw-  2.0 fat     4274 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
--rw-rw-rw-  2.0 fat     5582 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_302_block_references.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
--rw-rw-rw-  2.0 fat      913 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
--rw-rw-rw-  2.0 fat     3279 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
--rw-rw-rw-  2.0 fat     2609 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
--rw-rw-rw-  2.0 fat     2343 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_307_groupby.py
--rw-rw-rw-  2.0 fat    17748 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_308_query.py
--rw-rw-rw-  2.0 fat     6382 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_309_query_parser.py
--rw-rw-rw-  2.0 fat     5031 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
--rw-rw-rw-  2.0 fat     5782 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
--rw-rw-rw-  2.0 fat      647 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_313_redraw_order.py
--rw-rw-rw-  2.0 fat     6128 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
--rw-rw-rw-  2.0 fat     2750 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
--rw-rw-rw-  2.0 fat     5208 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
--rw-rw-rw-  2.0 fat     6795 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
--rw-rw-rw-  2.0 fat     4981 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
--rw-rw-rw-  2.0 fat     2450 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_405_classes.py
--rw-rw-rw-  2.0 fat     9094 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
--rw-rw-rw-  2.0 fat      848 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
--rw-rw-rw-  2.0 fat     3375 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
--rw-rw-rw-  2.0 fat     1433 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
--rw-rw-rw-  2.0 fat     5736 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_410_table.py
--rw-rw-rw-  2.0 fat     6607 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
--rw-rw-rw-  2.0 fat     2246 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
--rw-rw-rw-  2.0 fat    18072 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
--rw-rw-rw-  2.0 fat     4638 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
--rw-rw-rw-  2.0 fat    12336 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
--rw-rw-rw-  2.0 fat     6509 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
--rw-rw-rw-  2.0 fat     5656 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
--rw-rw-rw-  2.0 fat     5434 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
--rw-rw-rw-  2.0 fat      733 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
--rw-rw-rw-  2.0 fat     1240 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
--rw-rw-rw-  2.0 fat     5007 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
--rw-rw-rw-  2.0 fat      769 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
--rw-rw-rw-  2.0 fat     7289 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_424_audit.py
--rw-rw-rw-  2.0 fat     3737 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
--rw-rw-rw-  2.0 fat     2981 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
--rw-rw-rw-  2.0 fat     2416 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
--rw-rw-rw-  2.0 fat     2533 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
--rw-rw-rw-  2.0 fat   112800 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/conftest.py
--rw-rw-rw-  2.0 fat     5510 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_500_units.py
--rw-rw-rw-  2.0 fat     1052 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_501_truecolor.py
--rw-rw-rw-  2.0 fat     1021 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_502_raw_color.py
--rw-rw-rw-  2.0 fat     1695 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_503_indexing.py
--rw-rw-rw-  2.0 fat     1442 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_504_suppress_zeros.py
--rw-rw-rw-  2.0 fat      216 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_506_version.py
--rw-rw-rw-  2.0 fat      579 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_507_dxf_pretty_printer.py
--rw-rw-rw-  2.0 fat      657 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_508_read_zip.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_509_comments.py
--rw-rw-rw-  2.0 fat     1185 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_510_byte_stream.py
--rw-rw-rw-  2.0 fat     4239 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_511_bit_stream.py
--rw-rw-rw-  2.0 fat     5595 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_512_pattern.py
--rw-rw-rw-  2.0 fat     2372 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_513_reorder_entities.py
--rw-rw-rw-  2.0 fat    17710 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_514_text.py
--rw-rw-rw-  2.0 fat     5519 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_515_fonts.py
--rw-rw-rw-  2.0 fat     4002 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_516_zoom.py
--rw-rw-rw-  2.0 fat    34209 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_517_text_layout.py
--rw-rw-rw-  2.0 fat      474 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_518_header_guid.py
--rw-rw-rw-  2.0 fat     3716 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_519_mtext_editor.py
--rw-rw-rw-  2.0 fat     3205 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_520_mtext_context.py
--rw-rw-rw-  2.0 fat    22695 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_521_mtext_parser.py
--rw-rw-rw-  2.0 fat     3863 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_522_text_scanner.py
--rw-rw-rw-  2.0 fat     6202 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_523_text_size.py
--rw-rw-rw-  2.0 fat     5063 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_524_block_reference_manager.py
--rw-rw-rw-  2.0 fat      773 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_525_transparency.py
--rw-rw-rw-  2.0 fat     2133 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_526_explode.py
--rw-rw-rw-  2.0 fat    13521 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_527_gfxattribs.py
--rw-rw-rw-  2.0 fat     2748 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_528_difftags.py
--rw-rw-rw-  2.0 fat     6700 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_529_acis_sat.py
--rw-rw-rw-  2.0 fat     2062 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_530_acis_sab.py
--rw-rw-rw-  2.0 fat    12366 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_531_acis_entities.py
--rw-rw-rw-  2.0 fat     7533 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_532_acis_mesh.py
--rw-rw-rw-  2.0 fat    42518 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_533_shapefiles.py
--rw-rw-rw-  2.0 fat     1034 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_534_dwg_info.py
--rw-rw-rw-  2.0 fat    47921 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_535_xref_basic.py
--rw-rw-rw-  2.0 fat    27614 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_05_tools/test_536_xref_conflict.py
--rw-rw-rw-  2.0 fat     4026 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/conftest.py
--rw-rw-rw-  2.0 fat     7460 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_600_base.py
--rw-rw-rw-  2.0 fat     2098 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_601_bulge.py
--rw-rw-rw-  2.0 fat    14651 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_602_vec3.py
--rw-rw-rw-  2.0 fat     8956 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_603_vec2.py
--rw-rw-rw-  2.0 fat     2801 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_604_banded_matrix.py
--rw-rw-rw-  2.0 fat     9738 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_604_linalg.py
--rw-rw-rw-  2.0 fat    11458 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_605_matrix44.py
--rw-rw-rw-  2.0 fat     5888 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_606_convexhull.py
--rw-rw-rw-  2.0 fat     1010 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_607_perlin_noise.py
--rw-rw-rw-  2.0 fat     3833 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_608_intersection_line_line_2d.py
--rw-rw-rw-  2.0 fat     1676 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_609_point_on_line.py
--rw-rw-rw-  2.0 fat     3171 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_610_ocs.py
--rw-rw-rw-  2.0 fat     7529 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_611_ucs.py
--rw-rw-rw-  2.0 fat     1831 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_612_ucs_pass_trough.py
--rw-rw-rw-  2.0 fat     2586 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_613_point_in_poygon.py
--rw-rw-rw-  2.0 fat    10913 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_614_construct_3d.py
--rw-rw-rw-  2.0 fat      602 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_615_rytz_axis.py
--rw-rw-rw-  2.0 fat     5215 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_616_plane.py
--rw-rw-rw-  2.0 fat      772 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_617_clockwise_orientation.py
--rw-rw-rw-  2.0 fat     6384 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_618_clipping.py
--rw-rw-rw-  2.0 fat    10108 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_619_greiner_hormann.py
--rw-rw-rw-  2.0 fat     2669 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_620_knot.py
--rw-rw-rw-  2.0 fat    19780 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_621_bspline.py
--rw-rw-rw-  2.0 fat     7652 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_622_bsplineu.py
--rw-rw-rw-  2.0 fat    12197 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_623_rbspline.py
--rw-rw-rw-  2.0 fat    10809 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_624_global_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1247 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_626_local_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1967 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_627_bspline_basis.py
--rw-rw-rw-  2.0 fat    10545 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_629_bezier.py
--rw-rw-rw-  2.0 fat    10714 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_630a_bezier4p_base.py
--rw-rw-rw-  2.0 fat    10204 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_630b_bezier4p_functions.py
--rw-rw-rw-  2.0 fat     1683 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_631_euler_spiral.py
--rw-rw-rw-  2.0 fat     4021 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_632_bezier3p.py
--rw-rw-rw-  2.0 fat    19463 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_640_bbox.py
--rw-rw-rw-  2.0 fat     5393 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_641_construction_ray.py
--rw-rw-rw-  2.0 fat     3673 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_642_construction_line.py
--rw-rw-rw-  2.0 fat     9459 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_643_construction_box.py
--rw-rw-rw-  2.0 fat    10941 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_644_construction_circle.py
--rw-rw-rw-  2.0 fat    10988 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_645_construction_arc.py
--rw-rw-rw-  2.0 fat     3422 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_646_offset_vertices_2d.py
--rw-rw-rw-  2.0 fat     7672 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_647_transform_tools.py
--rw-rw-rw-  2.0 fat     8993 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_648_construction_ellipse.py
--rw-rw-rw-  2.0 fat     1991 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_649_nurbs_python_interface.py
--rw-rw-rw-  2.0 fat     4243 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_650_elliptic_arc_span.py
--rw-rw-rw-  2.0 fat     9011 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_651_construction_polyline.py
--rw-rw-rw-  2.0 fat     3168 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_652_approx_param_t.py
--rw-rw-rw-  2.0 fat     5806 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_653_polyline_intersection.py
--rw-rw-rw-  2.0 fat     5193 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_654_rtree.py
--rw-rw-rw-  2.0 fat      788 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_655_dbscan.py
--rw-rw-rw-  2.0 fat      834 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_656_k_means.py
--rw-rw-rw-  2.0 fat     4654 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_657_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    11628 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_658_bevel_tools.py
--rw-rw-rw-  2.0 fat     1875 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
--rw-rw-rw-  2.0 fat     1428 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
--rw-rw-rw-  2.0 fat     1741 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
--rw-rw-rw-  2.0 fat     3307 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_06_math/test_662_is_convex_polygon_2d.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_701_arrows.py
--rw-rw-rw-  2.0 fat    17245 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_702_render_forms.py
--rw-rw-rw-  2.0 fat    34220 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_703_mesh_builder.py
--rw-rw-rw-  2.0 fat     3852 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_704_render_linear_dimension.py
--rw-rw-rw-  2.0 fat     1345 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_705_shape.py
--rw-rw-rw-  2.0 fat      483 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_706_random_path.py
--rw-rw-rw-  2.0 fat     5603 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_707_trace.py
--rw-rw-rw-  2.0 fat    33834 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_708a_path.py
--rw-rw-rw-  2.0 fat    27145 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_708b_path_tools.py
--rw-rw-rw-  2.0 fat     3633 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_708c_matplotlib_path_tools.py
--rw-rw-rw-  2.0 fat     4725 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_708d_qpainter_path_tools.py
--rw-rw-rw-  2.0 fat     4589 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_708e_path_shapes.py
--rw-rw-rw-  2.0 fat     4118 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_708f_path_nesting.py
--rw-rw-rw-  2.0 fat     1308 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_709_linetype_renderer.py
--rw-rw-rw-  2.0 fat     2815 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_711_points.py
--rw-rw-rw-  2.0 fat     6594 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_712_render_curved_dimension.py
--rw-rw-rw-  2.0 fat     1472 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_713_mleader_builder.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_714_mleader_render_engine.py
--rw-rw-rw-  2.0 fat    11778 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_715_hatching.py
--rw-rw-rw-  2.0 fat     2626 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
--rw-rw-rw-  2.0 fat     4771 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_800_mtext_surrogate.py
--rw-rw-rw-  2.0 fat     1352 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_801_r12spline.py
--rw-rw-rw-  2.0 fat     7881 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_802_table_painter.py
--rw-rw-rw-  2.0 fat    12386 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_803_entities_to_code.py
--rw-rw-rw-  2.0 fat     6844 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_804_importer.py
--rw-rw-rw-  2.0 fat     2362 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_805_pycsg.py
--rw-rw-rw-  2.0 fat    15467 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_806_acadctb.py
--rw-rw-rw-  2.0 fat     4860 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_807_dwg_loader_basics.py
--rw-rw-rw-  2.0 fat    10862 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_810_drawing_properties.py
--rw-rw-rw-  2.0 fat    14074 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_811_drawing_frontend.py
--rw-rw-rw-  2.0 fat     4157 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
--rw-rw-rw-  2.0 fat    12547 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_813_geo_interface.py
--rw-rw-rw-  2.0 fat    16289 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_814_text2path.py
--rw-rw-rw-  2.0 fat    16239 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_815_dxf_browser.py
--rw-rw-rw-  2.0 fat    11275 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_816_bin_packing.py
--rw-rw-rw-  2.0 fat    12554 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_817_genetic_algorithm.py
--rw-rw-rw-  2.0 fat     9008 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_818_meshex.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_819_menger_sponge.py
--rw-rw-rw-  2.0 fat     4433 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_08_addons/test_820_openscad.py
--rw-rw-rw-  2.0 fat     2527 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
--rw-rw-rw-  2.0 fat     2199 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
--rw-rw-rw-  2.0 fat     1732 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
--rw-rw-rw-  2.0 fat     3158 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
--rw-rw-rw-  2.0 fat     1452 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
--rw-rw-rw-  2.0 fat     4755 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
--rw-rw-rw-  2.0 fat     2656 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_10_issues/test_issue_414_bbox_calculation.py
--rw-rw-rw-  2.0 fat     1213 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
--rw-rw-rw-  2.0 fat     2268 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_10_issues/test_issue_574_flattening_error.py
--rw-rw-rw-  2.0 fat     1754 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
--rw-rw-rw-  2.0 fat      682 b- defN 23-Mar-12 08:49 ezdxf-1.0.3b0/tests/test_10_issues/test_issue_749_text_layout.py
-798 files, 8500553 bytes uncompressed, 1892716 bytes compressed:  77.7%
+Zip file size: 2070357 bytes, number of entries: 819
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/integration_tests/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/LICENSE
+-rw-rw-rw-  2.0 fat      302 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/MANIFEST.in
+-rw-rw-rw-  2.0 fat    99978 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/NEWS.md
+-rw-rw-rw-  2.0 fat    67799 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/PKG-INFO
+-rw-rw-rw-  2.0 fat     6045 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/README.md
+-rw-rw-rw-  2.0 fat       37 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/requirements.txt
+-rw-rw-rw-  2.0 fat       74 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/setup.cfg
+-rw-rw-rw-  2.0 fat     5563 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/integration_tests/data/
+-rw-rw-rw-  2.0 fat      567 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/check_disable_c_ext_by_config_file.py
+-rw-rw-rw-  2.0 fat      541 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/check_disable_c_ext_by_env_var.py
+-rw-rw-rw-  2.0 fat     1054 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_acad_table.py
+-rw-rw-rw-  2.0 fat     4686 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_all_dimline_styles.py
+-rw-rw-rw-  2.0 fat     4133 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_all_ellipse_transformations.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_anonymous_blocks.py
+-rw-rw-rw-  2.0 fat      871 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_audit_critical_dxf_files.py
+-rw-rw-rw-  2.0 fat     1603 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_audit_layouts.py
+-rw-rw-rw-  2.0 fat     1726 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_complex_line_type_2.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_create_basic_graphics.py
+-rw-rw-rw-  2.0 fat     1921 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_document_guid.py
+-rw-rw-rw-  2.0 fat     1832 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_document_page_setup.py
+-rw-rw-rw-  2.0 fat      698 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_drawing_matplotlib_backend.py
+-rw-rw-rw-  2.0 fat      829 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_drawing_qt_backend.py
+-rw-rw-rw-  2.0 fat      998 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_dxf_info_scanning.py
+-rw-rw-rw-  2.0 fat     1558 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_entities_iterator.py
+-rw-rw-rw-  2.0 fat      934 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_fix_dulicate_handles.py
+-rw-rw-rw-  2.0 fat     1901 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_geo.py
+-rw-rw-rw-  2.0 fat     1250 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_groups.py
+-rw-rw-rw-  2.0 fat      630 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_ignore_junk_beyond_EOF.py
+-rw-rw-rw-  2.0 fat     1155 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_launcher.py
+-rw-rw-rw-  2.0 fat      631 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_leica_disto_r12.py
+-rw-rw-rw-  2.0 fat      737 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_load_dxf_unicode_notation.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat     1062 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_matplotlib_font_support.py
+-rw-rw-rw-  2.0 fat     2230 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_mtext_columns.py
+-rw-rw-rw-  2.0 fat     2310 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_mtext_explode_addon.py
+-rw-rw-rw-  2.0 fat     1846 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_mtext_text_frame.py
+-rw-rw-rw-  2.0 fat     1053 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_new_table_entries.py
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_none_ascii_read_write.py
+-rw-rw-rw-  2.0 fat     3435 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_odafc.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_open_binary_DXF_files.py
+-rw-rw-rw-  2.0 fat      751 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_open_coord_order_issue.py
+-rw-rw-rw-  2.0 fat     3842 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_open_exotic_dxf_files.py
+-rw-rw-rw-  2.0 fat      879 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_open_R13_R14.py
+-rw-rw-rw-  2.0 fat     3152 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_polyline_entity.py
+-rw-rw-rw-  2.0 fat     1749 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_preserve_binary_data_in_xrecords.py
+-rw-rw-rw-  2.0 fat     6892 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_r12export.py
+-rw-rw-rw-  2.0 fat     6256 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_r12strict.py
+-rw-rw-rw-  2.0 fat     3410 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_r12writer.py
+-rw-rw-rw-  2.0 fat      567 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_read_file_without_handles.py
+-rw-rw-rw-  2.0 fat     1121 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_read_write_modern_entites.py
+-rw-rw-rw-  2.0 fat     5375 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_recover.py
+-rw-rw-rw-  2.0 fat     1959 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_redraw_order.py
+-rw-rw-rw-  2.0 fat     1819 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_rotated_block_attributes.py
+-rw-rw-rw-  2.0 fat      774 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_surface_entities.py
+-rw-rw-rw-  2.0 fat      928 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_write_fixed_meta_data.py
+-rw-rw-rw-  2.0 fat     1806 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_write_without_handles.py
+-rw-rw-rw-  2.0 fat     3638 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_xref_detach.py
+-rw-rw-rw-  2.0 fat     3060 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/AC1003_LINE_Example.dxf
+-rw-rw-rw-  2.0 fat   179505 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/acad_table_with_blk_ref.dxf
+-rw-rw-rw-  2.0 fat     7956 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/ASCII_R12.dxf
+-rw-rw-rw-  2.0 fat     3761 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r12.dxf
+-rw-rw-rw-  2.0 fat    20914 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r13.dxf
+-rw-rw-rw-  2.0 fat    21137 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r14.dxf
+-rw-rw-rw-  2.0 fat    11564 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r2000.dxf
+-rw-rw-rw-  2.0 fat     6424 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/cc_dxflib.dxf
+-rw-rw-rw-  2.0 fat   173753 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/custom_blocks.dxf
+-rw-rw-rw-  2.0 fat    32203 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/duplicate_handles.dxf
+-rw-rw-rw-  2.0 fat    18554 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/dxf_unicode.dxf
+-rw-rw-rw-  2.0 fat     1592 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/empty_handles.dxf
+-rw-rw-rw-  2.0 fat    97103 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/groups.dxf
+-rw-rw-rw-  2.0 fat     9146 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/Leica_Disto_S910.dxf
+-rw-rw-rw-  2.0 fat    17986 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/MODEL.dxf
+-rw-rw-rw-  2.0 fat    25799 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/mtext_columns_R2007.dxf
+-rw-rw-rw-  2.0 fat    23927 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/mtext_columns_R2018.dxf
+-rw-rw-rw-  2.0 fat    98230 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/mtext_framed_columns.dxf
+-rw-rw-rw-  2.0 fat   106574 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/mtext_text_frame.dxf
+-rw-rw-rw-  2.0 fat    12001 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/no_layouts.dxf
+-rw-rw-rw-  2.0 fat    28788 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/POLI-ALL210_12.DXF
+-rw-rw-rw-  2.0 fat      144 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+-rw-rw-rw-  2.0 fat   212407 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/recover01.dxf
+-rw-rw-rw-  2.0 fat   115423 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/recover02.dxf
+-rw-rw-rw-  2.0 fat    21178 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/small_r13.dxf
+-rw-rw-rw-  2.0 fat    10326 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/small_r14.dxf
+-rw-rw-rw-  2.0 fat    11286 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/XRECORD_0.bin
+-rw-rw-rw-  2.0 fat    11662 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/XRECORD_1.bin
+-rw-rw-rw-  2.0 fat    15337 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/XRECORD_2.bin
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/acc/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/acis/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/lldxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/path/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/pp/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/resources/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/sections/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/tools/
+-rw-rw-rw-  2.0 fat     4710 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/appsettings.py
+-rw-rw-rw-  2.0 fat    19818 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/audit.py
+-rw-rw-rw-  2.0 fat     5912 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/bbox.py
+-rw-rw-rw-  2.0 fat     7888 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/blkrefs.py
+-rw-rw-rw-  2.0 fat    13157 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/colors.py
+-rw-rw-rw-  2.0 fat    38502 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/commands.py
+-rw-rw-rw-  2.0 fat     1549 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/comments.py
+-rw-rw-rw-  2.0 fat    22100 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/disassemble.py
+-rw-rw-rw-  2.0 fat    52604 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/document.py
+-rw-rw-rw-  2.0 fat      832 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/dwginfo.py
+-rw-rw-rw-  2.0 fat    16248 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entitydb.py
+-rw-rw-rw-  2.0 fat     7495 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/enums.py
+-rw-rw-rw-  2.0 fat    13948 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/explode.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/eztypes.py
+-rw-rw-rw-  2.0 fat    10289 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/filemanagement.py
+-rw-rw-rw-  2.0 fat    12157 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/gfxattribs.py
+-rw-rw-rw-  2.0 fat   107500 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/graphicsfactory.py
+-rw-rw-rw-  2.0 fat     3416 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/groupby.py
+-rw-rw-rw-  2.0 fat     2567 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/protocols.py
+-rw-rw-rw-  2.0 fat    32672 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/proxygraphic.py
+-rw-rw-rw-  2.0 fat       95 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/py.typed
+-rw-rw-rw-  2.0 fat    22499 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/query.py
+-rw-rw-rw-  2.0 fat     2780 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/queryparser.py
+-rw-rw-rw-  2.0 fat     9580 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/r12strict.py
+-rw-rw-rw-  2.0 fat    30769 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/recover.py
+-rw-rw-rw-  2.0 fat     3515 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/reorder.py
+-rw-rw-rw-  2.0 fat    30244 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/shapefile.py
+-rw-rw-rw-  2.0 fat    10364 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/transform.py
+-rw-rw-rw-  2.0 fat     5648 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/units.py
+-rw-rw-rw-  2.0 fat     8280 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/upright.py
+-rw-rw-rw-  2.0 fat     9875 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/urecord.py
+-rw-rw-rw-  2.0 fat     1024 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/version.py
+-rw-rw-rw-  2.0 fat    63359 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/xref.py
+-rw-rw-rw-  2.0 fat     2853 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/zoom.py
+-rw-rw-rw-  2.0 fat    12060 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/_options.py
+-rw-rw-rw-  2.0 fat     2667 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/__init__.py
+-rw-rw-rw-  2.0 fat     2781 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/__main__.py
+-rw-rw-rw-  2.0 fat     6072 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/bezier3p.pyx
+-rw-rw-rw-  2.0 fat     9983 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/bezier4p.pyx
+-rw-rw-rw-  2.0 fat    12964 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/bspline.pyx
+-rw-rw-rw-  2.0 fat       90 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/construct.pxd
+-rw-rw-rw-  2.0 fat     6584 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/construct.pyx
+-rw-rw-rw-  2.0 fat     3113 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/linetypes.pyx
+-rw-rw-rw-  2.0 fat    23989 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/mapbox_earcut.pyx
+-rw-rw-rw-  2.0 fat      381 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/matrix44.pxd
+-rw-rw-rw-  2.0 fat    20892 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/matrix44.pyx
+-rw-rw-rw-  2.0 fat     2014 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/vector.pxd
+-rw-rw-rw-  2.0 fat    23705 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/vector.pyx
+-rw-rw-rw-  2.0 fat     1784 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+-rw-rw-rw-  2.0 fat      599 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+-rw-rw-rw-  2.0 fat      424 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+-rw-rw-rw-  2.0 fat      960 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.cpp
+-rw-rw-rw-  2.0 fat      464 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.hpp
+-rw-rw-rw-  2.0 fat      407 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.pxd
+-rw-rw-rw-  2.0 fat     2135 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_vec3.hpp
+-rw-rw-rw-  2.0 fat      572 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_vec3.pxd
+-rw-rw-rw-  2.0 fat     1265 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/__init__.py
+-rw-rw-rw-  2.0 fat     6393 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/abstract.py
+-rw-rw-rw-  2.0 fat      884 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/api.py
+-rw-rw-rw-  2.0 fat     5484 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/const.py
+-rw-rw-rw-  2.0 fat     6726 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/dbg.py
+-rw-rw-rw-  2.0 fat     2980 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/dxf.py
+-rw-rw-rw-  2.0 fat    28991 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/entities.py
+-rw-rw-rw-  2.0 fat     4088 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/hdr.py
+-rw-rw-rw-  2.0 fat    12823 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/mesh.py
+-rw-rw-rw-  2.0 fat    18690 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/sab.py
+-rw-rw-rw-  2.0 fat    13184 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/sat.py
+-rw-rw-rw-  2.0 fat      115 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/__init__.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/addons/browser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/
+-rw-rw-rw-  2.0 fat    26402 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/acadctb.py
+-rw-rw-rw-  2.0 fat    22229 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/binpacking.py
+-rw-rw-rw-  2.0 fat    27692 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dimlines.py
+-rw-rw-rw-  2.0 fat    31371 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dxf2code.py
+-rw-rw-rw-  2.0 fat    22037 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/genetic_algorithm.py
+-rw-rw-rw-  2.0 fat    36445 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/geo.py
+-rw-rw-rw-  2.0 fat     2674 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/gerber_D6673.py
+-rw-rw-rw-  2.0 fat    25472 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/importer.py
+-rw-rw-rw-  2.0 fat    17355 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/iterdxf.py
+-rw-rw-rw-  2.0 fat     8940 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/menger_sponge.py
+-rw-rw-rw-  2.0 fat    24787 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/meshex.py
+-rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/mixins.py
+-rw-rw-rw-  2.0 fat     6203 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/mtextsurrogate.py
+-rw-rw-rw-  2.0 fat    13494 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/mtxpl.py
+-rw-rw-rw-  2.0 fat    16400 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/odafc.py
+-rw-rw-rw-  2.0 fat     9456 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/openscad.py
+-rw-rw-rw-  2.0 fat    15878 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/pycsg.py
+-rw-rw-rw-  2.0 fat    22496 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/r12export.py
+-rw-rw-rw-  2.0 fat    27198 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/r12writer.py
+-rw-rw-rw-  2.0 fat     7615 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/sierpinski_pyramid.py
+-rw-rw-rw-  2.0 fat    33167 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/tablepainter.py
+-rw-rw-rw-  2.0 fat    13174 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/text2path.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/xqt.py
+-rw-rw-rw-  2.0 fat      453 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/__init__.py
+-rw-rw-rw-  2.0 fat    10023 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/browser.py
+-rw-rw-rw-  2.0 fat     1907 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/data.py
+-rw-rw-rw-  2.0 fat       64 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/__init__.py
+-rw-rw-rw-  2.0 fat      820 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/bookmarks.py
+-rw-rw-rw-  2.0 fat    29403 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/browser.py
+-rw-rw-rw-  2.0 fat    14891 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/data.py
+-rw-rw-rw-  2.0 fat    10993 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/find_dialog.py
+-rw-rw-rw-  2.0 fat     1281 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/loader.py
+-rw-rw-rw-  2.0 fat    20974 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/model.py
+-rw-rw-rw-  2.0 fat     2214 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/tags.py
+-rw-rw-rw-  2.0 fat     1382 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/views.py
+-rw-rw-rw-  2.0 fat      133 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/__init__.py
+-rw-rw-rw-  2.0 fat     9960 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/backend.py
+-rw-rw-rw-  2.0 fat     6737 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/config.py
+-rw-rw-rw-  2.0 fat     2058 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/debug_backend.py
+-rw-rw-rw-  2.0 fat      503 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/debug_utils.py
+-rw-rw-rw-  2.0 fat    39832 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/frontend.py
+-rw-rw-rw-  2.0 fat     1823 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/gfxproxy.py
+-rw-rw-rw-  2.0 fat    15999 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/matplotlib.py
+-rw-rw-rw-  2.0 fat     5477 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/mpl_text_renderer.py
+-rw-rw-rw-  2.0 fat     9840 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/mtext_complex.py
+-rw-rw-rw-  2.0 fat    14024 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/pillow.py
+-rw-rw-rw-  2.0 fat    38021 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/properties.py
+-rw-rw-rw-  2.0 fat    13449 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/pyqt.py
+-rw-rw-rw-  2.0 fat    16757 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/qtviewer.py
+-rw-rw-rw-  2.0 fat     5119 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/qt_text_renderer.py
+-rw-rw-rw-  2.0 fat    13658 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/text.py
+-rw-rw-rw-  2.0 fat     1132 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/text_renderer.py
+-rw-rw-rw-  2.0 fat      344 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/type_hints.py
+-rw-rw-rw-  2.0 fat      171 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/__init__.py
+-rw-rw-rw-  2.0 fat     3112 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/classes_section.py
+-rw-rw-rw-  2.0 fat      763 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/const.py
+-rw-rw-rw-  2.0 fat     6091 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/crc.py
+-rw-rw-rw-  2.0 fat     3160 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/fileheader.py
+-rw-rw-rw-  2.0 fat    14851 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/header_section.py
+-rw-rw-rw-  2.0 fat     2976 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/loader.py
+-rw-rw-rw-  2.0 fat      141 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/__init__.py
+-rw-rw-rw-  2.0 fat     5227 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/api.py
+-rw-rw-rw-  2.0 fat     4863 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/backend.py
+-rw-rw-rw-  2.0 fat      513 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/compiler.py
+-rw-rw-rw-  2.0 fat      571 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/deps.py
+-rw-rw-rw-  2.0 fat     3658 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/dxf_backend.py
+-rw-rw-rw-  2.0 fat    14520 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/interpreter.py
+-rw-rw-rw-  2.0 fat     4835 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/page.py
+-rw-rw-rw-  2.0 fat     3130 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/pdf_backend.py
+-rw-rw-rw-  2.0 fat    11435 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/plotter.py
+-rw-rw-rw-  2.0 fat     1411 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/polygon_buffer.py
+-rw-rw-rw-  2.0 fat     4442 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/properties.py
+-rw-rw-rw-  2.0 fat     3349 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/svg_backend.py
+-rw-rw-rw-  2.0 fat     5291 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/tokenizer.py
+-rw-rw-rw-  2.0 fat      164 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/__init__.py
+-rw-rw-rw-  2.0 fat     4757 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat    18315 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/acad_table.py
+-rw-rw-rw-  2.0 fat    25923 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/acis.py
+-rw-rw-rw-  2.0 fat     4890 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/appdata.py
+-rw-rw-rw-  2.0 fat     1954 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/appid.py
+-rw-rw-rw-  2.0 fat     4942 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/arc.py
+-rw-rw-rw-  2.0 fat    26138 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/attrib.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/block.py
+-rw-rw-rw-  2.0 fat    10536 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/blockrecord.py
+-rw-rw-rw-  2.0 fat    50143 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/boundary_paths.py
+-rw-rw-rw-  2.0 fat     7961 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/circle.py
+-rw-rw-rw-  2.0 fat    23664 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dictionary.py
+-rw-rw-rw-  2.0 fat    48743 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dimension.py
+-rw-rw-rw-  2.0 fat    35012 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dimstyle.py
+-rw-rw-rw-  2.0 fat    23829 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dimstyleoverride.py
+-rw-rw-rw-  2.0 fat     4399 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dxfclass.py
+-rw-rw-rw-  2.0 fat    42404 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dxfentity.py
+-rw-rw-rw-  2.0 fat    26923 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dxfgfx.py
+-rw-rw-rw-  2.0 fat    15279 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dxfgroups.py
+-rw-rw-rw-  2.0 fat    23699 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dxfns.py
+-rw-rw-rw-  2.0 fat    13746 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dxfobj.py
+-rw-rw-rw-  2.0 fat    11186 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/ellipse.py
+-rw-rw-rw-  2.0 fat     4170 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/factory.py
+-rw-rw-rw-  2.0 fat    23785 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/geodata.py
+-rw-rw-rw-  2.0 fat     4020 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/gradient.py
+-rw-rw-rw-  2.0 fat    12263 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/hatch.py
+-rw-rw-rw-  2.0 fat     3944 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/helix.py
+-rw-rw-rw-  2.0 fat     4747 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/idbuffer.py
+-rw-rw-rw-  2.0 fat    26057 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/image.py
+-rw-rw-rw-  2.0 fat    27932 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/insert.py
+-rw-rw-rw-  2.0 fat    27834 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/layer.py
+-rw-rw-rw-  2.0 fat    14252 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/layout.py
+-rw-rw-rw-  2.0 fat    12978 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/leader.py
+-rw-rw-rw-  2.0 fat     4718 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/light.py
+-rw-rw-rw-  2.0 fat     3718 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/line.py
+-rw-rw-rw-  2.0 fat     9677 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/ltype.py
+-rw-rw-rw-  2.0 fat    18878 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/lwpolyline.py
+-rw-rw-rw-  2.0 fat    19653 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/material.py
+-rw-rw-rw-  2.0 fat    18435 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/mesh.py
+-rw-rw-rw-  2.0 fat    57367 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/mleader.py
+-rw-rw-rw-  2.0 fat    37144 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/mline.py
+-rw-rw-rw-  2.0 fat     8385 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/mpolygon.py
+-rw-rw-rw-  2.0 fat    48153 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/mtext.py
+-rw-rw-rw-  2.0 fat     4351 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/mtext_columns.py
+-rw-rw-rw-  2.0 fat     6284 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/objectcollection.py
+-rw-rw-rw-  2.0 fat     2111 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/oleframe.py
+-rw-rw-rw-  2.0 fat     4332 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/pattern.py
+-rw-rw-rw-  2.0 fat     5238 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/point.py
+-rw-rw-rw-  2.0 fat    16416 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/polygon.py
+-rw-rw-rw-  2.0 fat    40087 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/polyline.py
+-rw-rw-rw-  2.0 fat     4822 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/shape.py
+-rw-rw-rw-  2.0 fat    10443 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/solid.py
+-rw-rw-rw-  2.0 fat    24085 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/spline.py
+-rw-rw-rw-  2.0 fat     8246 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/subentity.py
+-rw-rw-rw-  2.0 fat     5196 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/sun.py
+-rw-rw-rw-  2.0 fat     2449 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/table.py
+-rw-rw-rw-  2.0 fat    17602 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/text.py
+-rw-rw-rw-  2.0 fat     9105 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/textstyle.py
+-rw-rw-rw-  2.0 fat     3597 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/tolerance.py
+-rw-rw-rw-  2.0 fat     2703 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/ucs.py
+-rw-rw-rw-  2.0 fat    14366 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/underlay.py
+-rw-rw-rw-  2.0 fat     6040 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/view.py
+-rw-rw-rw-  2.0 fat    27893 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/viewport.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/visualstyle.py
+-rw-rw-rw-  2.0 fat     9970 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/vport.py
+-rw-rw-rw-  2.0 fat    17024 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/xdata.py
+-rw-rw-rw-  2.0 fat     8495 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/xdict.py
+-rw-rw-rw-  2.0 fat     3062 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/xline.py
+-rw-rw-rw-  2.0 fat     3127 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/__init__.py
+-rw-rw-rw-  2.0 fat    16696 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/layouts/base.py
+-rw-rw-rw-  2.0 fat     4343 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/layouts/blocklayout.py
+-rw-rw-rw-  2.0 fat    29014 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/layouts/layout.py
+-rw-rw-rw-  2.0 fat    15314 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/layouts/layouts.py
+-rw-rw-rw-  2.0 fat      232 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/layouts/__init__.py
+-rw-rw-rw-  2.0 fat     8327 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/attributes.py
+-rw-rw-rw-  2.0 fat    16500 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/const.py
+-rw-rw-rw-  2.0 fat     1614 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/encoding.py
+-rw-rw-rw-  2.0 fat    17013 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/extendedtags.py
+-rw-rw-rw-  2.0 fat     5363 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/fileindex.py
+-rw-rw-rw-  2.0 fat      727 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/hdrvars.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/loader.py
+-rw-rw-rw-  2.0 fat     7447 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/packedtags.py
+-rw-rw-rw-  2.0 fat     6355 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/repair.py
+-rw-rw-rw-  2.0 fat    13058 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/tagger.py
+-rw-rw-rw-  2.0 fat    14336 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/tags.py
+-rw-rw-rw-  2.0 fat     8952 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/tagwriter.py
+-rw-rw-rw-  2.0 fat    12064 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/types.py
+-rw-rw-rw-  2.0 fat    17069 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/validator.py
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/__init__.py
+-rw-rw-rw-  2.0 fat    19193 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/arc.py
+-rw-rw-rw-  2.0 fat    16270 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/bbox.py
+-rw-rw-rw-  2.0 fat     9318 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/bezier.py
+-rw-rw-rw-  2.0 fat     2452 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/bezier_interpolation.py
+-rw-rw-rw-  2.0 fat     8730 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/box.py
+-rw-rw-rw-  2.0 fat    53488 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/bspline.py
+-rw-rw-rw-  2.0 fat     5608 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/bulge.py
+-rw-rw-rw-  2.0 fat     9002 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/circle.py
+-rw-rw-rw-  2.0 fat    24003 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/clipping.py
+-rw-rw-rw-  2.0 fat     4319 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/clustering.py
+-rw-rw-rw-  2.0 fat    12236 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/construct2d.py
+-rw-rw-rw-  2.0 fat    26265 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/construct3d.py
+-rw-rw-rw-  2.0 fat     1283 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/cspline.py
+-rw-rw-rw-  2.0 fat     9114 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/curvetools.py
+-rw-rw-rw-  2.0 fat    22048 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/ellipse.py
+-rw-rw-rw-  2.0 fat     4406 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/eulerspiral.py
+-rw-rw-rw-  2.0 fat    38883 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/linalg.py
+-rw-rw-rw-  2.0 fat    10231 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/line.py
+-rw-rw-rw-  2.0 fat     3053 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/offset2d.py
+-rw-rw-rw-  2.0 fat     8256 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/parametrize.py
+-rw-rw-rw-  2.0 fat    15602 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/perlin.py
+-rw-rw-rw-  2.0 fat    15921 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/polyline.py
+-rw-rw-rw-  2.0 fat    11867 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/rtree.py
+-rw-rw-rw-  2.0 fat     3910 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/shape.py
+-rw-rw-rw-  2.0 fat     2568 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/surfaces.py
+-rw-rw-rw-  2.0 fat    12155 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/transformtools.py
+-rw-rw-rw-  2.0 fat     3631 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/triangulation.py
+-rw-rw-rw-  2.0 fat    16971 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/ucs.py
+-rw-rw-rw-  2.0 fat     7253 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_bezier3p.py
+-rw-rw-rw-  2.0 fat    12957 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_bezier4p.py
+-rw-rw-rw-  2.0 fat     9440 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_bspline.py
+-rw-rw-rw-  2.0 fat     7272 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_construct.py
+-rw-rw-rw-  2.0 fat     2261 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_ctypes.py
+-rw-rw-rw-  2.0 fat    24954 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    24783 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_matrix44.py
+-rw-rw-rw-  2.0 fat    25912 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_vector.py
+-rw-rw-rw-  2.0 fat     2003 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/__init__.py
+-rw-rw-rw-  2.0 fat     1229 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/commands.py
+-rw-rw-rw-  2.0 fat    38526 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/converter.py
+-rw-rw-rw-  2.0 fat     6663 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/nesting.py
+-rw-rw-rw-  2.0 fat    16984 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/path.py
+-rw-rw-rw-  2.0 fat    10140 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/shapes.py
+-rw-rw-rw-  2.0 fat    34069 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/tools.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/__init__.py
+-rw-rw-rw-  2.0 fat     2987 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.css
+-rw-rw-rw-  2.0 fat     1148 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.html
+-rw-rw-rw-  2.0 fat    11304 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.js
+-rw-rw-rw-  2.0 fat    17144 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.py
+-rw-rw-rw-  2.0 fat     3770 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/pprint.py
+-rw-rw-rw-  2.0 fat      812 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.css
+-rw-rw-rw-  2.0 fat      316 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.html
+-rw-rw-rw-  2.0 fat     2545 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.py
+-rw-rw-rw-  2.0 fat     6896 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/reflinks.py
+-rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/__init__.py
+-rw-rw-rw-  2.0 fat    10070 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/abstract_mtext_renderer.py
+-rw-rw-rw-  2.0 fat    20495 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/arrows.py
+-rw-rw-rw-  2.0 fat    17749 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/curves.py
+-rw-rw-rw-  2.0 fat     4041 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dimension.py
+-rw-rw-rw-  2.0 fat    52028 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dim_base.py
+-rw-rw-rw-  2.0 fat    35702 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dim_curved.py
+-rw-rw-rw-  2.0 fat     6894 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dim_diameter.py
+-rw-rw-rw-  2.0 fat    24751 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dim_linear.py
+-rw-rw-rw-  2.0 fat     8084 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dim_ordinate.py
+-rw-rw-rw-  2.0 fat    20295 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dim_radius.py
+-rw-rw-rw-  2.0 fat    47170 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/forms.py
+-rw-rw-rw-  2.0 fat    24198 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/hatching.py
+-rw-rw-rw-  2.0 fat     4728 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/leader.py
+-rw-rw-rw-  2.0 fat      664 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/linetypes.py
+-rw-rw-rw-  2.0 fat    64121 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/mesh.py
+-rw-rw-rw-  2.0 fat    60923 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/mleader.py
+-rw-rw-rw-  2.0 fat     8437 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/mline.py
+-rw-rw-rw-  2.0 fat     2964 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/point.py
+-rw-rw-rw-  2.0 fat     8736 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/polyline.py
+-rw-rw-rw-  2.0 fat     7886 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/r12spline.py
+-rw-rw-rw-  2.0 fat    22541 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/trace.py
+-rw-rw-rw-  2.0 fat     2881 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/_linetypes.py
+-rw-rw-rw-  2.0 fat      778 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/__init__.py
+-rw-rw-rw-  2.0 fat     1050 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/16x16.png
+-rw-rw-rw-  2.0 fat     1420 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/24x24.png
+-rw-rw-rw-  2.0 fat    10638 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/256x256.png
+-rw-rw-rw-  2.0 fat     1758 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/32x32.png
+-rw-rw-rw-  2.0 fat     2335 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/48x48.png
+-rw-rw-rw-  2.0 fat     3050 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/64x64.png
+-rw-rw-rw-  2.0 fat     2090 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-copy-64px.png
+-rw-rw-rw-  2.0 fat     3109 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-find-64px.png
+-rw-rw-rw-  2.0 fat     2388 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-bookmark-64px.png
+-rw-rw-rw-  2.0 fat     2519 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-handle-64px.png
+-rw-rw-rw-  2.0 fat     2409 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-line-64px.png
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-left-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2322 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-next-entity-64px.png
+-rw-rw-rw-  2.0 fat     2320 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-prev-entity-64px.png
+-rw-rw-rw-  2.0 fat     2244 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-right-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2553 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-show-in-tree-64px.png
+-rw-rw-rw-  2.0 fat     2373 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-store-bookmark-64px.png
+-rw-rw-rw-  2.0 fat    10650 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/acdsdata.py
+-rw-rw-rw-  2.0 fat    16508 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/blocks.py
+-rw-rw-rw-  2.0 fat    11639 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/classes.py
+-rw-rw-rw-  2.0 fat     4137 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/entities.py
+-rw-rw-rw-  2.0 fat    11953 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/header.py
+-rw-rw-rw-  2.0 fat    60696 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/headervars.py
+-rw-rw-rw-  2.0 fat    27009 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/objects.py
+-rw-rw-rw-  2.0 fat    26581 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/table.py
+-rw-rw-rw-  2.0 fat     5270 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/tables.py
+-rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/__init__.py
+-rw-rw-rw-  2.0 fat    19711 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/analyze.py
+-rw-rw-rw-  2.0 fat    20434 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/binarydata.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/codepage.py
+-rw-rw-rw-  2.0 fat     7645 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/complex_ltype.py
+-rw-rw-rw-  2.0 fat     1782 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/crypt.py
+-rw-rw-rw-  2.0 fat     1511 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/debug.py
+-rw-rw-rw-  2.0 fat     2341 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/difftags.py
+-rw-rw-rw-  2.0 fat    19686 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/fonts.py
+-rw-rw-rw-  2.0 fat    59833 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/font_face_cache.json
+-rw-rw-rw-  2.0 fat    75485 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/font_measurement_cache.json
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/handle.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/indexing.py
+-rw-rw-rw-  2.0 fat     2145 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/juliandate.py
+-rw-rw-rw-  2.0 fat     6166 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/pattern.py
+-rw-rw-rw-  2.0 fat     1256 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/rawloader.py
+-rw-rw-rw-  2.0 fat   129174 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/standards.py
+-rw-rw-rw-  2.0 fat     6049 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/strip.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/test.py
+-rw-rw-rw-  2.0 fat    65395 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/text.py
+-rw-rw-rw-  2.0 fat    54234 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/text_layout.py
+-rw-rw-rw-  2.0 fat     6916 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/text_size.py
+-rw-rw-rw-  2.0 fat     3077 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/zipmanager.py
+-rw-rw-rw-  2.0 fat   142734 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/_iso_pattern.py
+-rw-rw-rw-  2.0 fat     4232 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/_matplotlib_font_support.py
+-rw-rw-rw-  2.0 fat     3564 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat       47 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat    67799 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      342 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat    31202 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/top_level.txt
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_01_dxf_entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_05_tools/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_06_math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_07_render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_08_addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_10_issues/
+-rw-rw-rw-  2.0 fat     2336 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+-rw-rw-rw-  2.0 fat     2599 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+-rw-rw-rw-  2.0 fat     1124 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+-rw-rw-rw-  2.0 fat     5456 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+-rw-rw-rw-  2.0 fat      582 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+-rw-rw-rw-  2.0 fat    11593 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+-rw-rw-rw-  2.0 fat     1191 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+-rw-rw-rw-  2.0 fat     1033 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+-rw-rw-rw-  2.0 fat     4792 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+-rw-rw-rw-  2.0 fat      989 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+-rw-rw-rw-  2.0 fat     1383 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_018_handle.py
+-rw-rw-rw-  2.0 fat     5518 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+-rw-rw-rw-  2.0 fat     8168 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+-rw-rw-rw-  2.0 fat     3787 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+-rw-rw-rw-  2.0 fat      401 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+-rw-rw-rw-  2.0 fat      539 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+-rw-rw-rw-  2.0 fat     2092 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_040_tags.py
+-rw-rw-rw-  2.0 fat     3073 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+-rw-rw-rw-  2.0 fat     6419 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+-rw-rw-rw-  2.0 fat     1632 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+-rw-rw-rw-  2.0 fat    11265 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+-rw-rw-rw-  2.0 fat     3363 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+-rw-rw-rw-  2.0 fat     1974 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+-rw-rw-rw-  2.0 fat     2321 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+-rw-rw-rw-  2.0 fat      568 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+-rw-rw-rw-  2.0 fat     8682 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+-rw-rw-rw-  2.0 fat     1051 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+-rw-rw-rw-  2.0 fat     1500 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+-rw-rw-rw-  2.0 fat    11689 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+-rw-rw-rw-  2.0 fat     2893 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_102_appdata.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_103_reactors.py
+-rw-rw-rw-  2.0 fat     4001 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_104_extension_dict.py
+-rw-rw-rw-  2.0 fat    20860 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_105_xdata.py
+-rw-rw-rw-  2.0 fat    14169 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_110_dxfentity.py
+-rw-rw-rw-  2.0 fat     2433 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+-rw-rw-rw-  2.0 fat     6781 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+-rw-rw-rw-  2.0 fat      695 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_112b_dxfobj.py
+-rw-rw-rw-  2.0 fat     2431 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_113_dxfclass.py
+-rw-rw-rw-  2.0 fat     4044 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_114_factory.py
+-rw-rw-rw-  2.0 fat     2256 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+-rw-rw-rw-  2.0 fat    15794 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_116_dictionary.py
+-rw-rw-rw-  2.0 fat     4999 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+-rw-rw-rw-  2.0 fat     3003 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_120_style_table_entry.py
+-rw-rw-rw-  2.0 fat     2943 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+-rw-rw-rw-  2.0 fat      379 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+-rw-rw-rw-  2.0 fat     1113 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_123_view_table_entry.py
+-rw-rw-rw-  2.0 fat     8757 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_125_image_def.py
+-rw-rw-rw-  2.0 fat     1312 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+-rw-rw-rw-  2.0 fat     1430 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_127_raster_variables.py
+-rw-rw-rw-  2.0 fat     1540 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_128_pdf_definition.py
+-rw-rw-rw-  2.0 fat     2778 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_129_xrecord.py
+-rw-rw-rw-  2.0 fat     2423 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_130_id_buffer.py
+-rw-rw-rw-  2.0 fat     2470 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_131_field_list.py
+-rw-rw-rw-  2.0 fat     2435 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_132_layer_filter.py
+-rw-rw-rw-  2.0 fat     2153 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_133_sun.py
+-rw-rw-rw-  2.0 fat      852 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_134_material.py
+-rw-rw-rw-  2.0 fat    11497 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_135_geo_data.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_136_vba_project.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_137_sortentstable.py
+-rw-rw-rw-  2.0 fat      704 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+-rw-rw-rw-  2.0 fat     7570 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_139_user_record.py
+-rw-rw-rw-  2.0 fat      714 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_140_block_record.py
+-rw-rw-rw-  2.0 fat     9153 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/conftest.py
+-rw-rw-rw-  2.0 fat     6532 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_200_line.py
+-rw-rw-rw-  2.0 fat     4273 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_201_point.py
+-rw-rw-rw-  2.0 fat     6827 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_202_circle.py
+-rw-rw-rw-  2.0 fat     8949 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_203_arc.py
+-rw-rw-rw-  2.0 fat     2852 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_204_shape.py
+-rw-rw-rw-  2.0 fat     8242 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_205_solid.py
+-rw-rw-rw-  2.0 fat     8476 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_206_text.py
+-rw-rw-rw-  2.0 fat     4947 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_207_attdef.py
+-rw-rw-rw-  2.0 fat     6312 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_208_attrib.py
+-rw-rw-rw-  2.0 fat     2671 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_209_vertex.py
+-rw-rw-rw-  2.0 fat     5930 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_1.py
+-rw-rw-rw-  2.0 fat    13489 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_2.py
+-rw-rw-rw-  2.0 fat     6650 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+-rw-rw-rw-  2.0 fat     1780 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+-rw-rw-rw-  2.0 fat     7847 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_211_viewport.py
+-rw-rw-rw-  2.0 fat    12629 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_212_insert.py
+-rw-rw-rw-  2.0 fat     6024 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_213_minsert.py
+-rw-rw-rw-  2.0 fat     3284 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_214_block.py
+-rw-rw-rw-  2.0 fat     6882 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_215_dimension.py
+-rw-rw-rw-  2.0 fat     4907 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+-rw-rw-rw-  2.0 fat    13186 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+-rw-rw-rw-  2.0 fat     6471 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+-rw-rw-rw-  2.0 fat     5535 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+-rw-rw-rw-  2.0 fat     3056 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+-rw-rw-rw-  2.0 fat     7181 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+-rw-rw-rw-  2.0 fat     2066 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+-rw-rw-rw-  2.0 fat     3615 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+-rw-rw-rw-  2.0 fat     6919 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_221_ellipse.py
+-rw-rw-rw-  2.0 fat     2223 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_222_xline.py
+-rw-rw-rw-  2.0 fat     1493 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_223_ray.py
+-rw-rw-rw-  2.0 fat     2176 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_224_group.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_225_mtext.py
+-rw-rw-rw-  2.0 fat    12020 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_226_spline.py
+-rw-rw-rw-  2.0 fat     5529 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+-rw-rw-rw-  2.0 fat    10893 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+-rw-rw-rw-  2.0 fat    15116 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_228_mesh.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+-rw-rw-rw-  2.0 fat    21421 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+-rw-rw-rw-  2.0 fat     6587 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+-rw-rw-rw-  2.0 fat     3140 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+-rw-rw-rw-  2.0 fat    12486 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+-rw-rw-rw-  2.0 fat     2274 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_231_underlay.py
+-rw-rw-rw-  2.0 fat     5243 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_231_underlay_2.py
+-rw-rw-rw-  2.0 fat     2294 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_acis.py
+-rw-rw-rw-  2.0 fat     6799 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_acis_2.py
+-rw-rw-rw-  2.0 fat     1854 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_surface.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_233_helix.py
+-rw-rw-rw-  2.0 fat     2040 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_234_light.py
+-rw-rw-rw-  2.0 fat     3806 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_235_leader.py
+-rw-rw-rw-  2.0 fat    20392 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_236_multileader.py
+-rw-rw-rw-  2.0 fat    10992 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_237_mline.py
+-rw-rw-rw-  2.0 fat     2356 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_238_tolerance.py
+-rw-rw-rw-  2.0 fat    27392 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+-rw-rw-rw-  2.0 fat     4347 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_241_hyperlink.py
+-rw-rw-rw-  2.0 fat    11313 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_242_random_transform.py
+-rw-rw-rw-  2.0 fat     3725 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_243_replace_entity.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+-rw-rw-rw-  2.0 fat     4456 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_245_wipeout.py
+-rw-rw-rw-  2.0 fat     6175 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_246_spline_audit.py
+-rw-rw-rw-  2.0 fat     8165 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+-rw-rw-rw-  2.0 fat     6003 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_248_mpolygon.py
+-rw-rw-rw-  2.0 fat    13682 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+-rw-rw-rw-  2.0 fat     5713 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+-rw-rw-rw-  2.0 fat     8331 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+-rw-rw-rw-  2.0 fat     7331 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_251_upright.py
+-rw-rw-rw-  2.0 fat     4795 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat     2082 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_253_ole2frame.py
+-rw-rw-rw-  2.0 fat      821 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_254_get_font_name.py
+-rw-rw-rw-  2.0 fat     5149 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_300_layout.py
+-rw-rw-rw-  2.0 fat     4274 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+-rw-rw-rw-  2.0 fat     5582 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_302_block_references.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+-rw-rw-rw-  2.0 fat      913 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+-rw-rw-rw-  2.0 fat     3279 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+-rw-rw-rw-  2.0 fat     2609 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+-rw-rw-rw-  2.0 fat     2343 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_307_groupby.py
+-rw-rw-rw-  2.0 fat    17748 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_308_query.py
+-rw-rw-rw-  2.0 fat     6382 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_309_query_parser.py
+-rw-rw-rw-  2.0 fat     5031 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+-rw-rw-rw-  2.0 fat     5782 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+-rw-rw-rw-  2.0 fat      647 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_313_redraw_order.py
+-rw-rw-rw-  2.0 fat     6128 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+-rw-rw-rw-  2.0 fat     2750 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+-rw-rw-rw-  2.0 fat     5208 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+-rw-rw-rw-  2.0 fat     6795 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+-rw-rw-rw-  2.0 fat     4981 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+-rw-rw-rw-  2.0 fat     2450 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_405_classes.py
+-rw-rw-rw-  2.0 fat     9094 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+-rw-rw-rw-  2.0 fat      848 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+-rw-rw-rw-  2.0 fat     3375 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+-rw-rw-rw-  2.0 fat     1433 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+-rw-rw-rw-  2.0 fat     5736 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_410_table.py
+-rw-rw-rw-  2.0 fat     6607 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+-rw-rw-rw-  2.0 fat    18072 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+-rw-rw-rw-  2.0 fat     4638 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+-rw-rw-rw-  2.0 fat    12336 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+-rw-rw-rw-  2.0 fat     6509 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+-rw-rw-rw-  2.0 fat     5656 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+-rw-rw-rw-  2.0 fat     5434 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+-rw-rw-rw-  2.0 fat      733 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+-rw-rw-rw-  2.0 fat     1240 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+-rw-rw-rw-  2.0 fat     5007 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+-rw-rw-rw-  2.0 fat      769 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+-rw-rw-rw-  2.0 fat     7289 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_424_audit.py
+-rw-rw-rw-  2.0 fat     3737 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+-rw-rw-rw-  2.0 fat     2981 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+-rw-rw-rw-  2.0 fat     2416 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+-rw-rw-rw-  2.0 fat     2533 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+-rw-rw-rw-  2.0 fat   112800 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/conftest.py
+-rw-rw-rw-  2.0 fat     5510 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_500_units.py
+-rw-rw-rw-  2.0 fat     1052 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_501_truecolor.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_502_raw_color.py
+-rw-rw-rw-  2.0 fat     1695 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_503_indexing.py
+-rw-rw-rw-  2.0 fat     1442 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_504_suppress_zeros.py
+-rw-rw-rw-  2.0 fat      216 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_506_version.py
+-rw-rw-rw-  2.0 fat      579 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_507_dxf_pretty_printer.py
+-rw-rw-rw-  2.0 fat      657 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_508_read_zip.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_509_comments.py
+-rw-rw-rw-  2.0 fat     1185 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_510_byte_stream.py
+-rw-rw-rw-  2.0 fat     4239 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_511_bit_stream.py
+-rw-rw-rw-  2.0 fat     5595 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_512_pattern.py
+-rw-rw-rw-  2.0 fat     2372 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_513_reorder_entities.py
+-rw-rw-rw-  2.0 fat    17710 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_514_text.py
+-rw-rw-rw-  2.0 fat     5519 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_515_fonts.py
+-rw-rw-rw-  2.0 fat     4002 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_516_zoom.py
+-rw-rw-rw-  2.0 fat    34209 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_517_text_layout.py
+-rw-rw-rw-  2.0 fat      474 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_518_header_guid.py
+-rw-rw-rw-  2.0 fat     3716 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_519_mtext_editor.py
+-rw-rw-rw-  2.0 fat     3205 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_520_mtext_context.py
+-rw-rw-rw-  2.0 fat    24506 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_521_mtext_parser.py
+-rw-rw-rw-  2.0 fat     3863 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_522_text_scanner.py
+-rw-rw-rw-  2.0 fat     6202 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_523_text_size.py
+-rw-rw-rw-  2.0 fat     5063 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_524_block_reference_manager.py
+-rw-rw-rw-  2.0 fat      773 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_525_transparency.py
+-rw-rw-rw-  2.0 fat     2133 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_526_explode.py
+-rw-rw-rw-  2.0 fat    13521 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_527_gfxattribs.py
+-rw-rw-rw-  2.0 fat     2748 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_528_difftags.py
+-rw-rw-rw-  2.0 fat     6700 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_529_acis_sat.py
+-rw-rw-rw-  2.0 fat     2062 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_530_acis_sab.py
+-rw-rw-rw-  2.0 fat    12366 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_531_acis_entities.py
+-rw-rw-rw-  2.0 fat     7533 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_532_acis_mesh.py
+-rw-rw-rw-  2.0 fat    42518 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_533_shapefiles.py
+-rw-rw-rw-  2.0 fat     1034 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_534_dwg_info.py
+-rw-rw-rw-  2.0 fat    47915 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_535_xref_basic.py
+-rw-rw-rw-  2.0 fat    27614 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_536_xref_conflict.py
+-rw-rw-rw-  2.0 fat     6887 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_537_transform.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/conftest.py
+-rw-rw-rw-  2.0 fat     7460 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_600_base.py
+-rw-rw-rw-  2.0 fat     2098 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_601_bulge.py
+-rw-rw-rw-  2.0 fat    14651 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_602_vec3.py
+-rw-rw-rw-  2.0 fat     8956 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_603_vec2.py
+-rw-rw-rw-  2.0 fat     2801 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_604_banded_matrix.py
+-rw-rw-rw-  2.0 fat     9738 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_604_linalg.py
+-rw-rw-rw-  2.0 fat    11458 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_605_matrix44.py
+-rw-rw-rw-  2.0 fat     5888 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_606_convexhull.py
+-rw-rw-rw-  2.0 fat     1010 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_607_perlin_noise.py
+-rw-rw-rw-  2.0 fat     3833 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_608_intersection_line_line_2d.py
+-rw-rw-rw-  2.0 fat     1676 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_609_point_on_line.py
+-rw-rw-rw-  2.0 fat     3171 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_610_ocs.py
+-rw-rw-rw-  2.0 fat     7529 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_611_ucs.py
+-rw-rw-rw-  2.0 fat     1831 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_612_ucs_pass_trough.py
+-rw-rw-rw-  2.0 fat     2586 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_613_point_in_poygon.py
+-rw-rw-rw-  2.0 fat    10913 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_614_construct_3d.py
+-rw-rw-rw-  2.0 fat      602 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_615_rytz_axis.py
+-rw-rw-rw-  2.0 fat     5215 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_616_plane.py
+-rw-rw-rw-  2.0 fat      772 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_617_clockwise_orientation.py
+-rw-rw-rw-  2.0 fat     6384 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_618_clipping.py
+-rw-rw-rw-  2.0 fat    10108 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_619_greiner_hormann.py
+-rw-rw-rw-  2.0 fat     2669 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_620_knot.py
+-rw-rw-rw-  2.0 fat    19780 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_621_bspline.py
+-rw-rw-rw-  2.0 fat     7652 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_622_bsplineu.py
+-rw-rw-rw-  2.0 fat    12197 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_623_rbspline.py
+-rw-rw-rw-  2.0 fat    10809 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_624_global_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1247 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_626_local_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1967 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_627_bspline_basis.py
+-rw-rw-rw-  2.0 fat    10545 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_629_bezier.py
+-rw-rw-rw-  2.0 fat    10714 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_630a_bezier4p_base.py
+-rw-rw-rw-  2.0 fat    10204 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_630b_bezier4p_functions.py
+-rw-rw-rw-  2.0 fat     1683 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_631_euler_spiral.py
+-rw-rw-rw-  2.0 fat     4021 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_632_bezier3p.py
+-rw-rw-rw-  2.0 fat    19463 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_640_bbox.py
+-rw-rw-rw-  2.0 fat     5393 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_641_construction_ray.py
+-rw-rw-rw-  2.0 fat     3673 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_642_construction_line.py
+-rw-rw-rw-  2.0 fat     9459 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_643_construction_box.py
+-rw-rw-rw-  2.0 fat    10941 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_644_construction_circle.py
+-rw-rw-rw-  2.0 fat    10988 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_645_construction_arc.py
+-rw-rw-rw-  2.0 fat     3422 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_646_offset_vertices_2d.py
+-rw-rw-rw-  2.0 fat     7672 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_647_transform_tools.py
+-rw-rw-rw-  2.0 fat     8993 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_648_construction_ellipse.py
+-rw-rw-rw-  2.0 fat     1991 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_649_nurbs_python_interface.py
+-rw-rw-rw-  2.0 fat     4243 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_650_elliptic_arc_span.py
+-rw-rw-rw-  2.0 fat     9011 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_651_construction_polyline.py
+-rw-rw-rw-  2.0 fat     3168 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_652_approx_param_t.py
+-rw-rw-rw-  2.0 fat     5806 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_653_polyline_intersection.py
+-rw-rw-rw-  2.0 fat     5193 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_654_rtree.py
+-rw-rw-rw-  2.0 fat      788 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_655_dbscan.py
+-rw-rw-rw-  2.0 fat      834 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_656_k_means.py
+-rw-rw-rw-  2.0 fat     4654 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_657_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    11628 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_658_bevel_tools.py
+-rw-rw-rw-  2.0 fat     1875 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1428 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1741 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+-rw-rw-rw-  2.0 fat     3307 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_662_is_convex_polygon_2d.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_701_arrows.py
+-rw-rw-rw-  2.0 fat    17245 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_702_render_forms.py
+-rw-rw-rw-  2.0 fat    34220 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_703_mesh_builder.py
+-rw-rw-rw-  2.0 fat     3852 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_704_render_linear_dimension.py
+-rw-rw-rw-  2.0 fat     1345 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_705_shape.py
+-rw-rw-rw-  2.0 fat      483 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_706_random_path.py
+-rw-rw-rw-  2.0 fat     5603 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_707_trace.py
+-rw-rw-rw-  2.0 fat    33834 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_708a_path.py
+-rw-rw-rw-  2.0 fat    27351 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_708b_path_tools.py
+-rw-rw-rw-  2.0 fat     3633 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_708c_matplotlib_path_tools.py
+-rw-rw-rw-  2.0 fat     4725 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_708d_qpainter_path_tools.py
+-rw-rw-rw-  2.0 fat     4589 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_708e_path_shapes.py
+-rw-rw-rw-  2.0 fat     4118 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_708f_path_nesting.py
+-rw-rw-rw-  2.0 fat     1308 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_709_linetype_renderer.py
+-rw-rw-rw-  2.0 fat     2815 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_711_points.py
+-rw-rw-rw-  2.0 fat     6594 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_712_render_curved_dimension.py
+-rw-rw-rw-  2.0 fat     1472 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_713_mleader_builder.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_714_mleader_render_engine.py
+-rw-rw-rw-  2.0 fat    11778 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_715_hatching.py
+-rw-rw-rw-  2.0 fat     2626 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+-rw-rw-rw-  2.0 fat     4771 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_800_mtext_surrogate.py
+-rw-rw-rw-  2.0 fat     1352 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_801_r12spline.py
+-rw-rw-rw-  2.0 fat     7881 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_802_table_painter.py
+-rw-rw-rw-  2.0 fat    12386 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_803_entities_to_code.py
+-rw-rw-rw-  2.0 fat     6844 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_804_importer.py
+-rw-rw-rw-  2.0 fat     2362 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_805_pycsg.py
+-rw-rw-rw-  2.0 fat    15467 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_806_acadctb.py
+-rw-rw-rw-  2.0 fat     4860 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_807_dwg_loader_basics.py
+-rw-rw-rw-  2.0 fat    10862 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_810_drawing_properties.py
+-rw-rw-rw-  2.0 fat    14074 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_811_drawing_frontend.py
+-rw-rw-rw-  2.0 fat     4157 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+-rw-rw-rw-  2.0 fat    12547 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_813_geo_interface.py
+-rw-rw-rw-  2.0 fat    16289 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_814_text2path.py
+-rw-rw-rw-  2.0 fat    16239 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_815_dxf_browser.py
+-rw-rw-rw-  2.0 fat    11275 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_816_bin_packing.py
+-rw-rw-rw-  2.0 fat    12554 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_817_genetic_algorithm.py
+-rw-rw-rw-  2.0 fat     9008 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_818_meshex.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_819_menger_sponge.py
+-rw-rw-rw-  2.0 fat     4433 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_820_openscad.py
+-rw-rw-rw-  2.0 fat    15352 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_821_hpgl2.py
+-rw-rw-rw-  2.0 fat     1322 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+-rw-rw-rw-  2.0 fat     2527 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+-rw-rw-rw-  2.0 fat     2199 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+-rw-rw-rw-  2.0 fat     1732 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+-rw-rw-rw-  2.0 fat     3158 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+-rw-rw-rw-  2.0 fat     1452 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+-rw-rw-rw-  2.0 fat     4755 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+-rw-rw-rw-  2.0 fat     2656 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_10_issues/test_issue_414_bbox_calculation.py
+-rw-rw-rw-  2.0 fat     1213 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_10_issues/test_issue_574_flattening_error.py
+-rw-rw-rw-  2.0 fat     1754 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+-rw-rw-rw-  2.0 fat      682 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_10_issues/test_issue_749_text_layout.py
+819 files, 8621198 bytes uncompressed, 1922889 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -1,2395 +1,2458 @@
-Filename: ezdxf-1.0.3b0/
+Filename: ezdxf-1.0.4b1/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/
+Filename: ezdxf-1.0.4b1/integration_tests/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/
+Filename: ezdxf-1.0.4b1/src/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/
+Filename: ezdxf-1.0.4b1/tests/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/LICENSE
+Filename: ezdxf-1.0.4b1/LICENSE
 Comment: 
 
-Filename: ezdxf-1.0.3b0/MANIFEST.in
+Filename: ezdxf-1.0.4b1/MANIFEST.in
 Comment: 
 
-Filename: ezdxf-1.0.3b0/NEWS.md
+Filename: ezdxf-1.0.4b1/NEWS.md
 Comment: 
 
-Filename: ezdxf-1.0.3b0/PKG-INFO
+Filename: ezdxf-1.0.4b1/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.0.3b0/README.md
+Filename: ezdxf-1.0.4b1/README.md
 Comment: 
 
-Filename: ezdxf-1.0.3b0/requirements.txt
+Filename: ezdxf-1.0.4b1/requirements.txt
 Comment: 
 
-Filename: ezdxf-1.0.3b0/setup.cfg
+Filename: ezdxf-1.0.4b1/setup.cfg
 Comment: 
 
-Filename: ezdxf-1.0.3b0/setup.py
+Filename: ezdxf-1.0.4b1/setup.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/
+Filename: ezdxf-1.0.4b1/integration_tests/data/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/check_disable_c_ext_by_config_file.py
+Filename: ezdxf-1.0.4b1/integration_tests/check_disable_c_ext_by_config_file.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/check_disable_c_ext_by_env_var.py
+Filename: ezdxf-1.0.4b1/integration_tests/check_disable_c_ext_by_env_var.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_acad_table.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_acad_table.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_all_dimline_styles.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_all_dimline_styles.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_all_ellipse_transformations.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_all_ellipse_transformations.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_anonymous_blocks.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_anonymous_blocks.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_audit_critical_dxf_files.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_audit_critical_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_audit_layouts.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_audit_layouts.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_complex_line_type_2.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_complex_line_type_2.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_create_basic_graphics.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_create_basic_graphics.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_document_guid.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_document_guid.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_document_page_setup.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_document_page_setup.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_drawing_matplotlib_backend.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_drawing_matplotlib_backend.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_drawing_qt_backend.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_drawing_qt_backend.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_dxf_info_scanning.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_dxf_info_scanning.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_entities_iterator.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_entities_iterator.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_fix_dulicate_handles.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_fix_dulicate_handles.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_geo.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_geo.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_groups.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_groups.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_ignore_junk_beyond_EOF.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_ignore_junk_beyond_EOF.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_launcher.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_launcher.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_leica_disto_r12.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_leica_disto_r12.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_load_dxf_unicode_notation.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_load_dxf_unicode_notation.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_mapbox_earcut.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_matplotlib_font_support.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_matplotlib_font_support.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_mtext_columns.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_mtext_explode_addon.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_mtext_explode_addon.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_mtext_text_frame.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_mtext_text_frame.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_new_table_entries.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_new_table_entries.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_none_ascii_read_write.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_none_ascii_read_write.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_odafc.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_odafc.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_open_binary_DXF_files.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_open_binary_DXF_files.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_open_coord_order_issue.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_open_coord_order_issue.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_open_exotic_dxf_files.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_open_exotic_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_open_R13_R14.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_open_R13_R14.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_polyline_entity.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_polyline_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_preserve_binary_data_in_xrecords.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_preserve_binary_data_in_xrecords.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_r12export.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_r12export.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_r12strict.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_r12strict.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_r12writer.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_r12writer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_read_file_without_handles.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_read_file_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_read_write_modern_entites.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_read_write_modern_entites.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_recover.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_recover.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_redraw_order.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_rotated_block_attributes.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_rotated_block_attributes.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_surface_entities.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_surface_entities.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_write_fixed_meta_data.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_write_fixed_meta_data.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/test_write_without_handles.py
+Filename: ezdxf-1.0.4b1/integration_tests/test_write_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/AC1003_LINE_Example.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/test_xref_detach.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/acad_table_with_blk_ref.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/AC1003_LINE_Example.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/ASCII_R12.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/acad_table_with_blk_ref.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/bin_dxf_r12.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/ASCII_R12.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/bin_dxf_r13.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r12.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/bin_dxf_r14.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/bin_dxf_r2000.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/cc_dxflib.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r2000.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/custom_blocks.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/cc_dxflib.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/duplicate_handles.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/custom_blocks.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/dxf_unicode.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/duplicate_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/empty_handles.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/dxf_unicode.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/groups.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/empty_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/Leica_Disto_S910.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/groups.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/MODEL.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/Leica_Disto_S910.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/mtext_columns_R2007.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/MODEL.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/mtext_columns_R2018.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/mtext_columns_R2007.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/mtext_framed_columns.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/mtext_columns_R2018.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/mtext_text_frame.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/mtext_framed_columns.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/no_layouts.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/mtext_text_frame.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/POLI-ALL210_12.DXF
+Filename: ezdxf-1.0.4b1/integration_tests/data/no_layouts.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/POLI-ALL210_12.DXF
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/recover01.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/R12_with_trash_beyond_EOF.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/recover02.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/recover01.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/small_r13.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/recover02.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/small_r14.dxf
+Filename: ezdxf-1.0.4b1/integration_tests/data/small_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/XRECORD_0.bin
+Filename: ezdxf-1.0.4b1/integration_tests/data/small_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/XRECORD_1.bin
+Filename: ezdxf-1.0.4b1/integration_tests/data/XRECORD_0.bin
 Comment: 
 
-Filename: ezdxf-1.0.3b0/integration_tests/data/XRECORD_2.bin
+Filename: ezdxf-1.0.4b1/integration_tests/data/XRECORD_1.bin
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/
+Filename: ezdxf-1.0.4b1/integration_tests/data/XRECORD_2.bin
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf.egg-info/
+Filename: ezdxf-1.0.4b1/src/ezdxf/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/
+Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acis/
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/
+Filename: ezdxf-1.0.4b1/src/ezdxf/acis/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/layouts/
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/
+Filename: ezdxf-1.0.4b1/src/ezdxf/layouts/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/path/
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/pp/
+Filename: ezdxf-1.0.4b1/src/ezdxf/path/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/
+Filename: ezdxf-1.0.4b1/src/ezdxf/pp/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/sections/
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/
+Filename: ezdxf-1.0.4b1/src/ezdxf/sections/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/appsettings.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/audit.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/appsettings.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/bbox.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/audit.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/blkrefs.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/bbox.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/colors.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/blkrefs.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/commands.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/colors.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/comments.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/commands.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/disassemble.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/comments.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/document.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/disassemble.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/dwginfo.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/document.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entitydb.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/dwginfo.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/enums.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entitydb.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/explode.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/enums.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/eztypes.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/explode.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/filemanagement.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/eztypes.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/gfxattribs.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/filemanagement.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/graphicsfactory.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/groupby.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/graphicsfactory.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/protocols.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/groupby.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/proxygraphic.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/protocols.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/py.typed
+Filename: ezdxf-1.0.4b1/src/ezdxf/proxygraphic.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/query.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/py.typed
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/queryparser.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/query.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/r12strict.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/queryparser.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/recover.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/r12strict.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/reorder.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/recover.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/shapefile.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/reorder.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/units.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/shapefile.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/upright.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/transform.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/urecord.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/units.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/version.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/upright.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/xref.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/urecord.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/zoom.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/version.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/_options.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/xref.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/zoom.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/__main__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/_options.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/bezier3p.pyx
+Filename: ezdxf-1.0.4b1/src/ezdxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/bezier4p.pyx
+Filename: ezdxf-1.0.4b1/src/ezdxf/__main__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/bspline.pyx
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/bezier3p.pyx
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/construct.pxd
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/bezier4p.pyx
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/construct.pyx
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/bspline.pyx
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/linetypes.pyx
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/construct.pxd
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/mapbox_earcut.pyx
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/construct.pyx
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/matrix44.pxd
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/linetypes.pyx
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/matrix44.pyx
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/mapbox_earcut.pyx
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/vector.pxd
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/matrix44.pxd
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/vector.pyx
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/matrix44.pyx
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/vector.pxd
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/vector.pyx
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_quad_bezier.cpp
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_quad_bezier.hpp
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_quad_bezier.pxd
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_vec3.hpp
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_vec3.pxd
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acc/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_vec3.hpp
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acis/abstract.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_vec3.pxd
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acis/api.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/acc/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acis/const.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/acis/abstract.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acis/dbg.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/acis/api.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acis/dxf.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/acis/const.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acis/entities.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/acis/dbg.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acis/hdr.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/acis/dxf.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acis/mesh.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/acis/entities.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acis/sab.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/acis/hdr.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acis/sat.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/acis/mesh.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/acis/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/acis/sab.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/acisbrowser/
+Filename: ezdxf-1.0.4b1/src/ezdxf/acis/sat.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/browser/
+Filename: ezdxf-1.0.4b1/src/ezdxf/acis/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/dwg/
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/acadctb.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/binpacking.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/dimlines.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/dxf2code.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/acadctb.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/genetic_algorithm.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/binpacking.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/geo.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dimlines.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/gerber_D6673.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dxf2code.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/importer.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/iterdxf.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/geo.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/menger_sponge.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/gerber_D6673.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/meshex.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/importer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/mixins.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/iterdxf.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/mtextsurrogate.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/mtxpl.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/meshex.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/odafc.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/mixins.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/openscad.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/mtextsurrogate.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/pycsg.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/mtxpl.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/r12export.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/odafc.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/r12writer.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/openscad.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/sierpinski_pyramid.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/pycsg.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/tablepainter.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/r12export.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/text2path.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/r12writer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/xqt.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/sierpinski_pyramid.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/tablepainter.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/acisbrowser/browser.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/text2path.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/acisbrowser/data.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/xqt.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/acisbrowser/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/browser/bookmarks.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/browser.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/browser/browser.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/data.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/browser/data.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/browser/find_dialog.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/bookmarks.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/browser/loader.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/browser.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/browser/model.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/data.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/browser/tags.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/find_dialog.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/browser/views.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/loader.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/browser/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/model.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/backend.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/tags.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/config.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/views.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/debug_backend.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/debug_utils.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/backend.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/frontend.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/config.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/gfxproxy.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/debug_backend.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/matplotlib.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/debug_utils.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/mpl_text_renderer.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/frontend.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/mtext_complex.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/gfxproxy.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/pillow.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/matplotlib.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/properties.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/mpl_text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/pyqt.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/mtext_complex.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/qtviewer.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/pillow.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/qt_text_renderer.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/properties.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/text.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/pyqt.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/text_renderer.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/qtviewer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/type_hints.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/qt_text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/drawing/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/text.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/dwg/classes_section.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/dwg/const.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/type_hints.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/dwg/crc.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/dwg/fileheader.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/classes_section.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/dwg/header_section.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/const.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/dwg/loader.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/crc.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/addons/dwg/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/fileheader.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/acad_proxy_entity.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/header_section.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/acad_table.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/loader.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/acis.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/appdata.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/api.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/appid.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/backend.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/arc.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/compiler.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/attrib.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/deps.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/block.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/dxf_backend.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/blockrecord.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/interpreter.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/boundary_paths.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/page.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/circle.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/pdf_backend.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/dictionary.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/plotter.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/dimension.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/polygon_buffer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/dimstyle.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/properties.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/dimstyleoverride.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/svg_backend.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/dxfclass.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/tokenizer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/dxfentity.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/dxfgfx.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/dxfgroups.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/acad_table.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/dxfns.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/acis.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/dxfobj.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/appdata.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/ellipse.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/appid.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/factory.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/arc.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/geodata.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/attrib.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/gradient.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/block.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/hatch.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/blockrecord.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/helix.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/idbuffer.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/circle.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/image.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dictionary.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/insert.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/layer.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dimstyle.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/layout.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dimstyleoverride.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/leader.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/light.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/line.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/ltype.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/lwpolyline.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dxfns.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/material.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/mesh.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/mleader.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/factory.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/mline.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/geodata.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/mpolygon.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/gradient.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/mtext.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/hatch.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/mtext_columns.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/helix.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/objectcollection.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/idbuffer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/oleframe.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/image.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/pattern.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/insert.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/point.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/layer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/polygon.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/layout.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/polyline.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/leader.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/shape.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/light.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/solid.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/line.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/spline.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/ltype.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/subentity.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/lwpolyline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/sun.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/material.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/table.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/mesh.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/text.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/mleader.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/textstyle.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/mline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/tolerance.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/ucs.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/mtext.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/underlay.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/view.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/objectcollection.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/viewport.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/oleframe.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/visualstyle.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/pattern.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/vport.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/point.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/xdata.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/polygon.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/xdict.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/polyline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/xline.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/shape.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/entities/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/solid.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/layouts/base.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/spline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/layouts/blocklayout.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/subentity.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/layouts/layout.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/sun.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/layouts/layouts.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/table.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/layouts/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/text.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/attributes.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/textstyle.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/const.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/tolerance.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/encoding.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/ucs.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/extendedtags.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/underlay.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/fileindex.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/view.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/hdrvars.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/viewport.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/loader.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/visualstyle.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/packedtags.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/vport.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/repair.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/xdata.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/tagger.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/xdict.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/tags.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/xline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/tagwriter.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/entities/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/types.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/layouts/base.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/validator.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/layouts/blocklayout.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/lldxf/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/layouts/layout.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/arc.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/layouts/layouts.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/bbox.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/layouts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/bezier.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/attributes.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/bezier_interpolation.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/const.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/box.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/encoding.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/bspline.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/extendedtags.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/bulge.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/fileindex.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/circle.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/hdrvars.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/clipping.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/loader.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/clustering.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/packedtags.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/construct2d.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/repair.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/construct3d.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/tagger.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/cspline.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/tags.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/curvetools.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/tagwriter.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/ellipse.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/types.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/eulerspiral.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/validator.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/linalg.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/line.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/arc.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/offset2d.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/bbox.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/parametrize.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/bezier.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/perlin.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/bezier_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/polyline.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/box.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/rtree.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/bspline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/shape.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/bulge.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/surfaces.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/circle.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/transformtools.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/clipping.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/triangulation.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/clustering.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/ucs.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/construct2d.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/_bezier3p.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/construct3d.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/_bezier4p.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/cspline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/_bspline.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/curvetools.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/_construct.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/_ctypes.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/eulerspiral.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/_mapbox_earcut.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/linalg.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/_matrix44.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/line.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/_vector.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/offset2d.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/math/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/parametrize.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/path/commands.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/perlin.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/path/converter.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/polyline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/path/nesting.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/rtree.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/path/path.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/shape.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/path/shapes.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/surfaces.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/path/tools.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/transformtools.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/path/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/triangulation.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/pp/dxfpp.css
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/ucs.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/pp/dxfpp.html
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/pp/dxfpp.js
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/pp/dxfpp.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/_bspline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/pp/pprint.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/_construct.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/pp/rawpp.css
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/_ctypes.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/pp/rawpp.html
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/pp/rawpp.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/pp/reflinks.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/_vector.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/pp/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/math/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/abstract_mtext_renderer.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/path/commands.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/arrows.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/path/converter.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/curves.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/path/nesting.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/dimension.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/path/path.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/dim_base.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/path/shapes.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/dim_curved.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/path/tools.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/dim_diameter.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/path/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/dim_linear.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.css
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/dim_ordinate.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.html
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/dim_radius.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.js
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/forms.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/hatching.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/pp/pprint.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/leader.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.css
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/linetypes.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.html
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/mesh.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/mleader.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/pp/reflinks.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/mline.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/pp/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/point.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/abstract_mtext_renderer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/polyline.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/arrows.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/r12spline.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/curves.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/trace.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/_linetypes.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/dim_base.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/render/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/dim_curved.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/16x16.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/dim_diameter.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/24x24.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/dim_linear.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/256x256.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/dim_ordinate.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/32x32.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/dim_radius.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/48x48.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/forms.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/64x64.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/hatching.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/icon-copy-64px.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/leader.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/icon-find-64px.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/linetypes.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/icon-goto-bookmark-64px.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/mesh.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/icon-goto-handle-64px.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/mleader.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/icon-goto-line-64px.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/mline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/icon-left-arrow-64px.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/point.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/icon-next-entity-64px.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/polyline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/icon-prev-entity-64px.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/r12spline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/icon-right-arrow-64px.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/trace.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/icon-show-in-tree-64px.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/_linetypes.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/resources/icon-store-bookmark-64px.png
+Filename: ezdxf-1.0.4b1/src/ezdxf/render/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/sections/acdsdata.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/16x16.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/sections/blocks.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/24x24.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/sections/classes.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/256x256.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/sections/entities.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/32x32.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/sections/header.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/48x48.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/sections/headervars.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/64x64.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/sections/objects.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-copy-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/sections/table.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-find-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/sections/tables.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/sections/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-handle-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/analyze.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-line-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/binarydata.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-left-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/codepage.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-next-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/complex_ltype.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-prev-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/crypt.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-right-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/debug.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-show-in-tree-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/difftags.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-store-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/fonts.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/sections/acdsdata.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/font_face_cache.json
+Filename: ezdxf-1.0.4b1/src/ezdxf/sections/blocks.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/font_measurement_cache.json
+Filename: ezdxf-1.0.4b1/src/ezdxf/sections/classes.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/handle.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/sections/entities.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/indexing.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/sections/header.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/juliandate.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/sections/headervars.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/pattern.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/sections/objects.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/rawloader.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/sections/table.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/standards.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/sections/tables.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/strip.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/sections/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/test.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/analyze.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/text.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/binarydata.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/text_layout.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/codepage.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/text_size.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/complex_ltype.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/zipmanager.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/crypt.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/_iso_pattern.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/debug.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/_matplotlib_font_support.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/difftags.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf/tools/__init__.py
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/fonts.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf.egg-info/dependency_links.txt
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/font_face_cache.json
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf.egg-info/entry_points.txt
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/font_measurement_cache.json
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf.egg-info/not-zip-safe
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/handle.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf.egg-info/PKG-INFO
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/indexing.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf.egg-info/requires.txt
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/juliandate.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf.egg-info/SOURCES.txt
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/pattern.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/src/ezdxf.egg-info/top_level.txt
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/rawloader.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/standards.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/strip.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/test.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/text.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/text_layout.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/text_size.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/zipmanager.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/_iso_pattern.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/_matplotlib_font_support.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_09_cython_acceleration/
+Filename: ezdxf-1.0.4b1/src/ezdxf/tools/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_10_issues/
+Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/entry_points.txt
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/not-zip-safe
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/requires.txt
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/top_level.txt
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_018_handle.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+Filename: ezdxf-1.0.4b1/tests/test_10_issues/
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_040_tags.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_011_codepage.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_018_handle.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_102_appdata.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_103_reactors.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_104_extension_dict.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_105_xdata.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_110_dxfentity.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_040_tags.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_112b_dxfobj.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_113_dxfclass.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_114_factory.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_116_dictionary.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_120_style_table_entry.py
+Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_102_appdata.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_123_view_table_entry.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_103_reactors.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_104_extension_dict.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_125_image_def.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_105_xdata.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_110_dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_127_raster_variables.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_128_pdf_definition.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_129_xrecord.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_112b_dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_130_id_buffer.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_113_dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_131_field_list.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_114_factory.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_132_layer_filter.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_133_sun.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_116_dictionary.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_134_material.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_135_geo_data.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_118_appid_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_136_vba_project.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_137_sortentstable.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_120_style_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_139_user_record.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_122_vport_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_140_block_record.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_123_view_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/conftest.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_125_image_def.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_200_line.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_201_point.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_127_raster_variables.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_202_circle.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_128_pdf_definition.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_203_arc.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_129_xrecord.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_204_shape.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_130_id_buffer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_205_solid.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_131_field_list.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_206_text.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_132_layer_filter.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_207_attdef.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_133_sun.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_208_attrib.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_134_material.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_209_vertex.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_135_geo_data.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_210_polyline_1.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_136_vba_project.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_210_polyline_2.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_137_sortentstable.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_139_user_record.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_211_viewport.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_140_block_record.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_212_insert.py
+Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_213_minsert.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/conftest.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_214_block.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_200_line.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_215_dimension.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_201_point.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_202_circle.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_203_arc.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_204_shape.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_205_solid.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_206_text.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_207_attdef.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_208_attrib.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_209_vertex.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_221_ellipse.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_1.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_222_xline.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_2.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_223_ray.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_224_group.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_225_mtext.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_211_viewport.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_226_spline.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_212_insert.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_213_minsert.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_214_block.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_228_mesh.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_215_dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_231_underlay.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_231_underlay_2.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_232_acis.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_232_acis_2.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_221_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_232_surface.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_222_xline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_233_helix.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_223_ray.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_234_light.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_224_group.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_235_leader.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_225_mtext.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_236_multileader.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_226_spline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_237_mline.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_238_tolerance.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_228_mesh.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_241_hyperlink.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_242_random_transform.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_243_replace_entity.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_245_wipeout.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_231_underlay.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_246_spline_audit.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_231_underlay_2.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_acis.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_248_mpolygon.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_acis_2.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_surface.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_233_helix.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_234_light.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_251_upright.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_235_leader.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_236_multileader.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_253_ole2frame.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_237_mline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_254_get_font_name.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_238_tolerance.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_300_layout.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_302_block_references.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_241_hyperlink.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_242_random_transform.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_243_replace_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_245_wipeout.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_307_groupby.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_246_spline_audit.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_308_query.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_309_query_parser.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_248_mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_313_redraw_order.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_251_upright.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_253_ole2frame.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_254_get_font_name.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_300_layout.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_405_classes.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_302_block_references.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_410_table.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_307_groupby.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_308_query.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_309_query_parser.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_313_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_405_classes.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_424_audit.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_410_table.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/conftest.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_500_units.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_501_truecolor.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_502_raw_color.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_503_indexing.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_504_suppress_zeros.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_506_version.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_507_dxf_pretty_printer.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_508_read_zip.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_509_comments.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_510_byte_stream.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_511_bit_stream.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_512_pattern.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_424_audit.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_513_reorder_entities.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_514_text.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_515_fonts.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_516_zoom.py
+Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_517_text_layout.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/conftest.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_518_header_guid.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_500_units.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_519_mtext_editor.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_501_truecolor.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_520_mtext_context.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_502_raw_color.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_521_mtext_parser.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_503_indexing.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_522_text_scanner.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_504_suppress_zeros.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_523_text_size.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_506_version.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_524_block_reference_manager.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_507_dxf_pretty_printer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_525_transparency.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_508_read_zip.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_526_explode.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_509_comments.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_527_gfxattribs.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_510_byte_stream.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_528_difftags.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_511_bit_stream.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_529_acis_sat.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_512_pattern.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_530_acis_sab.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_513_reorder_entities.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_531_acis_entities.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_514_text.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_532_acis_mesh.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_515_fonts.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_533_shapefiles.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_516_zoom.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_534_dwg_info.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_517_text_layout.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_535_xref_basic.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_518_header_guid.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_05_tools/test_536_xref_conflict.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_519_mtext_editor.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/conftest.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_520_mtext_context.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_600_base.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_521_mtext_parser.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_601_bulge.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_522_text_scanner.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_602_vec3.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_523_text_size.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_603_vec2.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_524_block_reference_manager.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_604_banded_matrix.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_525_transparency.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_604_linalg.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_526_explode.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_605_matrix44.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_527_gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_606_convexhull.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_528_difftags.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_607_perlin_noise.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_529_acis_sat.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_608_intersection_line_line_2d.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_530_acis_sab.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_609_point_on_line.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_531_acis_entities.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_610_ocs.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_532_acis_mesh.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_611_ucs.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_533_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_612_ucs_pass_trough.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_534_dwg_info.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_613_point_in_poygon.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_535_xref_basic.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_614_construct_3d.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_536_xref_conflict.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_615_rytz_axis.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_537_transform.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_616_plane.py
+Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_617_clockwise_orientation.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/conftest.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_618_clipping.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_600_base.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_619_greiner_hormann.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_601_bulge.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_620_knot.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_602_vec3.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_621_bspline.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_603_vec2.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_622_bsplineu.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_604_banded_matrix.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_623_rbspline.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_604_linalg.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_624_global_bspline_interpolation.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_605_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_626_local_bspline_interpolation.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_606_convexhull.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_627_bspline_basis.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_607_perlin_noise.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_629_bezier.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_608_intersection_line_line_2d.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_630a_bezier4p_base.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_609_point_on_line.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_630b_bezier4p_functions.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_610_ocs.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_631_euler_spiral.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_611_ucs.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_632_bezier3p.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_612_ucs_pass_trough.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_640_bbox.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_613_point_in_poygon.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_641_construction_ray.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_614_construct_3d.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_642_construction_line.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_615_rytz_axis.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_643_construction_box.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_616_plane.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_644_construction_circle.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_617_clockwise_orientation.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_645_construction_arc.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_618_clipping.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_646_offset_vertices_2d.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_619_greiner_hormann.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_647_transform_tools.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_620_knot.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_648_construction_ellipse.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_621_bspline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_649_nurbs_python_interface.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_622_bsplineu.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_650_elliptic_arc_span.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_623_rbspline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_651_construction_polyline.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_624_global_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_652_approx_param_t.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_626_local_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_653_polyline_intersection.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_627_bspline_basis.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_654_rtree.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_629_bezier.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_655_dbscan.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_630a_bezier4p_base.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_656_k_means.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_630b_bezier4p_functions.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_657_mapbox_earcut.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_631_euler_spiral.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_658_bevel_tools.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_632_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_640_bbox.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_641_construction_ray.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_642_construction_line.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_06_math/test_662_is_convex_polygon_2d.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_643_construction_box.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_701_arrows.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_644_construction_circle.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_702_render_forms.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_645_construction_arc.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_703_mesh_builder.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_646_offset_vertices_2d.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_704_render_linear_dimension.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_647_transform_tools.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_705_shape.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_648_construction_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_706_random_path.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_649_nurbs_python_interface.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_707_trace.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_650_elliptic_arc_span.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_708a_path.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_651_construction_polyline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_708b_path_tools.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_652_approx_param_t.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_708c_matplotlib_path_tools.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_653_polyline_intersection.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_708d_qpainter_path_tools.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_654_rtree.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_708e_path_shapes.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_655_dbscan.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_708f_path_nesting.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_656_k_means.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_709_linetype_renderer.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_657_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_711_points.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_658_bevel_tools.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_712_render_curved_dimension.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_713_mleader_builder.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_714_mleader_render_engine.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_715_hatching.py
+Filename: ezdxf-1.0.4b1/tests/test_06_math/test_662_is_convex_polygon_2d.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_701_arrows.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_800_mtext_surrogate.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_702_render_forms.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_801_r12spline.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_703_mesh_builder.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_802_table_painter.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_704_render_linear_dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_803_entities_to_code.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_705_shape.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_804_importer.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_706_random_path.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_805_pycsg.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_707_trace.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_806_acadctb.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_708a_path.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_807_dwg_loader_basics.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_708b_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_810_drawing_properties.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_708c_matplotlib_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_811_drawing_frontend.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_708d_qpainter_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_708e_path_shapes.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_813_geo_interface.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_708f_path_nesting.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_814_text2path.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_709_linetype_renderer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_815_dxf_browser.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_711_points.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_816_bin_packing.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_712_render_curved_dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_817_genetic_algorithm.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_713_mleader_builder.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_818_meshex.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_714_mleader_render_engine.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_819_menger_sponge.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_715_hatching.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_08_addons/test_820_openscad.py
+Filename: ezdxf-1.0.4b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_800_mtext_surrogate.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_801_r12spline.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_802_table_painter.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_803_entities_to_code.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_804_importer.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_805_pycsg.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_806_acadctb.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_807_dwg_loader_basics.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_10_issues/test_issue_574_flattening_error.py
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_810_drawing_properties.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_811_drawing_frontend.py
 Comment: 
 
-Filename: ezdxf-1.0.3b0/tests/test_10_issues/test_issue_749_text_layout.py
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_813_geo_interface.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_814_text2path.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_815_dxf_browser.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_816_bin_packing.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_817_genetic_algorithm.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_818_meshex.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_819_menger_sponge.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_820_openscad.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_821_hpgl2.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_10_issues/test_issue_574_flattening_error.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Comment: 
+
+Filename: ezdxf-1.0.4b1/tests/test_10_issues/test_issue_749_text_layout.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ezdxf-1.0.3b0/LICENSE` & `ezdxf-1.0.4b1/LICENSE`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/NEWS.md` & `ezdxf-1.0.4b1/NEWS.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 
 News
 ====
 
-Version 1.0.3b0 - dev
+Version 1.0.4b1 - dev
 ---------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
+- NEW: added setter to `BlockLayout.base_point` property
+- BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
+- BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
+  scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
+- PREVIEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG,  
+  final release in v1.1
+- PREVIEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF, final release in v1.1
+- PREVIEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG, final release in v1.1
+- PREVIEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF, final release in v1.1
+
+Version 1.0.3 - 2023-03-26
+--------------------------
+
+- Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: [#833](https://github.com/mozman/ezdxf/issues/833)
   logging non-unique entity handles when loading a DXF document as warnings, auditing 
   the document may fix this issue
 - NEW: improved auditing & fixing capabilities
 - NEW: `DXFTagStorage.graphic_properties()` returns the graphical properties for unknown
   or unsupported DXF entities
 - NEW: `GfxAttribs.from_dict()`
 - BUGFIX: audit process preserves dimensional constraints
 - BUGFIX: MTextExplode add-on created invalid text style table entries
 - PREVIEW: `ezdxf.addons.r12export` module to export any DXF document as a simple R12 
   file, final release in v1.1
 - PREVIEW: `ezdxf.r12strict` module to make DXF R12 drawing 100% compatible to Autodesk 
   products, final release in v1.1
+- PREVIEW: `ezdxf.transform` module to apply transformations to multiple DXF entities 
+  in a convenient and safe way, final release in v1.1
 
 Version 1.0.2 - 2023-02-15
 --------------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: `Drawing.validate()` also prints report of resolved issues
 - NEW: copy and transform support for `PDFUNDERLAY`, `DWFUNDERLAY` and `DGNUNDERLAY`
```

## Comparing `ezdxf-1.0.3b0/PKG-INFO` & `ezdxf-1.0.4b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.0.3b0
+Version: 1.0.4b1
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
@@ -92,14 +92,15 @@
 - `MTextExplode` add-on for exploding MTEXT entities into single-line TEXT entities
 - `text2path` add-on to convert text into outline paths
 - `geo` add-on to support the [`__geo_interface__`](https://gist.github.com/sgillies/2217756)
 - `meshex` for exchanging meshes with other tools as STL, OFF or OBJ files
 - `openscad` add-on, an interface to [OpenSCAD](https://openscad.org)
 - `odafc` add-on, an interface to the [ODA File Converter](https://www.opendesign.com/guestfiles/oda_file_converter) 
   to read and write DWG files
+- `hpgl2` add-on for converting HPGL/2 plot files to DXF, SVG and PDF
 
 A simple example:
 
 ```Python
 import ezdxf
 from ezdxf import colors
 from ezdxf.enums import TextEntityAlignment
@@ -209,31 +210,47 @@
 Feedback is greatly appreciated.
 
 Manfred
 
 News
 ====
 
-Version 1.0.3b0 - dev
+Version 1.0.4b1 - dev
 ---------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
+- NEW: added setter to `BlockLayout.base_point` property
+- BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
+- BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
+  scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
+- PREVIEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG,  
+  final release in v1.1
+- PREVIEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF, final release in v1.1
+- PREVIEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG, final release in v1.1
+- PREVIEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF, final release in v1.1
+
+Version 1.0.3 - 2023-03-26
+--------------------------
+
+- Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: [#833](https://github.com/mozman/ezdxf/issues/833)
   logging non-unique entity handles when loading a DXF document as warnings, auditing 
   the document may fix this issue
 - NEW: improved auditing & fixing capabilities
 - NEW: `DXFTagStorage.graphic_properties()` returns the graphical properties for unknown
   or unsupported DXF entities
 - NEW: `GfxAttribs.from_dict()`
 - BUGFIX: audit process preserves dimensional constraints
 - BUGFIX: MTextExplode add-on created invalid text style table entries
 - PREVIEW: `ezdxf.addons.r12export` module to export any DXF document as a simple R12 
   file, final release in v1.1
 - PREVIEW: `ezdxf.r12strict` module to make DXF R12 drawing 100% compatible to Autodesk 
   products, final release in v1.1
+- PREVIEW: `ezdxf.transform` module to apply transformations to multiple DXF entities 
+  in a convenient and safe way, final release in v1.1
 
 Version 1.0.2 - 2023-02-15
 --------------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: `Drawing.validate()` also prints report of resolved issues
 - NEW: copy and transform support for `PDFUNDERLAY`, `DWFUNDERLAY` and `DGNUNDERLAY`
```

## Comparing `ezdxf-1.0.3b0/README.md` & `ezdxf-1.0.4b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 - `MTextExplode` add-on for exploding MTEXT entities into single-line TEXT entities
 - `text2path` add-on to convert text into outline paths
 - `geo` add-on to support the [`__geo_interface__`](https://gist.github.com/sgillies/2217756)
 - `meshex` for exchanging meshes with other tools as STL, OFF or OBJ files
 - `openscad` add-on, an interface to [OpenSCAD](https://openscad.org)
 - `odafc` add-on, an interface to the [ODA File Converter](https://www.opendesign.com/guestfiles/oda_file_converter) 
   to read and write DWG files
+- `hpgl2` add-on for converting HPGL/2 plot files to DXF, SVG and PDF
 
 A simple example:
 
 ```Python
 import ezdxf
 from ezdxf import colors
 from ezdxf.enums import TextEntityAlignment
```

## Comparing `ezdxf-1.0.3b0/setup.py` & `ezdxf-1.0.4b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,16 @@
     try:
         with open(os.path.join(os.path.dirname(__file__), fname)) as f:
             return read_until(f.readlines()) if until else f.read()
     except IOError:
         return "File '%s' not found.\n" % fname
 
 
-DRAW = ["matplotlib", "PySide6", "Pillow"]
-DRAW5 = ["matplotlib", "PyQt5", "Pillow"]
+DRAW = ["matplotlib", "PySide6", "Pillow", "PyMuPDF"]
+DRAW5 = ["matplotlib", "PyQt5", "Pillow", "PyMuPDF"]
 TEST = ["pytest", "geomdl"]
 DEV = ["setuptools", "wheel", "Cython"]
 
 setup(
     name="ezdxf",
     version=get_version(),
     description="A Python package to create/manipulate DXF drawings.",
```

## Comparing `ezdxf-1.0.3b0/integration_tests/check_disable_c_ext_by_config_file.py` & `ezdxf-1.0.4b1/integration_tests/check_disable_c_ext_by_config_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/check_disable_c_ext_by_env_var.py` & `ezdxf-1.0.4b1/integration_tests/check_disable_c_ext_by_env_var.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_acad_table.py` & `ezdxf-1.0.4b1/integration_tests/test_acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_all_dimline_styles.py` & `ezdxf-1.0.4b1/integration_tests/test_all_dimline_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_all_ellipse_transformations.py` & `ezdxf-1.0.4b1/integration_tests/test_all_ellipse_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_anonymous_blocks.py` & `ezdxf-1.0.4b1/integration_tests/test_anonymous_blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_audit_critical_dxf_files.py` & `ezdxf-1.0.4b1/integration_tests/test_audit_critical_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_audit_layouts.py` & `ezdxf-1.0.4b1/integration_tests/test_audit_layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_complex_line_type_2.py` & `ezdxf-1.0.4b1/integration_tests/test_complex_line_type_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_create_basic_graphics.py` & `ezdxf-1.0.4b1/integration_tests/test_create_basic_graphics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_document_guid.py` & `ezdxf-1.0.4b1/integration_tests/test_document_guid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_document_page_setup.py` & `ezdxf-1.0.4b1/integration_tests/test_document_page_setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_drawing_matplotlib_backend.py` & `ezdxf-1.0.4b1/integration_tests/test_drawing_matplotlib_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_drawing_qt_backend.py` & `ezdxf-1.0.4b1/integration_tests/test_drawing_qt_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_dxf_info_scanning.py` & `ezdxf-1.0.4b1/integration_tests/test_dxf_info_scanning.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_entities_iterator.py` & `ezdxf-1.0.4b1/integration_tests/test_entities_iterator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_fix_dulicate_handles.py` & `ezdxf-1.0.4b1/integration_tests/test_fix_dulicate_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_geo.py` & `ezdxf-1.0.4b1/integration_tests/test_geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_groups.py` & `ezdxf-1.0.4b1/integration_tests/test_groups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_ignore_junk_beyond_EOF.py` & `ezdxf-1.0.4b1/integration_tests/test_ignore_junk_beyond_EOF.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_launcher.py` & `ezdxf-1.0.4b1/integration_tests/test_launcher.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_leica_disto_r12.py` & `ezdxf-1.0.4b1/integration_tests/test_leica_disto_r12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_load_dxf_unicode_notation.py` & `ezdxf-1.0.4b1/integration_tests/test_load_dxf_unicode_notation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_mapbox_earcut.py` & `ezdxf-1.0.4b1/integration_tests/test_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_matplotlib_font_support.py` & `ezdxf-1.0.4b1/integration_tests/test_matplotlib_font_support.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_mtext_columns.py` & `ezdxf-1.0.4b1/integration_tests/test_mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_mtext_explode_addon.py` & `ezdxf-1.0.4b1/integration_tests/test_mtext_explode_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_mtext_text_frame.py` & `ezdxf-1.0.4b1/integration_tests/test_mtext_text_frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_new_table_entries.py` & `ezdxf-1.0.4b1/integration_tests/test_new_table_entries.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_none_ascii_read_write.py` & `ezdxf-1.0.4b1/integration_tests/test_none_ascii_read_write.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_odafc.py` & `ezdxf-1.0.4b1/integration_tests/test_odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_open_binary_DXF_files.py` & `ezdxf-1.0.4b1/integration_tests/test_open_binary_DXF_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_open_coord_order_issue.py` & `ezdxf-1.0.4b1/integration_tests/test_open_coord_order_issue.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_open_exotic_dxf_files.py` & `ezdxf-1.0.4b1/integration_tests/test_open_exotic_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_open_R13_R14.py` & `ezdxf-1.0.4b1/integration_tests/test_open_R13_R14.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_polyline_entity.py` & `ezdxf-1.0.4b1/integration_tests/test_polyline_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_preserve_binary_data_in_xrecords.py` & `ezdxf-1.0.4b1/integration_tests/test_preserve_binary_data_in_xrecords.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_r12export.py` & `ezdxf-1.0.4b1/integration_tests/test_r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_r12strict.py` & `ezdxf-1.0.4b1/integration_tests/test_r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_r12writer.py` & `ezdxf-1.0.4b1/integration_tests/test_r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_read_file_without_handles.py` & `ezdxf-1.0.4b1/integration_tests/test_read_file_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_read_write_modern_entites.py` & `ezdxf-1.0.4b1/integration_tests/test_read_write_modern_entites.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_recover.py` & `ezdxf-1.0.4b1/integration_tests/test_recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_redraw_order.py` & `ezdxf-1.0.4b1/integration_tests/test_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_rotated_block_attributes.py` & `ezdxf-1.0.4b1/integration_tests/test_rotated_block_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_surface_entities.py` & `ezdxf-1.0.4b1/integration_tests/test_surface_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_write_fixed_meta_data.py` & `ezdxf-1.0.4b1/integration_tests/test_write_fixed_meta_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/test_write_without_handles.py` & `ezdxf-1.0.4b1/integration_tests/test_write_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/AC1003_LINE_Example.dxf` & `ezdxf-1.0.4b1/integration_tests/data/AC1003_LINE_Example.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/acad_table_with_blk_ref.dxf` & `ezdxf-1.0.4b1/integration_tests/data/acad_table_with_blk_ref.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/ASCII_R12.dxf` & `ezdxf-1.0.4b1/integration_tests/data/ASCII_R12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/bin_dxf_r12.dxf` & `ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/bin_dxf_r13.dxf` & `ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/bin_dxf_r14.dxf` & `ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/bin_dxf_r2000.dxf` & `ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r2000.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/cc_dxflib.dxf` & `ezdxf-1.0.4b1/integration_tests/data/cc_dxflib.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/custom_blocks.dxf` & `ezdxf-1.0.4b1/integration_tests/data/custom_blocks.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/duplicate_handles.dxf` & `ezdxf-1.0.4b1/integration_tests/data/duplicate_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/dxf_unicode.dxf` & `ezdxf-1.0.4b1/integration_tests/data/dxf_unicode.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/empty_handles.dxf` & `ezdxf-1.0.4b1/integration_tests/data/empty_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/groups.dxf` & `ezdxf-1.0.4b1/integration_tests/data/groups.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/Leica_Disto_S910.dxf` & `ezdxf-1.0.4b1/integration_tests/data/Leica_Disto_S910.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/MODEL.dxf` & `ezdxf-1.0.4b1/integration_tests/data/MODEL.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/mtext_columns_R2007.dxf` & `ezdxf-1.0.4b1/integration_tests/data/mtext_columns_R2007.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/mtext_columns_R2018.dxf` & `ezdxf-1.0.4b1/integration_tests/data/mtext_columns_R2018.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/mtext_framed_columns.dxf` & `ezdxf-1.0.4b1/integration_tests/data/mtext_framed_columns.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/mtext_text_frame.dxf` & `ezdxf-1.0.4b1/integration_tests/data/mtext_text_frame.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/no_layouts.dxf` & `ezdxf-1.0.4b1/integration_tests/data/no_layouts.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/POLI-ALL210_12.DXF` & `ezdxf-1.0.4b1/integration_tests/data/POLI-ALL210_12.DXF`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/recover01.dxf` & `ezdxf-1.0.4b1/integration_tests/data/recover01.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/recover02.dxf` & `ezdxf-1.0.4b1/integration_tests/data/recover02.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/small_r13.dxf` & `ezdxf-1.0.4b1/integration_tests/data/small_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/small_r14.dxf` & `ezdxf-1.0.4b1/integration_tests/data/small_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/XRECORD_0.bin` & `ezdxf-1.0.4b1/integration_tests/data/XRECORD_0.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/XRECORD_1.bin` & `ezdxf-1.0.4b1/integration_tests/data/XRECORD_1.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/integration_tests/data/XRECORD_2.bin` & `ezdxf-1.0.4b1/integration_tests/data/XRECORD_2.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/appsettings.py` & `ezdxf-1.0.4b1/src/ezdxf/appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/audit.py` & `ezdxf-1.0.4b1/src/ezdxf/audit.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,15 @@
             if handle == self._rootdict_handle or entity.dxftype() == "TABLE":
                 return  # '0' handle as owner is valid
         if owner_handle not in doc.entitydb:
             if handle == self._rootdict_handle:
                 entity.dxf.owner = "0"
                 self.fixed_error(
                     code=AuditError.INVALID_OWNER_HANDLE,
-                    message=f"Fixed invalid owner handle in root {str(self)}.",
+                    message=f"Fixed invalid owner handle in root {str(entity)}.",
                 )
             elif entity.dxftype() == "TABLE":
                 name = entity.dxf.get("name", "UNKNOWN")
                 entity.dxf.owner = "0"
                 self.fixed_error(
                     code=AuditError.INVALID_OWNER_HANDLE,
                     message=f"Fixed invalid owner handle for {name} table.",
@@ -452,27 +452,27 @@
                 self.trash(doc.entitydb.get(handle))  # type: ignore
 
     def check_extrusion_vector(self, entity: DXFEntity) -> None:
         if NULLVEC.isclose(entity.dxf.extrusion):
             entity.dxf.discard("extrusion")
             self.fixed_error(
                 code=AuditError.INVALID_EXTRUSION_VECTOR,
-                message=f"Fixed extrusion vector for entity: {str(self)}.",
+                message=f"Fixed extrusion vector for entity: {str(entity)}.",
                 dxf_entity=entity,
             )
 
     def check_transparency(self, entity: DXFEntity) -> None:
         value = entity.dxf.transparency
         if value is None:
             return
         if not validator.is_transparency(value):
             entity.dxf.discard("transparency")
             self.fixed_error(
                 code=AuditError.INVALID_TRANSPARENCY,
-                message=f"Fixed invalid transparency for entity: {str(self)}.",
+                message=f"Fixed invalid transparency for entity: {str(entity)}.",
                 dxf_entity=entity,
             )
 
     def check_block_reference_cycles(self) -> None:
         cycle_detector = BlockCycleDetector(self.doc)
         for block in self.doc.blocks:
             if cycle_detector.has_cycle(block.name):
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/bbox.py` & `ezdxf-1.0.4b1/src/ezdxf/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/blkrefs.py` & `ezdxf-1.0.4b1/src/ezdxf/blkrefs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/colors.py` & `ezdxf-1.0.4b1/src/ezdxf/colors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/commands.py` & `ezdxf-1.0.4b1/src/ezdxf/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -126,17 +126,15 @@
 class Audit(Command):
     """Launcher sub-command: audit"""
 
     NAME = "audit"
 
     @staticmethod
     def add_parser(subparsers):
-        parser = subparsers.add_parser(
-            Audit.NAME, help="audit and repair DXF files"
-        )
+        parser = subparsers.add_parser(Audit.NAME, help="audit and repair DXF files")
         parser.add_argument(
             "files",
             metavar="FILE",
             nargs="+",
             help="audit DXF files",
         )
         parser.add_argument(
@@ -242,17 +240,15 @@
     except const.DXFStructureError:
         msg = f'Invalid or corrupted DXF file: "{filename}"'
         print(msg, file=sys.stderr)
         sys.exit(3)
 
     if auditor.has_errors:
         # But is most likely good enough for rendering.
-        msg = (
-            f"Audit process found {len(auditor.errors)} unrecoverable error(s)."
-        )
+        msg = f"Audit process found {len(auditor.errors)} unrecoverable error(s)."
         print(msg)
         logger.error(msg)
     if auditor.has_fixes:
         msg = f"Audit process fixed {len(auditor.fixes)} error(s)."
         print(msg)
         logger.info(msg)
     return doc, auditor
@@ -261,16 +257,15 @@
 HELP_LTYPE = (
     "select the line type rendering method, default is approximate. "
     "Approximate uses the closest approximation available to the "
     "backend, the accurate method renders as accurately as possible "
     "but this approach is slower."
 )
 HELP_LWSCALE = (
-    "set custom line weight scaling, default is 0 to disable line "
-    "weights at all"
+    "set custom line weight scaling, default is 0 to disable line " "weights at all"
 )
 
 
 @register
 class Draw(Command):
     """Launcher sub-command: draw"""
 
@@ -589,44 +584,34 @@
         layout_properties = LayoutProperties.from_layout(layout)
         if bg is not None:
             if not bg.startswith("#"):
                 bg = "#" + bg
             try:
                 layout_properties.set_colors(bg)
             except ValueError:
-                print(
-                    f'ERROR: invalid background color value "{args.background}"'
-                )
+                print(f'ERROR: invalid background color value "{args.background}"')
                 sys.exit(4)
 
         ctx = RenderContext(doc)
         # force accurate linetype rendering by the frontend
-        config = Configuration.defaults().with_changes(
-            line_policy=LinePolicy.ACCURATE
-        )
+        config = Configuration.defaults().with_changes(line_policy=LinePolicy.ACCURATE)
         if verbose:
             print(f"detecting extents...\n")
         bbox_cache = bbox.Cache()
         if layout.is_any_paperspace:
             # get entity bounding boxes in modelspace for faster paperspace
             # rendering
             bbox.extents(doc.modelspace(), fast=True, cache=bbox_cache)
         extents = bbox.extents(layout, fast=True, cache=bbox_cache)
         img_x, img_y = parse_image_size(args.image_size)
         if verbose:
             print(f"    units: {units.unit_name(layout.units)}")
-            print(
-                f"    modelspace size: {extents.size.x:.3f} x {extents.size.y:.3f}"
-            )
-            print(
-                f"    min extents: ({extents.extmin.x:.3f}, {extents.extmin.y:.3f})"
-            )
-            print(
-                f"    max extents: ({extents.extmax.x:.3f}, {extents.extmax.y:.3f})"
-            )
+            print(f"    modelspace size: {extents.size.x:.3f} x {extents.size.y:.3f}")
+            print(f"    min extents: ({extents.extmin.x:.3f}, {extents.extmin.y:.3f})")
+            print(f"    max extents: ({extents.extmax.x:.3f}, {extents.extmax.y:.3f})")
             print(f"\nimage size: {img_x} x {img_y}")
         try:
             out = PillowBackend(
                 extents,
                 image_size=(img_x, img_y),
                 oversampling=args.oversampling,
                 margin=args.margin,
@@ -674,17 +659,15 @@
 class Browse(Command):
     """Launcher sub-command: browse"""
 
     NAME = "browse"
 
     @staticmethod
     def add_parser(subparsers):
-        parser = subparsers.add_parser(
-            Browse.NAME, help="browse DXF file structure"
-        )
+        parser = subparsers.add_parser(Browse.NAME, help="browse DXF file structure")
         parser.add_argument(
             "file",
             metavar="FILE",
             nargs="?",
             help="DXF file to browse",
         )
         parser.add_argument(
@@ -769,17 +752,15 @@
 class Strip(Command):
     """Launcher sub-command: strip"""
 
     NAME = "strip"
 
     @staticmethod
     def add_parser(subparsers):
-        parser = subparsers.add_parser(
-            Strip.NAME, help="strip comments from DXF files"
-        )
+        parser = subparsers.add_parser(Strip.NAME, help="strip comments from DXF files")
         parser.add_argument(
             "file",
             metavar="FILE",
             nargs="+",
             help='DXF file to process, wildcards "*" and "?" are supported',
         )
         parser.add_argument(
@@ -987,17 +968,241 @@
                         process(filename2)
                         file_count += 1
                 else:
                     process(filename)
                     file_count += 1
 
             if file_count == 0:
-                sys.stderr.write(
-                    f'No matching files for pattern: "{pattern}"\n'
-                )
+                sys.stderr.write(f'No matching files for pattern: "{pattern}"\n')
+
+
+def make_plt2fmt_parser(subparsers, name, fmt):
+    parser = subparsers.add_parser(name, help=f"convert HPGL/2 plot files to {fmt}")
+    parser.add_argument(
+        "files",
+        metavar="FILE",
+        nargs="+",
+        help=f"convert HPGL/2 plot files to {fmt}, wildcards (*, ?) supported",
+    )
+    parser.add_argument(
+        "-r",
+        "--rotate",
+        type=int,
+        choices=(0, 90, 180, 270),
+        default=0,
+        required=False,
+        help="rotate page about 90, 180 or 270 degrees",
+    )
+    parser.add_argument(
+        "-x",
+        "--scale_x",
+        type=float,
+        metavar="SX",
+        default=1.0,
+        required=False,
+        help="scale page in x-axis direction, use negative values to mirror page",
+    )
+    parser.add_argument(
+        "-y",
+        "--scale_y",
+        type=float,
+        metavar="SY",
+        default=1.0,
+        required=False,
+        help="scale page in y-axis direction, use negative values to mirror page",
+    )
+    parser.add_argument(
+        "-m",
+        "--merge_control",
+        type=int,
+        required=False,
+        default=2,
+        choices=(0, 1, 2),
+        help="provides control over the order of filled polygons, 0=off (print order), "
+        "1=luminance (order by luminance), 2=auto (default)",
+    )
+    parser.add_argument(
+        "-f",
+        "--force",
+        action="store_true",
+        required=False,
+        help="inserts the mandatory 'enter HPGL/2 mode' escape sequence into the data "
+        "stream; use this flag when no HPGL/2 data was found and you are sure the "
+        "file is a HPGL/2 plot file",
+    )
+    return parser
+
+
+@register
+class Plt2Dxf(Command):
+    """Launcher sub-command: plt2dxf"""
+
+    NAME = "plt2dxf"
+
+    @staticmethod
+    def add_parser(subparsers):
+        parser = make_plt2fmt_parser(subparsers, Plt2Dxf.NAME, "DXF")
+        parser.epilog = "Note that plot files are intended to be plotted on white paper."
+        parser.add_argument(
+            "--aci",
+            action="store_true",
+            required=False,
+            help="use pen numbers as ACI colors",
+        )
+        parser.add_argument(
+            "--map_black_to_white",
+            action="store_true",
+            required=False,
+            help="map black RGB plot colors (and only real black (0, 0, 0)) to white RGB, "
+            "does not affect ACI colors",
+        )
+
+    @staticmethod
+    def run(args):
+        from ezdxf.addons.hpgl2 import api as hpgl2
+        from ezdxf.addons.hpgl2.dxf_backend import ColorMode
+
+        def _convert(filepath: Path) -> None:
+            msg = f"converting HPGL/2 plot file to DXF: {filename}"
+            print(msg)
+            try:
+                data = filepath.read_bytes()
+            except IOError as e:
+                print(str(e), file=sys.stderr)
+                return
+            if args.force:
+                data = b"%1B" + data
+
+            color_mode = ColorMode.ACI if args.aci else ColorMode.RGB
+            doc = hpgl2.to_dxf(
+                data,
+                rotation=args.rotate,
+                sx=args.scale_x,
+                sy=args.scale_y,
+                color_mode=color_mode,
+                map_black_rgb_to_white_rgb=args.map_black_to_white,
+                merge_control=args.merge_control,
+            )
+            dxf_filepath = filepath.with_suffix(".dxf")
+            try:
+                doc.saveas(dxf_filepath)
+            except IOError as e:
+                print(str(e), file=sys.stderr)
+
+        for pattern in args.files:
+            names = list(glob.glob(pattern))
+            if len(names) == 0:
+                msg = f"File(s) '{pattern}' not found."
+                print(msg, file=sys.stderr)
+                logger.error(msg)
+                continue
+            for filename in names:
+                _convert(Path(filename))
+
+
+@register
+class Plt2Svg(Command):
+    """Launcher sub-command: plt2svg"""
+
+    NAME = "plt2svg"
+
+    @staticmethod
+    def add_parser(subparsers):
+        make_plt2fmt_parser(subparsers, Plt2Svg.NAME, "SVG")
+
+    @staticmethod
+    def run(args):
+        from ezdxf.addons.hpgl2 import api as hpgl2
+
+        def _convert(filepath: Path) -> None:
+            msg = f"converting HPGL/2 plot file to SVG: {filename}"
+            print(msg)
+            logger.info(msg)
+            try:
+                data = filepath.read_bytes()
+            except IOError as e:
+                print(str(e), file=sys.stderr)
+                return
+
+            if args.force:
+                data = b"%1B" + data
+
+            svg_string = hpgl2.to_svg(
+                data,
+                rotation=args.rotate,
+                sx=args.scale_x,
+                sy=args.scale_y,
+                merge_control=args.merge_control,
+            )
+            svg_filepath = filepath.with_suffix(".svg")
+            try:
+                svg_filepath.write_text(svg_string)
+            except IOError as e:
+                print(str(e), file=sys.stderr)
+
+        for pattern in args.files:
+            names = list(glob.glob(pattern))
+            if len(names) == 0:
+                msg = f"File(s) '{pattern}' not found."
+                print(msg)
+                logger.error(msg)
+                continue
+            for filename in names:
+                _convert(Path(filename))
+
+
+@register
+class Plt2Pdf(Command):
+    """Launcher sub-command: plt2pdf"""
+
+    NAME = "plt2pdf"
+
+    @staticmethod
+    def add_parser(subparsers):
+        make_plt2fmt_parser(subparsers, Plt2Pdf.NAME, "PDF")
+
+    @staticmethod
+    def run(args):
+        from ezdxf.addons.hpgl2 import api as hpgl2
+
+        def _convert(filepath: Path) -> None:
+            msg = f"converting HPGL/2 plot file to PDF: {filename}"
+            print(msg)
+            logger.info(msg)
+            try:
+                data = filepath.read_bytes()
+            except IOError as e:
+                print(str(e), file=sys.stderr)
+                return
+
+            if args.force:
+                data = b"%1B" + data
+
+            pdf_bytes = hpgl2.to_pdf(
+                data,
+                rotation=args.rotate,
+                sx=args.scale_x,
+                sy=args.scale_y,
+                merge_control=args.merge_control,
+            )
+            pdf_filepath = filepath.with_suffix(".pdf")
+            try:
+                pdf_filepath.write_bytes(pdf_bytes)
+            except IOError as e:
+                print(str(e), file=sys.stderr)
+
+        for pattern in args.files:
+            names = list(glob.glob(pattern))
+            if len(names) == 0:
+                msg = f"File(s) '{pattern}' not found."
+                print(msg)
+                logger.error(msg)
+                continue
+            for filename in names:
+                _convert(Path(filename))
 
 
 def set_app_icon(app):
     from ezdxf.addons.xqt import QtGui, QtCore
 
     app_icon = QtGui.QIcon()
     p = resources_path()
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/comments.py` & `ezdxf-1.0.4b1/src/ezdxf/comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/disassemble.py` & `ezdxf-1.0.4b1/src/ezdxf/disassemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,15 +537,15 @@
     if max_flattening_distance:
         primitive.max_flattening_distance = max_flattening_distance
     return primitive
 
 
 def recursive_decompose(entities: Iterable[DXFEntity]) -> Iterable[DXFEntity]:
     """Recursive decomposition of the given DXF entity collection into a flat
-    DXF entity stream. All block references (INSERT) and entities which provide
+    stream of DXF entities. All block references (INSERT) and entities which provide
     a :meth:`virtual_entities` method will be disassembled into simple DXF
     sub-entities, therefore the returned entity stream does not contain any
     INSERT entity.
 
     Point entities will **not** be disassembled into DXF sub-entities,
     as defined by the current point style $PDMODE.
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/document.py` & `ezdxf-1.0.4b1/src/ezdxf/document.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/dwginfo.py` & `ezdxf-1.0.4b1/src/ezdxf/dwginfo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entitydb.py` & `ezdxf-1.0.4b1/src/ezdxf/entitydb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/enums.py` & `ezdxf-1.0.4b1/src/ezdxf/enums.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/explode.py` & `ezdxf-1.0.4b1/src/ezdxf/explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/eztypes.py` & `ezdxf-1.0.4b1/src/ezdxf/eztypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/filemanagement.py` & `ezdxf-1.0.4b1/src/ezdxf/filemanagement.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/gfxattribs.py` & `ezdxf-1.0.4b1/src/ezdxf/gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/graphicsfactory.py` & `ezdxf-1.0.4b1/src/ezdxf/graphicsfactory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/groupby.py` & `ezdxf-1.0.4b1/src/ezdxf/groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/protocols.py` & `ezdxf-1.0.4b1/src/ezdxf/protocols.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/proxygraphic.py` & `ezdxf-1.0.4b1/src/ezdxf/proxygraphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/query.py` & `ezdxf-1.0.4b1/src/ezdxf/query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/queryparser.py` & `ezdxf-1.0.4b1/src/ezdxf/queryparser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/r12strict.py` & `ezdxf-1.0.4b1/src/ezdxf/r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/recover.py` & `ezdxf-1.0.4b1/src/ezdxf/recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/reorder.py` & `ezdxf-1.0.4b1/src/ezdxf/reorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/shapefile.py` & `ezdxf-1.0.4b1/src/ezdxf/shapefile.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/units.py` & `ezdxf-1.0.4b1/src/ezdxf/units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/upright.py` & `ezdxf-1.0.4b1/src/ezdxf/upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/urecord.py` & `ezdxf-1.0.4b1/src/ezdxf/urecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/version.py` & `ezdxf-1.0.4b1/src/ezdxf/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # examples:
 #   major pre-release alpha 2: VERSION = "0.9.0a2"; version = (0, 9, 0, 'a2')
 #   major release candidate 0: VERSION = "0.9.0rc0"; version = (0, 9, 0, 'rc0')
 #   major release: VERSION = "0.9.0"; version = (0, 9, 0, 'release')
 #   1. bug fix release beta0: VERSION = "0.9.1b0"; version = (0, 9, 1, 'b0')
 #   2. bug fix release: VERSION = "0.9.2"; version = (0, 9, 2, 'release')
 
-version = (1, 0, 3, "b0")
-__version__ = "1.0.3b0"
+version = (1, 0, 4, "b1")
+__version__ = "1.0.4b1"
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/xref.py` & `ezdxf-1.0.4b1/src/ezdxf/xref.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,18 @@
     "load_paperspace",
     "Registry",
     "ResourceMapper",
     "ConflictPolicy",
     "Loader",
     "dxf_info",
     "DXFInfo",
+    "XrefError",
+    "XrefDefinitionError",
+    "EntityError",
+    "LayoutError",
 ]
 
 logger = logging.getLogger("ezdxf")
 NO_BLOCK = "0"
 DEFAULT_LINETYPES = {"CONTINUOUS", "BYLAYER", "BYBLOCK"}
 DEFAULT_LAYER = "0"
 STANDARD = "STANDARD"
@@ -73,14 +77,36 @@
 # I prefer to see the debug messages stored in the object, because I mostly debug test
 # code and pytest does not show logging or print messages by default.
 def _log_debug_messages(messages: Iterable[str]) -> None:
     for msg in messages:
         logger.debug(msg)
 
 
+class XrefError(Exception):
+    """base exception for the xref module"""
+
+    pass
+
+
+class XrefDefinitionError(XrefError):
+    pass
+
+
+class EntityError(XrefError):
+    pass
+
+
+class LayoutError(XrefError):
+    pass
+
+
+class InternalError(XrefError):
+    pass
+
+
 class ConflictPolicy(enum.Enum):
     # What to do when a name conflict of existing and loaded resources occur:
     # keep existing resource <name> and ignore loaded resource
     KEEP = enum.auto()
 
     # ALWAYS rename imported resources to <xref>$0$<name>
     # This is the default behavior of BricsCAD when binding an external reference.
@@ -188,26 +214,35 @@
     Args:
         doc: host document
         block_name: name of the xref block
         filename: external reference filename
         overlay: creates an XREF overlay if ``True`` and an XREF attachment otherwise
 
     Raises:
-        ValueError: block with same name exist
+        XrefDefinitionError: block with same name exist
 
     .. versionadded:: 1.1
 
     """
     if block_name in doc.blocks:
-        raise ValueError(f"block '{block_name}' already exist")
+        raise XrefDefinitionError(f"block '{block_name}' already exist")
+    doc.blocks.new(
+        name=block_name,
+        dxfattribs={
+            "flags": make_xref_flags(overlay),
+            "xref_path": filename,
+        },
+    )
+
+
+def make_xref_flags(overlay: bool) -> int:
     if overlay:
-        flags = const.BLK_XREF_OVERLAY | const.BLK_EXTERNAL
+        return const.BLK_XREF_OVERLAY | const.BLK_EXTERNAL
     else:
-        flags = const.BLK_XREF | const.BLK_EXTERNAL
-    doc.blocks.new(name=block_name, dxfattribs={"flags": flags, "xref_path": filename})
+        return const.BLK_XREF | const.BLK_EXTERNAL
 
 
 def attach(
     doc: Drawing,
     *,
     block_name: str,
     filename: str,
@@ -242,15 +277,15 @@
         rotation: rotation angle in degrees
         overlay: creates an XREF overlay if ``True`` and an XREF attachment otherwise
 
     Returns:
         Insert: default block reference for the XREF
 
     Raises:
-        ValueError: block with same name exist
+        XrefDefinitionError: block with same name exist
 
     .. versionadded:: 1.1
 
     """
     define(doc, block_name, filename, overlay=overlay)
     dxfattribs = dict()
     if rotation:
@@ -317,34 +352,34 @@
         xref: :class:`BlockLayout` of the XREF document
         load_fn: function to load the content of the XREF as `Drawing` object
         search_paths: list of folders to search for XREFS, default is the folder of the
             host document or the current directory if no filepath is set
         conflict_policy: how to resolve name conflicts
 
     Raises:
-        ValueError: argument `xref` is not a XREF definition
+        XrefDefinitionError: argument `xref` is not a XREF definition
         FileNotFoundError: XREF file not found
         DXFVersionError: cannot load a XREF with a newer DXF version than the host
             document, try the :mod:`~ezdxf.addons.odafc` add-on to downgrade the XREF
             document or upgrade the host document
 
     .. versionadded:: 1.1
 
     """
     assert isinstance(xref, BlockLayout), "expected BLOCK definition of XREF"
     target_doc = xref.doc
     assert target_doc is not None, "valid DXF document required"
     block = xref.block
     assert isinstance(block, Block)
     if not block.is_xref:
-        raise ValueError("argument 'xref' is not a XREF definition")
+        raise XrefDefinitionError("argument 'xref' is not a XREF definition")
 
     xref_path: str = block.dxf.get("xref_path", "")
     if not xref_path:
-        raise ValueError("no xref path defined")
+        raise XrefDefinitionError("no xref path defined")
 
     _search_paths = [pathlib.Path(p) for p in search_paths]
     _search_paths.insert(0, target_doc.get_abs_filepath())
 
     filepath = find_xref(xref_path, _search_paths)
     if not filepath.exists():
         raise FileNotFoundError(f"file not found: '{filepath}'")
@@ -364,32 +399,61 @@
     block.set_flag_state(const.BLK_XREF | const.BLK_EXTERNAL, state=False)
     # update BLOCK origin:
     origin = source_doc.header.get("$INSBASE")
     if origin:
         block.dxf.base_point = Vec3(origin)
 
 
-def detach(block: BlockLayout, *, xref_filename: str) -> Drawing:
+def detach(
+    block: BlockLayout, *, xref_filename: str | os.PathLike, overlay=False
+) -> Drawing:
     """Write the content of `block` into the modelspace of a new DXF document and
     convert `block` to an external reference (XREF).  The new DXF document has to be
     written by the caller: :code:`xref_doc.saveas(xref_filename)`.
     This way it is possible to convert the DXF document to DWG by the
     :mod:`~ezdxf.addons.odafc` add-on if necessary::
 
         xref_doc = xref.detach(my_block, "my_block.dwg")
         odafc.export_dwg(xref_doc, "my_block.dwg")
 
+    It's recommended to clean up the entity database of the host document afterwards::
+
+        doc.entitydb.purge()
+
     Args:
         block: block definition to detach
         xref_filename: name of the external referenced file
+        overlay: creates an XREF overlay if ``True`` and an XREF attachment otherwise
 
     .. versionadded:: 1.1
 
     """
-    raise NotImplementedError()
+    source_doc = block.doc
+    assert source_doc is not None, "valid DXF document required"
+    target_doc = ezdxf.new(dxfversion=source_doc.dxfversion, units=block.units)
+    loader = Loader(source_doc, target_doc, conflict_policy=ConflictPolicy.KEEP)
+    loader.load_block_layout_into(block, target_doc.modelspace())
+    loader.execute()
+    target_doc.header["$INSBASE"] = block.base_point
+    block_to_xref(block, xref_filename, overlay=overlay)
+    return target_doc
+
+
+def block_to_xref(
+    block: BlockLayout, xref_filename: str | os.PathLike, *, overlay=False
+) -> None:
+    """Convert a block definition into an external reference.
+
+    (internal API)
+    """
+    block.delete_all_entities()
+    block_entity = block.block
+    assert block_entity is not None, "invalid BlockLayout"
+    block_entity.dxf.xref_path = str(xref_filename)
+    block_entity.dxf.flags = make_xref_flags(overlay)
 
 
 def write_block(entities: Sequence[DXFEntity], *, origin: UVec = (0, 0, 0)) -> Drawing:
     """Write `entities` into the modelspace of a new DXF document.
 
     This function is called "write_block" because the new DXF document can be used as
     an external referenced block.  This function is similar to the WBLOCK command in CAD
@@ -400,23 +464,23 @@
 
     Args:
         entities: DXF entities to write
         origin: block origin, defines the point in the modelspace which will be inserted
             at the insert location of the block reference
 
     Raises:
-        ValueError: virtual entities are not supported
+        EntityError: virtual entities are not supported
 
     .. versionadded:: 1.1
 
     """
     if len(entities) == 0:
         return ezdxf.new()
     if any(e.dxf.owner is None for e in entities):
-        raise ValueError("virtual entities are not supported")
+        raise EntityError("virtual entities are not supported")
     source_doc = entities[0].doc
     assert source_doc is not None, "expected a valid source document"
     target_doc = ezdxf.new(dxfversion=source_doc.dxfversion, units=source_doc.units)
     loader = Loader(source_doc, target_doc)
     loader.add_command(LoadEntities(entities, target_doc.modelspace()))
     loader.execute()
     target_doc.header["$INSBASE"] = Vec3(origin)
@@ -459,15 +523,15 @@
         psp: paperspace layout to load
         tdoc: target document
         filter_fn: optional function to filter entities from the source paperspace layout
         conflict_policy: how to resolve name conflicts
 
     """
     if psp.doc is tdoc:
-        raise const.DXFValueError("Paperspace layout cannot be from target document.")
+        raise LayoutError("Source paperspace layout cannot be from target document.")
     loader = Loader(psp.doc, tdoc, conflict_policy=conflict_policy)
     loader.load_paperspace_layout(psp, filter_fn=filter_fn)
     loader.execute()
 
 
 class Registry(Protocol):
     def add_entity(self, entity: DXFEntity, block_key: str = NO_BLOCK) -> None:
@@ -549,17 +613,15 @@
     """Loads all given entities into the target layout."""
 
     def __init__(
         self, entities: Sequence[DXFEntity], target_layout: BaseLayout
     ) -> None:
         self.entities = entities
         if not isinstance(target_layout, BaseLayout):
-            raise const.DXFTypeError(
-                f"invalid target layout type: {type(target_layout)}"
-            )
+            raise LayoutError(f"invalid target layout type: {type(target_layout)}")
         self.target_layout = target_layout
 
     def register_resources(self, registry: Registry) -> None:
         for e in self.entities:
             registry.add_entity(e, block_key=e.dxf.owner)
 
     def execute(self, transfer: _Transfer) -> None:
@@ -591,15 +653,15 @@
     """Loads a paperspace layout as a new paperspace layout into the target document.
     If a paperspace layout with same name already exists the layout will be renamed
     to  "<layout name> (x)" where x is 2 or the next free number.
     """
 
     def __init__(self, psp: Paperspace, filter_fn: Optional[FilterFunction]) -> None:
         if not isinstance(psp, Paperspace):
-            raise const.DXFTypeError(f"invalid paperspace layout type: {type(psp)}")
+            raise LayoutError(f"invalid paperspace layout type: {type(psp)}")
         self.paperspace_layout = psp
         self.filter_fn = filter_fn
 
     def source_entities(self) -> list[DXFEntity]:
         filter_fn = self.filter_fn
         if filter_fn:
             return [e for e in self.paperspace_layout if filter_fn(e)]
@@ -633,15 +695,15 @@
 class LoadBlockLayout(LoadingCommand):
     """Loads a block layout as a new block layout into the target document. If a block
     layout with the same name exists the conflict policy will be applied.
     """
 
     def __init__(self, block: BlockLayout) -> None:
         if not isinstance(block, BlockLayout):
-            raise const.DXFTypeError(f"invalid block layout type: {type(block)}")
+            raise LayoutError(f"invalid block layout type: {type(block)}")
         self.block_layout = block
 
     def register_resources(self, registry: Registry) -> None:
         block_record = self.block_layout.block_record
         if isinstance(block_record, BlockRecord):
             registry.add_entity(block_record)
 
@@ -691,19 +753,17 @@
         the target document, the modelspace of the target document is the default target
         layout.  The target layout can be any layout: modelspace, paperspace layout or
         block layout.
         """
         if target_layout is None:
             target_layout = self.tdoc.modelspace()
         elif not isinstance(target_layout, BaseLayout):
-            raise const.DXFTypeError(
-                f"invalid target layout type: {type(target_layout)}"
-            )
+            raise LayoutError(f"invalid target layout type: {type(target_layout)}")
         if target_layout.doc is not self.tdoc:
-            raise const.DXFValueError(
+            raise LayoutError(
                 f"given target layout does not belong to the target document"
             )
         if filter_fn is None:
             entities = list(self.sdoc.modelspace())
         else:
             entities = [e for e in self.sdoc.modelspace() if filter_fn(e)]
         self.add_command(LoadEntities(entities, target_layout))
@@ -718,15 +778,15 @@
         to  "<layout name> (2)" or "<layout name> (3)" and so on. The content of the
         modelspace which may be displayed through a VIEWPORT entity will **not** be
         loaded!
         """
         if not isinstance(psp, Paperspace):
             raise const.DXFTypeError(f"invalid paperspace layout type: {type(psp)}")
         if psp.doc is not self.sdoc:
-            raise const.DXFValueError(
+            raise LayoutError(
                 f"given paperspace layout does not belong to the source document"
             )
         self.add_command(LoadPaperspaceLayout(psp, filter_fn))
 
     def load_paperspace_layout_into(
         self,
         psp: Paperspace,
@@ -735,25 +795,23 @@
     ) -> None:
         """Loads the content of a paperspace layout into an existing layout of the target
         document. The target layout can be any layout: modelspace, paperspace layout
         or block layout.  The content of the modelspace which may be displayed through a
         VIEWPORT entity will **not** be loaded!
         """
         if not isinstance(psp, Paperspace):
-            raise const.DXFTypeError(f"invalid paperspace layout type: {type(psp)}")
+            raise LayoutError(f"invalid paperspace layout type: {type(psp)}")
         if not isinstance(target_layout, BaseLayout):
-            raise const.DXFTypeError(
-                f"invalid target layout type: {type(target_layout)}"
-            )
+            raise LayoutError(f"invalid target layout type: {type(target_layout)}")
         if psp.doc is not self.sdoc:
-            raise const.DXFValueError(
+            raise LayoutError(
                 f"given paperspace layout does not belong to the source document"
             )
         if target_layout.doc is not self.tdoc:
-            raise const.DXFValueError(
+            raise LayoutError(
                 f"given target layout does not belong to the target document"
             )
         if filter_fn is None:
             entities = list(psp)
         else:
             entities = [e for e in psp if filter_fn(e)]
         self.add_command(LoadEntities(entities, target_layout))
@@ -763,17 +821,17 @@
         block_layout: BlockLayout,
     ) -> None:
         """Loads a block layout (block definition) as a new block layout into the target
         document. If a block layout with the same name exists the conflict policy will
         be applied.  This method cannot load modelspace or paperspace layouts.
         """
         if not isinstance(block_layout, BlockLayout):
-            raise const.DXFTypeError(f"invalid block layout type: {type(block_layout)}")
+            raise LayoutError(f"invalid block layout type: {type(block_layout)}")
         if block_layout.doc is not self.sdoc:
-            raise const.DXFValueError(
+            raise LayoutError(
                 f"given block layout does not belong to the source document"
             )
         self.add_command(LoadBlockLayout(block_layout))
 
     def load_block_layout_into(
         self,
         block_layout: BlockLayout,
@@ -781,25 +839,23 @@
     ) -> None:
         """Loads the content of a block layout (block definition) into an existing layout
         of the target document. The target layout can be any layout: modelspace,
         paperspace layout or block layout.  This method cannot load the content of
         modelspace or paperspace layouts.
         """
         if not isinstance(block_layout, BlockLayout):
-            raise const.DXFTypeError(f"invalid block layout type: {type(block_layout)}")
+            raise LayoutError(f"invalid block layout type: {type(block_layout)}")
         if not isinstance(target_layout, BaseLayout):
-            raise const.DXFTypeError(
-                f"invalid target layout type: {type(target_layout)}"
-            )
+            raise LayoutError(f"invalid target layout type: {type(target_layout)}")
         if block_layout.doc is not self.sdoc:
-            raise const.DXFValueError(
+            raise LayoutError(
                 f"given block layout does not belong to the source document"
             )
         if target_layout.doc is not self.tdoc:
-            raise const.DXFValueError(
+            raise LayoutError(
                 f"given target layout does not belong to the target document"
             )
         self.add_command(LoadEntities(list(block_layout), target_layout))
 
     def load_layers(self, names: Sequence[str]) -> None:
         """Loads the layers defined by the argument `names` into the target document.
         In the case of a name conflict the conflict policy will be applied.
@@ -938,25 +994,25 @@
             self.add_entity(entity, block_handle)
         self.add_entity(block_record.endblk, block_handle)  # type: ignore
 
     def add_handle(self, handle: Optional[str]) -> None:
         """Add resource by handle (table entry or object), cannot add graphic entities.
 
         Raises:
-            TypeError: cannot add graphic entity
+            EntityError: cannot add graphic entity
 
         """
         if handle is None or handle == "0":
             return
         entity = self.source_doc.entitydb.get(handle)
         if entity is None:
             self.debug(f"source entity #{handle} does not exist")
             return
         if is_graphic_entity(entity):
-            raise TypeError(f"cannot add graphic entity: {str(entity)}")
+            raise EntityError(f"cannot add graphic entity: {str(entity)}")
         self.add_entity(entity)
 
     def add_layer(self, name: str) -> None:
         if name == DEFAULT_LAYER:
             # Layer name "0" gets never mangled and always exist in the target document.
             return
         try:
@@ -1061,15 +1117,15 @@
         return None
 
     def map_resources_of_copy(self, entity: DXFEntity) -> None:
         clone = self.get_entity_copy(entity)
         if clone:
             entity.map_resources(clone, self)
         else:
-            raise const.DXFInternalEzdxfError(f"copy of {entity} not found")
+            raise InternalError(f"copy of {entity} not found")
 
     def map_pointers(self, tags: Tags, new_owner_handle: str = "") -> None:
         for index, tag in enumerate(tags):
             if types.is_translatable_pointer(tag):
                 handle = self.get_handle(tag.value, default="0")
                 tags[index] = types.DXFTag(tag.code, handle)
                 if new_owner_handle and types.is_hard_owner(tag):
@@ -1223,28 +1279,24 @@
 
     def map_entity_resources(self) -> None:
         source_db = self.registry.source_doc.entitydb
         for block_key, block in self.copied_blocks.items():
             for source_entity_handle, clone in block.items():
                 source_entity = source_db.get(source_entity_handle)
                 if source_entity is None:
-                    raise const.DXFInternalEzdxfError(
-                        "database error, source entity not found"
-                    )
+                    raise InternalError("database error, source entity not found")
                 if clone is not None and clone.is_alive:
                     source_entity.map_resources(clone, self)
 
     def map_object_resources(self) -> None:
         source_db = self.registry.source_doc.entitydb
         for source_object_handle, clone in self.copied_objects.items():
             source_entity = source_db.get(source_object_handle)
             if source_entity is None:
-                raise const.DXFInternalEzdxfError(
-                    "database error, source object not found"
-                )
+                raise InternalError("database error, source object not found")
             if clone is not None and clone.is_alive:
                 source_entity.map_resources(clone, self)
 
     def add_layer_entry(self, layer: Layer) -> None:
         tdoc = self.registry.target_doc
         layer_name = layer.dxf.name.upper()
 
@@ -1342,15 +1394,15 @@
                 name = block_record.dxf.name
                 msg = f"skipping non-graphic DXF entity in BLOCK_RECORD('{name}', #{handle}): {str(entity)}"
                 logging.warning(msg)  # this is a DXF structure error
                 self.debug(msg)
         if isinstance(block, Block) and isinstance(endblk, EndBlk):
             block_record.set_block(block, endblk)
         else:
-            raise const.DXFInternalEzdxfError("invalid BLOCK_RECORD copy")
+            raise InternalError("invalid BLOCK_RECORD copy")
 
     def add_ucs_entry(self, ucs: UCSTableEntry) -> None:
         # name mapping is not supported for UCS table entries
         tdoc = self.registry.target_doc
         self.add_table_entry(tdoc.ucs, ucs)
 
     def add_table_entry(self, table, entity: DXFEntity) -> None:
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/zoom.py` & `ezdxf-1.0.4b1/src/ezdxf/zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/_options.py` & `ezdxf-1.0.4b1/src/ezdxf/_options.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/__init__.py` & `ezdxf-1.0.4b1/src/ezdxf/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/__main__.py` & `ezdxf-1.0.4b1/src/ezdxf/__main__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/bezier3p.pyx` & `ezdxf-1.0.4b1/src/ezdxf/acc/bezier3p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/bezier4p.pyx` & `ezdxf-1.0.4b1/src/ezdxf/acc/bezier4p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/bspline.pyx` & `ezdxf-1.0.4b1/src/ezdxf/acc/bspline.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/construct.pyx` & `ezdxf-1.0.4b1/src/ezdxf/acc/construct.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/linetypes.pyx` & `ezdxf-1.0.4b1/src/ezdxf/acc/linetypes.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/mapbox_earcut.pyx` & `ezdxf-1.0.4b1/src/ezdxf/acc/mapbox_earcut.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/matrix44.pyx` & `ezdxf-1.0.4b1/src/ezdxf/acc/matrix44.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/vector.pxd` & `ezdxf-1.0.4b1/src/ezdxf/acc/vector.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/vector.pyx` & `ezdxf-1.0.4b1/src/ezdxf/acc/vector.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_cubic_bezier.cpp` & `ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_cubic_bezier.hpp` & `ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_quad_bezier.cpp` & `ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_vec3.hpp` & `ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_vec3.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/_cpp_vec3.pxd` & `ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_vec3.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acc/__init__.py` & `ezdxf-1.0.4b1/src/ezdxf/acc/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acis/abstract.py` & `ezdxf-1.0.4b1/src/ezdxf/acis/abstract.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acis/api.py` & `ezdxf-1.0.4b1/src/ezdxf/acis/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acis/const.py` & `ezdxf-1.0.4b1/src/ezdxf/acis/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acis/dbg.py` & `ezdxf-1.0.4b1/src/ezdxf/acis/dbg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acis/dxf.py` & `ezdxf-1.0.4b1/src/ezdxf/acis/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acis/entities.py` & `ezdxf-1.0.4b1/src/ezdxf/acis/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acis/hdr.py` & `ezdxf-1.0.4b1/src/ezdxf/acis/hdr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acis/mesh.py` & `ezdxf-1.0.4b1/src/ezdxf/acis/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acis/sab.py` & `ezdxf-1.0.4b1/src/ezdxf/acis/sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/acis/sat.py` & `ezdxf-1.0.4b1/src/ezdxf/acis/sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/acadctb.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/binpacking.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/binpacking.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/dimlines.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/dimlines.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/dxf2code.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/dxf2code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/genetic_algorithm.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/geo.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/gerber_D6673.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/gerber_D6673.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/importer.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/iterdxf.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/iterdxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/menger_sponge.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/meshex.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/mtextsurrogate.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/mtextsurrogate.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 class MTextSurrogate(SubscriptAttributes):
     """MTEXT surrogate for DXF R12 build up by TEXT Entities. This add-on was
     added to simplify the transition from :mod:`dxfwrite` to :mod:`ezdxf`.
 
     The rich-text formatting capabilities for the regular MTEXT entity are not
     supported, if these features are required use the regular MTEXT entity and
     the :class:`~ezdxf.addons.MTextExplode` add-on to explode the MTEXT entity
-    into simpler DXF primitives.
+    into DXF primitives.
 
     .. important::
 
         The align-point is always the insert-point, there is no need for
         a second align-point because the horizontal alignments FIT, ALIGN,
         BASELINE_MIDDLE are not supported.
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/mtxpl.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/mtxpl.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/odafc.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/odafc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright (c) 2020-2022, Manfred Moitzi
+# Copyright (c) 2020-2023, Manfred Moitzi
 # License: MIT License
 # type: ignore
 from __future__ import annotations
-from typing import Optional, Union
+from typing import Optional
 import logging
 import os
 import platform
 import shutil
 import subprocess
 import tempfile
 import time
@@ -104,15 +104,15 @@
 
 
 def map_version(version: str) -> str:
     return VERSION_MAP.get(version.upper(), version.upper())
 
 
 def readfile(
-    filename: str, version: Optional[str] = None, *, audit: bool = False
+    filename: str | os.PathLike, version: Optional[str] = None, *, audit: bool = False
 ) -> Optional[Drawing]:
     """Uses an installed `ODA File Converter`_ to convert a DWG/DXB/DXF file
     into a temporary DXF file and load this file by `ezdxf`.
 
     Args:
         filename: file to load by ODA File Converter
         version: load file as specific DXF version, by default the same version
@@ -149,15 +149,15 @@
             doc.filename = infile.with_suffix(".dxf")
             return doc
     raise UnknownODAFCError("Failed to convert file: Unknown Error")
 
 
 def export_dwg(
     doc: Drawing,
-    filename: str,
+    filename: str | os.PathLike,
     version: Optional[str] = None,
     *,
     audit: bool = False,
     replace: bool = False,
 ) -> None:
     """Uses an installed `ODA File Converter`_ to export the DXF document `doc`
     as a DWG file.
@@ -207,22 +207,20 @@
                 str(out_folder),
                 output_format="DWG",
                 version=export_version,
                 audit=audit,
             )
             _execute_odafc(arguments)
     else:
-        raise FileNotFoundError(
-            f"No such file or directory: '{str(out_folder)}'"
-        )
+        raise FileNotFoundError(f"No such file or directory: '{str(out_folder)}'")
 
 
 def convert(
-    source: Union[str, Path],
-    dest: Union[str, Path] = "",
+    source: str | os.PathLike,
+    dest: str | os.PathLike = "",
     *,
     version="R2018",
     audit=True,
     replace=False,
 ):
     """Convert `source` file to `dest` file.
 
@@ -269,17 +267,15 @@
         else:
             raise UnsupportedFileFormat(f"Unsupported file format: '{ext}'")
     if dest_path.exists() and not replace:
         raise FileExistsError(f"Target file already exists: '{dest_path}'")
     parent_dir = dest_path.parent
     if not parent_dir.exists() or not parent_dir.is_dir():
         # Cannot copy result to destination folder!
-        raise FileNotFoundError(
-            f"Destination folder does not exist: '{parent_dir}'"
-        )
+        raise FileNotFoundError(f"Destination folder does not exist: '{parent_dir}'")
     ext = dest_path.suffix
     fmt = ext.upper()[1:]
     if fmt not in ("DXF", "DWG"):
         raise UnsupportedFileFormat(f"Unsupported file format: '{ext}'")
 
     with tempfile.TemporaryDirectory(prefix="odafc_") as tmp_dir:
         arguments = _odafc_arguments(
@@ -408,17 +404,15 @@
         yield display
         try:
             proc.terminate()
             proc.wait()
         except OSError:
             pass
     else:
-        logger.warning(
-            f"Install xvfb to prevent the ODAFileConverter GUI from opening"
-        )
+        logger.warning(f"Install xvfb to prevent the ODAFileConverter GUI from opening")
         yield os.environ["DISPLAY"]
 
 
 def _run_with_no_gui(
     system: str, command: str, arguments: list[str]
 ) -> subprocess.Popen:
     """Execute ODAFC application without launching the GUI.
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/openscad.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/pycsg.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/r12export.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/r12writer.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/sierpinski_pyramid.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/sierpinski_pyramid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/tablepainter.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/tablepainter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/text2path.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/xqt.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/xqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/acisbrowser/browser.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/acisbrowser/data.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/browser/bookmarks.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/browser/bookmarks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/browser/browser.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/browser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/browser/data.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/browser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/browser/find_dialog.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/browser/find_dialog.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/browser/loader.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/browser/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/browser/model.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/browser/model.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/browser/tags.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/browser/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/browser/views.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/browser/views.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/backend.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/config.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/config.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/debug_backend.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/debug_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/frontend.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/frontend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/gfxproxy.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/gfxproxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/matplotlib.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/matplotlib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/mpl_text_renderer.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/mpl_text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/mtext_complex.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/mtext_complex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/pillow.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/pillow.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/properties.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/pyqt.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/pyqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/qtviewer.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/qtviewer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/qt_text_renderer.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/qt_text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/text.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/drawing/text_renderer.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/dwg/classes_section.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/dwg/classes_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/dwg/const.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/dwg/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/dwg/crc.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/dwg/crc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/dwg/fileheader.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/dwg/fileheader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/dwg/header_section.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/dwg/header_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/addons/dwg/loader.py` & `ezdxf-1.0.4b1/src/ezdxf/addons/dwg/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/acad_proxy_entity.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/acad_table.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/acis.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/appdata.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/appid.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/appid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/arc.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/attrib.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/block.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/blockrecord.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/blockrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/boundary_paths.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/circle.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/dictionary.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/dimension.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/dimstyle.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/dimstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/dimstyleoverride.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/dimstyleoverride.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/dxfclass.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/dxfentity.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/dxfgfx.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/dxfgroups.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/dxfns.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/dxfns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/dxfobj.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/ellipse.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/ellipse.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,30 +222,30 @@
         e.swap_axis()
         self.update_dxf_attribs(e.dxfattribs())
 
     @classmethod
     def from_arc(cls, entity: DXFGraphic) -> Ellipse:
         """Create a new virtual ELLIPSE entity from an ARC or a CIRCLE entity.
 
-        The new SPLINE entity has no owner, no handle, is not stored in
-        the entity database nor assigned to any layout!
+        The new entity has no owner, no handle, is not stored in the entity database nor
+        assigned to any layout!
 
         """
         assert entity.dxftype() in {"ARC", "CIRCLE"}, "ARC or CIRCLE entity required"
         attribs = entity.dxfattribs(drop={"owner", "handle", "thickness"})
         e = ellipse.ConstructionEllipse.from_arc(
             center=attribs.get("center", NULLVEC),
             extrusion=attribs.get("extrusion", Z_AXIS),
             # Remove all not ELLIPSE attributes:
             radius=attribs.pop("radius", 1.0),
             start_angle=attribs.pop("start_angle", 0),
             end_angle=attribs.pop("end_angle", 360),
         )
         attribs.update(e.dxfattribs())
-        return Ellipse.new(dxfattribs=attribs, doc=entity.doc)
+        return cls.new(dxfattribs=attribs, doc=entity.doc)
 
     def transform(self, m: Matrix44) -> Ellipse:
         """Transform the ELLIPSE entity by transformation matrix `m` inplace."""
         e = self.construction_tool()
         e.transform(m)
         self.update_dxf_attribs(e.dxfattribs())
         self.post_transform(m)
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/factory.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/geodata.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/geodata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/gradient.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/gradient.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/hatch.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/hatch.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/helix.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/idbuffer.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/idbuffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/image.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/image.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/insert.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/layer.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/layout.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/leader.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/light.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/line.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/ltype.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/lwpolyline.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/lwpolyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/material.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/mesh.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/mleader.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/mleader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) 2018-2022, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union, Optional, Iterable, Any, Iterator
 import copy
 import logging
+import math
 from collections import namedtuple
 
 from ezdxf.lldxf import const
 from ezdxf.lldxf.types import cast_value
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
@@ -26,15 +27,15 @@
     Matrix44,
     WCSTransform,
     OCSTransform,
     NonUniformScalingError,
 )
 from ezdxf import colors
 from ezdxf.proxygraphic import ProxyGraphicError
-from ezdxf.tools.text import safe_string
+from ezdxf.tools.text import safe_string, scale_mtext_inline_commands
 from ezdxf.tools.handle import safe_handle
 
 from .dxfentity import base_class, SubclassProcessor
 from .dxfobj import DXFObject
 from .dxfgfx import DXFGraphic, acdb_entity
 
 from .factory import register_entity
@@ -542,15 +543,17 @@
     def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, MultiLeader)
         super().map_resources(clone, mapping)
         dxf = self.dxf
         clone_dxf = clone.dxf
         clone_dxf.style_handle = mapping.get_handle(dxf.style_handle)
-        clone_dxf.leader_linetype_handle = mapping.get_handle(dxf.leader_linetype_handle)
+        clone_dxf.leader_linetype_handle = mapping.get_handle(
+            dxf.leader_linetype_handle
+        )
         clone_dxf.arrow_head_handle = mapping.get_handle(dxf.arrow_head_handle)
         clone_dxf.text_style_handle = mapping.get_handle(dxf.text_style_handle)
         clone_dxf.block_record_handle = mapping.get_handle(dxf.block_record_handle)
         clone.map_arrow_head_handles(mapping)
         clone.map_block_attrib_handles(mapping)
         clone.context.map_resources(mapping)
 
@@ -973,27 +976,37 @@
         self.insert = m.transform(self.insert)  # WCS
         self.text_direction = wcs.m.transform_direction(  # WCS
             self.text_direction, normalize=True
         )
         # don't use rotation ;)
         self.rotation = ocs.transform_angle(self.rotation)
         scale = wcs.uniform_scale
+        if math.isclose(scale, 1.0) or abs(scale) <= 1e-12:
+            return
         self.width *= scale
         self.defined_height *= scale
         self.column_width *= scale
         self.column_gutter_width *= scale
         self.column_sizes = [size * scale for size in self.column_sizes]
+        self.default_content = scale_mtext_inline_commands(
+            self.default_content, scale
+        )
 
     def apply_conversion_factor(self, conversion_factor: float):
         # conversion_factor: convert from an old scaling to a new scaling
+        if math.isclose(conversion_factor, 1.0) or abs(conversion_factor) <= 1e-12:
+            return
         self.width *= conversion_factor
         self.defined_height *= conversion_factor
         self.column_width *= conversion_factor
         self.column_gutter_width *= conversion_factor
         self.column_sizes = [h * conversion_factor for h in self.column_sizes]
+        self.default_content = scale_mtext_inline_commands(
+            self.default_content, conversion_factor
+        )
 
 
 class BlockData:
     ATTRIBS = {
         341: "block_record_handle",
         14: "extrusion",
         15: "insert",
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/mline.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/mpolygon.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/mtext.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/mtext.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from ezdxf.math.transformtools import transform_extrusion
 from ezdxf.colors import rgb2int, RGB
 from ezdxf.tools.text import (
     split_mtext_string,
     escape_dxf_line_endings,
     fast_plain_mtext,
     plain_mtext,
+    scale_mtext_inline_commands,
 )
 from . import factory
 from .dxfentity import base_class, SubclassProcessor
 from .dxfgfx import DXFGraphic, acdb_entity
 from .xdata import XData
 
 if TYPE_CHECKING:
@@ -1027,18 +1028,27 @@
         new_extrusion, _ = transform_extrusion(old_extrusion, m)
         self.convert_rotation_to_text_direction()
 
         old_text_direction = Vec3(dxf.text_direction)
         new_text_direction = m.transform_direction(old_text_direction)
 
         old_vertical_direction = old_extrusion.cross(old_text_direction)
-        old_char_height_vec = old_vertical_direction.normalize(dxf.char_height)
+        old_char_height = float(dxf.char_height)
+        old_char_height_vec = old_vertical_direction.normalize(old_char_height)
         new_char_height_vec = m.transform_direction(old_char_height_vec)
         oblique = new_text_direction.angle_between(new_char_height_vec)
-        dxf.char_height = new_char_height_vec.magnitude * math.sin(oblique)
+        new_char_height = new_char_height_vec.magnitude * math.sin(oblique)
+        dxf.char_height = new_char_height
+        if (
+            not math.isclose(old_char_height, new_char_height)
+            and abs(old_char_height) > 1e-12
+        ):
+            factor = new_char_height / old_char_height
+            # Column content is transformed by the sub-entities itself!
+            self.text = scale_mtext_inline_commands(self.text, factor)
 
         if dxf.hasattr("width"):
             width_vec = old_text_direction.normalize(dxf.width)
             dxf.width = m.transform_direction(width_vec).magnitude
 
         dxf.insert = m.transform(dxf.insert)
         dxf.text_direction = new_text_direction
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/mtext_columns.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/objectcollection.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/objectcollection.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,14 +30,22 @@
     return name
 
 
 T = TypeVar("T", bound="DXFObject")
 
 
 class ObjectCollection(Generic[T]):
+    """
+    Note:
+    ObjectCollections may contain entries where the name stored in the entity as
+    "name" attribute diverges from the key in the DICTIONARY object e.g. MLEADERSTYLE
+    collection may have entries for "Standard" and "Annotative" but both MLEADERSTYLE
+    objects have the name "Standard".
+
+    """
     def __init__(
         self,
         doc: Drawing,
         dict_name: str = "ACAD_MATERIAL",
         object_type: str = "MATERIAL",
     ):
         self.doc: Drawing = doc
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/oleframe.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/oleframe.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/pattern.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/point.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/polygon.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/polygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/polyline.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/shape.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/solid.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/spline.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/subentity.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/subentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/sun.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/table.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/text.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/textstyle.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/textstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/tolerance.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/ucs.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/underlay.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/view.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/view.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/viewport.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/visualstyle.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/visualstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/vport.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/vport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/xdata.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/xdict.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/xdict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/xline.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/entities/__init__.py` & `ezdxf-1.0.4b1/src/ezdxf/entities/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/layouts/base.py` & `ezdxf-1.0.4b1/src/ezdxf/layouts/base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/layouts/blocklayout.py` & `ezdxf-1.0.4b1/src/ezdxf/layouts/blocklayout.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) 2019-2021, Manfred Moitzi
 # License: MIT License
 from typing import Iterable, Optional
-from ezdxf.math import Vec3
+from ezdxf.math import Vec3, UVec
 from ezdxf.lldxf import const
 from .base import BaseLayout
 from ezdxf.entities import DXFGraphic, AttDef, Block, EndBlk
 
 
 class BlockLayout(BaseLayout):
     """BlockLayout has the same factory-functions as Layout, but is managed
@@ -70,17 +70,21 @@
 
     @scale_uniformly.setter
     def scale_uniformly(self, value: bool):
         self.block_record.dxf.scale = int(value)
 
     @property
     def base_point(self) -> Vec3:
-        """Returns the base point of the block."""
+        """Get/Set the base point of the block."""
         return Vec3(self.block.dxf.base_point)  # type: ignore
 
+    @base_point.setter
+    def base_point(self, value: UVec) -> None:
+        self.block.dxf.base_point = Vec3(value)  # type: ignore
+
     def attdefs(self) -> Iterable[AttDef]:
         """Returns iterable of all :class:`~ezdxf.entities.attrib.Attdef`
         entities.
         """
         return (e for e in self if isinstance(e, AttDef))
 
     def has_attdef(self, tag: str) -> bool:
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/layouts/layout.py` & `ezdxf-1.0.4b1/src/ezdxf/layouts/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/layouts/layouts.py` & `ezdxf-1.0.4b1/src/ezdxf/layouts/layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/attributes.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/const.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/encoding.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/extendedtags.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/extendedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/fileindex.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/fileindex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/hdrvars.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/hdrvars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/loader.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/packedtags.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/packedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/repair.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/repair.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/tagger.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/tagger.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/tags.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/tagwriter.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/tagwriter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/types.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/lldxf/validator.py` & `ezdxf-1.0.4b1/src/ezdxf/lldxf/validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/arc.py` & `ezdxf-1.0.4b1/src/ezdxf/math/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/bbox.py` & `ezdxf-1.0.4b1/src/ezdxf/math/bbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2022, Manfred Moitzi
+# Copyright (c) 2019-2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import Iterable, Optional, Iterator, Sequence
 import abc
 
 from ezdxf.math import Vec3, Vec2, UVec, AnyVec
 
@@ -129,15 +129,15 @@
         v = list(vertices)
         if not v:
             return
         if self.has_data:
             v.extend([self.extmin, self.extmax])
         self.extmin, self.extmax = self.extends_detector(v)
 
-    def union(self, other: "AbstractBoundingBox"):
+    def union(self, other: AbstractBoundingBox):
         """Returns a new bounding box as union of this and `other` bounding
         box.
         """
         vertices: list[AnyVec] = []
         if self.has_data:
             vertices.extend(self)
         if other.has_data:
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/bezier.py` & `ezdxf-1.0.4b1/src/ezdxf/math/bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/bezier_interpolation.py` & `ezdxf-1.0.4b1/src/ezdxf/math/bezier_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/box.py` & `ezdxf-1.0.4b1/src/ezdxf/math/box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/bspline.py` & `ezdxf-1.0.4b1/src/ezdxf/math/bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/bulge.py` & `ezdxf-1.0.4b1/src/ezdxf/math/bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/circle.py` & `ezdxf-1.0.4b1/src/ezdxf/math/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/clipping.py` & `ezdxf-1.0.4b1/src/ezdxf/math/clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/clustering.py` & `ezdxf-1.0.4b1/src/ezdxf/math/clustering.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/construct2d.py` & `ezdxf-1.0.4b1/src/ezdxf/math/construct2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# Copyright (c) 2011-2022, Manfred Moitzi
+# Copyright (c) 2011-2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
-from typing import Iterable, Sequence
+from typing import Iterable, Sequence, Iterator
 
 from functools import partial
 import math
 from ezdxf.math import (
     Vec3,
     Vec2,
     UVec,
@@ -41,15 +41,15 @@
     "decdeg2dms",
     "ellipse_param_span",
 ]
 
 
 def linspace(
     start: float, stop: float, num: int, endpoint=True
-) -> Iterable[float]:
+) -> Iterator[float]:
     """Return evenly spaced numbers over a specified interval, like
     numpy.linspace().
 
     Returns `num` evenly spaced samples, calculated over the interval
     [start, stop]. The endpoint of the interval can optionally be excluded.
 
     """
@@ -94,15 +94,15 @@
 
     Alias to function: :func:`ezdxf.math.arc_angle_span_rad`
 
     """
     return arc_angle_span_rad(float(start_param), float(end_param))
 
 
-def closest_point(base: UVec, points: Iterable[UVec]) -> "Vec3":
+def closest_point(base: UVec, points: Iterable[UVec]) -> Vec3:
     """Returns the closest point to a give `base` point.
 
     Args:
         base: base point as :class:`Vec3` compatible object
         points: iterable of points as :class:`Vec3` compatible object
 
     """
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/construct3d.py` & `ezdxf-1.0.4b1/src/ezdxf/math/construct3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/cspline.py` & `ezdxf-1.0.4b1/src/ezdxf/math/cspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/curvetools.py` & `ezdxf-1.0.4b1/src/ezdxf/math/curvetools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/ellipse.py` & `ezdxf-1.0.4b1/src/ezdxf/math/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/eulerspiral.py` & `ezdxf-1.0.4b1/src/ezdxf/math/eulerspiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/linalg.py` & `ezdxf-1.0.4b1/src/ezdxf/math/linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/line.py` & `ezdxf-1.0.4b1/src/ezdxf/math/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/offset2d.py` & `ezdxf-1.0.4b1/src/ezdxf/math/offset2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/parametrize.py` & `ezdxf-1.0.4b1/src/ezdxf/math/parametrize.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/perlin.py` & `ezdxf-1.0.4b1/src/ezdxf/math/perlin.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/polyline.py` & `ezdxf-1.0.4b1/src/ezdxf/math/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/rtree.py` & `ezdxf-1.0.4b1/src/ezdxf/math/rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/shape.py` & `ezdxf-1.0.4b1/src/ezdxf/math/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/surfaces.py` & `ezdxf-1.0.4b1/src/ezdxf/math/surfaces.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/transformtools.py` & `ezdxf-1.0.4b1/src/ezdxf/math/transformtools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/triangulation.py` & `ezdxf-1.0.4b1/src/ezdxf/math/triangulation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/ucs.py` & `ezdxf-1.0.4b1/src/ezdxf/math/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/_bezier3p.py` & `ezdxf-1.0.4b1/src/ezdxf/math/_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/_bezier4p.py` & `ezdxf-1.0.4b1/src/ezdxf/math/_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/_bspline.py` & `ezdxf-1.0.4b1/src/ezdxf/math/_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/_construct.py` & `ezdxf-1.0.4b1/src/ezdxf/math/_construct.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/_ctypes.py` & `ezdxf-1.0.4b1/src/ezdxf/math/_ctypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/_mapbox_earcut.py` & `ezdxf-1.0.4b1/src/ezdxf/math/_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/_matrix44.py` & `ezdxf-1.0.4b1/src/ezdxf/math/_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/_vector.py` & `ezdxf-1.0.4b1/src/ezdxf/math/_vector.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/math/__init__.py` & `ezdxf-1.0.4b1/src/ezdxf/math/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/path/commands.py` & `ezdxf-1.0.4b1/src/ezdxf/path/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/path/converter.py` & `ezdxf-1.0.4b1/src/ezdxf/path/converter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/path/nesting.py` & `ezdxf-1.0.4b1/src/ezdxf/path/nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/path/path.py` & `ezdxf-1.0.4b1/src/ezdxf/path/path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/path/shapes.py` & `ezdxf-1.0.4b1/src/ezdxf/path/shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/path/tools.py` & `ezdxf-1.0.4b1/src/ezdxf/path/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -651,14 +651,19 @@
 
     def bulge_to(p1: Vec3, p2: Vec3, bulge: float, segments: int):
         if p1.isclose(p2, rel_tol=IS_CLOSE_TOL, abs_tol=0):
             return
         # each cubic_bezier adds 3 segments, need 1 minimum
         num_bez = math.ceil(segments / 3)
         center, start_angle, end_angle, radius = bulge_to_arc(p1, p2, bulge)
+        # normalize angles into range 0 .. 2pi
+        start_angle = start_angle % math.tau
+        end_angle = end_angle % math.tau
+        if start_angle > end_angle:
+            end_angle += math.tau
         angles = list(linspace(start_angle, end_angle, num_bez + 1))
         curves = []
         for i in range(num_bez):
             ellipse = ConstructionEllipse.from_arc(
                 center,
                 radius,
                 Z_AXIS,
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/pp/dxfpp.css` & `ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/pp/dxfpp.html` & `ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.html`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/pp/dxfpp.js` & `ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.js`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/pp/dxfpp.py` & `ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/pp/pprint.py` & `ezdxf-1.0.4b1/src/ezdxf/pp/pprint.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/pp/rawpp.css` & `ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/pp/rawpp.py` & `ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/pp/reflinks.py` & `ezdxf-1.0.4b1/src/ezdxf/pp/reflinks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/abstract_mtext_renderer.py` & `ezdxf-1.0.4b1/src/ezdxf/render/abstract_mtext_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/arrows.py` & `ezdxf-1.0.4b1/src/ezdxf/render/arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/curves.py` & `ezdxf-1.0.4b1/src/ezdxf/render/curves.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/dimension.py` & `ezdxf-1.0.4b1/src/ezdxf/render/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/dim_base.py` & `ezdxf-1.0.4b1/src/ezdxf/render/dim_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/dim_curved.py` & `ezdxf-1.0.4b1/src/ezdxf/render/dim_curved.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/dim_diameter.py` & `ezdxf-1.0.4b1/src/ezdxf/render/dim_diameter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/dim_linear.py` & `ezdxf-1.0.4b1/src/ezdxf/render/dim_linear.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/dim_ordinate.py` & `ezdxf-1.0.4b1/src/ezdxf/render/dim_ordinate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/dim_radius.py` & `ezdxf-1.0.4b1/src/ezdxf/render/dim_radius.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/forms.py` & `ezdxf-1.0.4b1/src/ezdxf/render/forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/hatching.py` & `ezdxf-1.0.4b1/src/ezdxf/render/hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/leader.py` & `ezdxf-1.0.4b1/src/ezdxf/render/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/linetypes.py` & `ezdxf-1.0.4b1/src/ezdxf/render/linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/mesh.py` & `ezdxf-1.0.4b1/src/ezdxf/render/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/mleader.py` & `ezdxf-1.0.4b1/src/ezdxf/render/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/mline.py` & `ezdxf-1.0.4b1/src/ezdxf/render/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/point.py` & `ezdxf-1.0.4b1/src/ezdxf/render/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/polyline.py` & `ezdxf-1.0.4b1/src/ezdxf/render/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/r12spline.py` & `ezdxf-1.0.4b1/src/ezdxf/render/r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/trace.py` & `ezdxf-1.0.4b1/src/ezdxf/render/trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/_linetypes.py` & `ezdxf-1.0.4b1/src/ezdxf/render/_linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/render/__init__.py` & `ezdxf-1.0.4b1/src/ezdxf/render/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/16x16.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/16x16.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/24x24.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/24x24.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/256x256.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/256x256.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/32x32.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/32x32.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/48x48.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/48x48.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/64x64.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/64x64.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/icon-copy-64px.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/icon-copy-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/icon-find-64px.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/icon-find-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/icon-goto-bookmark-64px.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/icon-goto-handle-64px.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-handle-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/icon-goto-line-64px.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-line-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/icon-left-arrow-64px.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/icon-left-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/icon-next-entity-64px.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/icon-next-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/icon-prev-entity-64px.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/icon-prev-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/icon-right-arrow-64px.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/icon-right-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/icon-show-in-tree-64px.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/icon-show-in-tree-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/resources/icon-store-bookmark-64px.png` & `ezdxf-1.0.4b1/src/ezdxf/resources/icon-store-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/sections/acdsdata.py` & `ezdxf-1.0.4b1/src/ezdxf/sections/acdsdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/sections/blocks.py` & `ezdxf-1.0.4b1/src/ezdxf/sections/blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/sections/classes.py` & `ezdxf-1.0.4b1/src/ezdxf/sections/classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/sections/entities.py` & `ezdxf-1.0.4b1/src/ezdxf/sections/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/sections/header.py` & `ezdxf-1.0.4b1/src/ezdxf/sections/header.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/sections/headervars.py` & `ezdxf-1.0.4b1/src/ezdxf/sections/headervars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/sections/objects.py` & `ezdxf-1.0.4b1/src/ezdxf/sections/objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/sections/table.py` & `ezdxf-1.0.4b1/src/ezdxf/sections/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/sections/tables.py` & `ezdxf-1.0.4b1/src/ezdxf/sections/tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/analyze.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/analyze.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/binarydata.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/binarydata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/codepage.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/codepage.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/complex_ltype.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/complex_ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/crypt.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/debug.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/debug.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/difftags.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/fonts.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/fonts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/font_face_cache.json` & `ezdxf-1.0.4b1/src/ezdxf/tools/font_face_cache.json`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/font_measurement_cache.json` & `ezdxf-1.0.4b1/src/ezdxf/tools/font_measurement_cache.json`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/handle.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/indexing.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/juliandate.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/pattern.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/rawloader.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/rawloader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/standards.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/standards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/strip.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/strip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/test.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/test.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/text.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 # License: MIT License
 """
 Tools in this module should be as independent of DXF entities as possible!
 """
 from __future__ import annotations
 from typing import (
     Iterable,
+    Iterator,
     TYPE_CHECKING,
     Union,
     Optional,
     Callable,
     NamedTuple,
+    Any,
 )
 import enum
 import re
 import math
 
 from ezdxf.lldxf import validator, const
 from ezdxf.enums import (
@@ -58,17 +60,15 @@
 
     def __init__(self, text: str, font: "AbstractFont"):
         self._font = font
         self._text_width: float = font.text_width(text)
         self._stretch_x: float = 1.0
         self._stretch_y: float = 1.0
 
-    def stretch(
-        self, alignment: TextEntityAlignment, p1: Vec3, p2: Vec3
-    ) -> None:
+    def stretch(self, alignment: TextEntityAlignment, p1: Vec3, p2: Vec3) -> None:
         """Set stretch factors for FIT and ALIGNED alignments to fit the
         text between `p1` and `p2`, only the distance between these points is
         important. Other given `alignment` values are ignore.
 
         """
         assert isinstance(alignment, TextEntityAlignment)
         sx: float = 1.0
@@ -116,15 +116,15 @@
         """
         fm = self.font_measurements()
         vertices = [
             Vec2(0, fm.baseline),
             Vec2(self.width, fm.baseline),
         ]
         shift = self._shift_vector(halign, valign, fm)
-        # Oblique angle is deliberately not supported, the base line should be
+        # Oblique angle is deliberately not supported, the baseline should be
         # (near) the y-coordinate=0.
         return TextLine.transform_2d(vertices, insert, shift, angle, scale)
 
     def corner_vertices(
         self,
         insert: UVec,
         halign: int = 0,
@@ -149,17 +149,15 @@
         vertices = [
             Vec2(0, fm.bottom),
             Vec2(self.width, fm.bottom),
             Vec2(self.width, fm.cap_top),
             Vec2(0, fm.cap_top),
         ]
         shift = self._shift_vector(halign, valign, fm)
-        return TextLine.transform_2d(
-            vertices, insert, shift, angle, scale, oblique
-        )
+        return TextLine.transform_2d(vertices, insert, shift, angle, scale, oblique)
 
     def _shift_vector(
         self, halign: int, valign: int, fm: FontMeasurements
     ) -> tuple[float, float]:
         return _shift_x(self.width, halign), _shift_y(fm, valign)
 
     @staticmethod
@@ -189,15 +187,15 @@
         # Operating in 2D is faster than building a full 3D transformation
         # matrix and a pure 2D transformation matrix is not implemented!
         # This function doesn't transform many vertices at the same time,
         # mostly only 4 vertices, therefore the matrix multiplication overhead
         # does not pay off.
         # The most expensive rotation transformation is the least frequently
         # used transformation.
-        # IMPORTANT: this assumptions are not verified by profiling!
+        # IMPORTANT: these assumptions are not verified by profiling!
 
         # Use 2D vectors:
         vertices_: Iterable[Vec2] = Vec2.generate(vertices)
 
         # 1. slanting at the original location (very rare):
         if oblique:
             slant_x = math.tan(oblique)
@@ -258,24 +256,20 @@
         halign = entity.dxf.halign
         valign = entity.dxf.valign
         if halign in (TextHAlign.ALIGNED, TextHAlign.FIT):
             # For the alignments ALIGNED and FIT the text stretching has to be
             # handles separately.
             halign = CENTER
             valign = BASELINE
-        elif (
-            halign == TextHAlign.MIDDLE
-        ):  # MIDDLE is different to MIDDLE/CENTER
+        elif halign == TextHAlign.MIDDLE:  # MIDDLE is different to MIDDLE/CENTER
             halign = CENTER
             valign = X_MIDDLE
         return halign, valign
     elif dxftype == "MTEXT":
-        return MAP_MTEXT_ALIGN_TO_FLAGS.get(
-            entity.dxf.attachment_point, (LEFT, TOP)
-        )
+        return MAP_MTEXT_ALIGN_TO_FLAGS.get(entity.dxf.attachment_point, (LEFT, TOP))
     else:
         raise TypeError(f"invalid DXF {dxftype}")
 
 
 def plain_text(text: str) -> str:
     """Returns the plain text for :class:`~ezdxf.entities.Text`,
     :class:`~ezdxf.entities.Attrib` and :class:`~ezdxf.entities.Attdef` content.
@@ -349,16 +343,16 @@
 # \pi-2,l2; = first line -2 & paragraph left 2
 # \pi0,l2;  = first line  0 & paragraph left 2
 #
 # \X	Paragraph wrap on the dimension line (only in dimensions)
 # \Q	Slanting (oblique) text by angle - e.g. \Q30;
 # \H	Text height relative - e.g. \H3x;
 # \H	Text height absolute - e.g. \H3;
-# \W	Text width factor - e.g. \W0.8x;
-# \W	Text width absolute - e.g. \W0.8;
+# \W	Text width factor relative e.g. \W0.8x;
+# \W	Text width factor absolute e.g. \W0.8;
 # \F	Font selection
 # \f	Font selection
 #
 #     e.g. \Fgdt;o - GDT-tolerance
 #     e.g. \fArial|b0|i0|c238|p10; - font Arial, non-bold, non-italic,
 #     codepage 238, pitch 10
 #     codepage 0 = no change
@@ -396,25 +390,25 @@
 #     \c65280; = GREEN (0, 255, 0)
 #     \c16711680; = BLUE (0, 0, 255)
 
 #     RGB color = \c7528479;  = 31,224,114
 #     ezdxf.rgb2int((31,224,114)) = 2089074 (r,g,b) wrong!
 #     ezdxf.rgb2int((114,224,31)) = 7528479 (b,g,r) reversed order is correct!
 #
-# \T	Tracking, char.spacing absolute - e.g. \T2;
-# \T	Tracking, char.spacing relative - e.g. \T2x;
+# \T	Tracking, char spacing factor as absolute value e.g. \T2;
+# \T	Tracking, char spacing factor as relative value e.g. \T2x;
 # {}	Braces - define the text area influenced by the code
 #       Multiple codes after the opening brace are valid until the closing
 #       brace.  e.g. {\H0.4x;\A1;small centered text}
 #
 # Codes and braces can be nested up to 8 levels deep
 #
 # Column types in BricsCAD:
 #   - dynamic auto height: all columns have the same height
-#   - dynamic manual height: each columns has an individual height
+#   - dynamic manual height: each column has an individual height
 #   - no columns
 #   - static: all columns have the same height, like dynamic auto height,
 #     difference is only important for user interaction in CAD applications
 #
 # - All columns have the same width and gutter.
 # - Paragraphs do overflow into the next column if required.
 
@@ -619,15 +613,15 @@
         get_text_width: callable which returns the width of the given string
 
     """
     # Copyright (c) 2020-2021, Matthew Broadway
     # License: MIT License
     if not text or text.isspace():
         return []
-    manual_lines = re.split(r"(\n)", text)  # includes \n as it's own token
+    manual_lines = re.split(r"(\n)", text)  # includes \n as its own token
     tokens = [t for line in manual_lines for t in re.split(r"(\s+)", line) if t]
     lines: list[str] = []
     current_line: str = ""
     line_just_wrapped = False
 
     for t in tokens:
         on_first_line = not lines
@@ -637,18 +631,15 @@
         if t == "\n":
             lines.append(current_line.rstrip())
             current_line = ""
         elif t.isspace():
             if current_line or on_first_line:
                 current_line += t
         else:
-            if (
-                box_width is not None
-                and get_text_width(current_line + t) > box_width
-            ):
+            if box_width is not None and get_text_width(current_line + t) > box_width:
                 if not current_line:
                     current_line += t
                 else:
                     lines.append(current_line.rstrip())
                     current_line = t
                     line_just_wrapped = True
             else:
@@ -660,17 +651,15 @@
 
 
 def is_text_vertical_stacked(text: DXFEntity) -> bool:
     """Returns ``True`` if the associated text :class:`~ezdxf.entities.Textstyle`
     is vertical stacked.
     """
     if not text.is_supported_dxf_attrib("style"):
-        raise TypeError(
-            f"{text.dxftype()} does not support the style attribute."
-        )
+        raise TypeError(f"{text.dxftype()} does not support the style attribute.")
 
     if text.doc:
         style = text.doc.styles.get(text.dxf.style)
         if style:
             return style.is_vertical_stacked  # type: ignore
     return False
 
@@ -810,15 +799,15 @@
     STRIKE_START = r"\K"
     STRIKE_STOP = r"\k"
     GROUP_START = "{"
     GROUP_END = "}"
     ALIGN_BOTTOM = r"\A0;"
     ALIGN_MIDDLE = r"\A1;"
     ALIGN_TOP = r"\A2;"
-    NBSP = r"\~"  # non breaking space
+    NBSP = r"\~"  # non-breaking space
     TAB = "^I"
 
     def append(self, text: str) -> MTextEditor:
         """Append `text`."""
         self.text += text
         return self
 
@@ -837,17 +826,15 @@
         """Returns the MTEXT content attribute :attr:`text`."""
         return self.text
 
     def clear(self):
         """Reset the content to an empty string."""
         self.text = ""
 
-    def font(
-        self, name: str, bold: bool = False, italic: bool = False
-    ) -> MTextEditor:
+    def font(self, name: str, bold: bool = False, italic: bool = False) -> MTextEditor:
         """Set the text font by the font family name. Changing the font height
         should be done by the :meth:`height` or the :meth:`scale_height` method.
         The font family name is the name shown in font selection widgets in
         desktop applications: "Arial", "Times New Roman", "Comic Sans MS".
         Switching the codepage is not supported.
 
         Args:
@@ -856,15 +843,15 @@
             italic: flag
 
         """
         # c0 = current codepage
         # The current implementation of ezdxf writes everything in one
         # encoding, defined by $DWGCODEPAGE < DXF R2007 or utf8 for DXF R2007+
         # Switching codepage makes no sense!
-        # p0 = current text size
+        # p0 = current text size;
         # Text size should be changed by \H<factor>x;
         return self.append(rf"\f{name}|b{int(bold)}|i{int(italic)};")
 
     def scale_height(self, factor: float) -> MTextEditor:
         """Scale the text height by a `factor`. This scaling will accumulate,
         which means starting at height 2.5 and scaling by 2 and again by 3 will
         set the text height to 2.5 x 2 x 3 = 15. The current text height is not
@@ -999,37 +986,38 @@
                 indent=-indent * 0.75,  # like BricsCAD
                 left=indent,
                 tab_stops=(indent,),
             )
         )
         items.append(
             "".join(
-                b + self.TAB + c + self.NEW_PARAGRAPH
-                for b, c in zip(bullets, content)
+                b + self.TAB + c + self.NEW_PARAGRAPH for b, c in zip(bullets, content)
             )
         )
         return self.group(str(items))
 
 
+class UnknownCommand(Exception):
+    pass
+
+
 class MTextContext:
     """Internal class to store the MTEXT context state."""
 
     def __init__(self) -> None:
         self._stroke: int = 0
         self.continue_stroke: bool = False
         self._aci = 7  # used if rgb is None
         self.rgb: Optional[RGB] = None  # overrules aci
         self.align = MTextLineAlignment.BOTTOM
         self.font_face: FontFace = FontFace()  # is immutable
         self.cap_height: float = 1.0
         self.width_factor: float = 1.0
         self.char_tracking_factor: float = 1.0
-        self.oblique: float = (
-            0.0  # in degrees, where 0 is vertical (TEXT entity)
-        )
+        self.oblique: float = 0.0  # in degrees, where 0 is vertical (TEXT entity)
         self.paragraph = ParagraphProperties()
 
     def __copy__(self) -> MTextContext:
         p = MTextContext()
         p._stroke = self._stroke
         p.continue_stroke = self.continue_stroke
         p._aci = self._aci
@@ -1073,17 +1061,15 @@
     def aci(self, aci: int):
         if 0 <= aci <= 256:
             self._aci = aci
             self.rgb = None  # clear rgb
         else:
             raise ValueError("aci not in range[0,256]")
 
-    def _set_stroke_state(
-        self, stroke: MTextStroke, state: bool = True
-    ) -> None:
+    def _set_stroke_state(self, stroke: MTextStroke, state: bool = True) -> None:
         """Set/clear binary `stroke` flag in `self._stroke`.
 
         Args:
             stroke: set/clear stroke flag
             state: ``True`` for setting, ``False`` for clearing
 
         """
@@ -1198,25 +1184,32 @@
             raise IndexError(stop)
         return self._text[self._index : stop]
 
     def tail(self) -> str:
         """Returns the unprocessed part of the content."""
         return self._text[self._index :]
 
+    def index(self) -> int:
+        return self._index
+
+    def substr2(self, start: int, stop: int) -> str:
+        return self._text[start:stop]
+
 
 class TokenType(enum.IntEnum):
     NONE = 0
     WORD = 1  # data = str
-    STACK = 2  # data = upr: str, lwr:str, type:str
+    STACK = 2  # data = tuple[upr: str, lwr:str, type:str]
     SPACE = 3  # data = None
     NBSP = 4  # data = None
     TABULATOR = 5  # data = None
     NEW_PARAGRAPH = 6  # data = None
     NEW_COLUMN = 7  # data = None
     WRAP_AT_DIMLINE = 8  # data = None
+    PROPERTIES_CHANGED = 9  # data = full command string e.g. "\H150;"
 
 
 class MTextToken:
     __slots__ = ("type", "ctx", "data")
 
     def __init__(self, t: TokenType, ctx: MTextContext, data=None):
         self.type: TokenType = t
@@ -1243,38 +1236,44 @@
     the same way.
 
     The parser works as iterator and yields MTextToken objects.
 
     Args:
         content: MText content string
         ctx: initial MText context
+        yield_property_commands: yield commands that change properties or context,
+            default is ``False``
 
     """
 
-    __slots__ = ("ctx", "scanner", "_ctx_stack", "_continue_stroke")
-
-    def __init__(self, content: str, ctx: Optional[MTextContext] = None):
+    def __init__(
+        self,
+        content: str,
+        ctx: Optional[MTextContext] = None,
+        yield_property_commands=False,
+    ):
         if ctx is None:
             ctx = MTextContext()
         self.ctx = ctx
         self.scanner = TextScanner(caret_decode(content))
         self._ctx_stack: list[MTextContext] = []
         self._continue_stroke = False
+        self._yield_property_commands = bool(yield_property_commands)
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[MTextToken]:
         return self.parse()
 
     def push_ctx(self) -> None:
         self._ctx_stack.append(self.ctx)
 
     def pop_ctx(self) -> None:
         if self._ctx_stack:
             self.ctx = self._ctx_stack.pop()
 
-    def parse(self) -> Iterable[MTextToken]:
+    def parse(self) -> Iterator[MTextToken]:
         # localize method calls
         scanner = self.scanner
         consume = scanner.fast_consume
         peek = scanner.fast_peek
         followup_token: Optional[TokenType] = None
         space_token = TokenType.SPACE
         word_token = TokenType.WORD
@@ -1284,19 +1283,20 @@
             consume()
             if word:
                 followup_token = token
                 return word_token, word
             else:
                 return token, None
 
-        def next_token():
-            word = ""
+        def next_token() -> tuple[TokenType, Any]:
+            word: str = ""
             while scanner.has_data:
                 escape = False
                 letter = peek()
+                cmd_start_index = scanner.index()
                 if letter == "\\":
                     # known escape sequences: "\\", "\{", "\}"
                     if peek(1) in "\\{}":
                         escape = True
                         consume()  # leading backslash
                         letter = peek()
                     else:
@@ -1315,17 +1315,25 @@
                         if cmd == "X":
                             return TokenType.WRAP_AT_DIMLINE, None
                         if cmd == "S":
                             return self.parse_stacking()
                         if cmd:
                             try:
                                 self.parse_properties(cmd)
-                            except ValueError:
+                            except UnknownCommand:
                                 # print invalid escaped letters verbatim
                                 word += letter + cmd
+                            else:
+                                if self._yield_property_commands:
+                                    return (
+                                        TokenType.PROPERTIES_CHANGED,
+                                        scanner.substr2(
+                                            cmd_start_index, scanner.index()
+                                        ),
+                                    )
                         continue
 
                 # process control chars, caret decoding is already done!
                 if letter < " ":
                     if letter == "\t":
                         return word_and_token(word, TokenType.TABULATOR)
                     elif letter == "\n":  # LF
@@ -1374,15 +1382,15 @@
                 yield MTextToken(type_, self.ctx, data)
                 if followup_token:
                     yield MTextToken(followup_token, self.ctx, None)
                     followup_token = None
             else:
                 break
 
-    def parse_stacking(self) -> tuple:
+    def parse_stacking(self) -> tuple[TokenType, Any]:
         """Returns a tuple of strings: (numerator, denominator, type).
         The numerator and denominator is always a single and can contain spaces,
         which are not decoded as separate tokens. The type string is "^" for
         a limit style fraction without a line, "/" for a horizontal fraction
         and "#" for a diagonal fraction. If the expression does not contain
         any stacking type char, the type and denominator string are empty "".
 
@@ -1463,16 +1471,16 @@
             self.parse_oblique(new_ctx)
         elif cmd == "T":
             self.parse_char_tracking(new_ctx)
         elif cmd == "p":
             self.parse_paragraph_properties(new_ctx)
         elif cmd == "f" or cmd == "F":
             self.parse_font_properties(new_ctx)
-        else:  # unknown commands
-            raise ValueError("unknown command")
+        else:
+            raise UnknownCommand(f"unknown command: {cmd}")
         new_ctx.continue_stroke = self._continue_stroke
         self.ctx = new_ctx
 
     def parse_align(self, ctx: MTextContext):
         char = self.scanner.get()  # always consume next char
         if char in "012":
             ctx.align = MTextLineAlignment(int(char))
@@ -1546,16 +1554,16 @@
             start, end = match.span()
             result = tail[start:end]
             self.scanner.consume(end)
         return result
 
     def extract_expression(self, escape=False) -> str:
         """Returns the next expression from the current location until
-        the terminating ";". The terminating semi-colon is not included.
-        Skips escaped "\\;" semi-colons if `escape` is True.
+        the terminating ";". The terminating semicolon is not included.
+        Skips escaped "\\;" semicolons if `escape` is True.
 
         """
         stop = self.scanner.find(";", escape=escape)
         if stop < 0:  # ";" not found
             expr = self.scanner.tail()  # scan until end of content
         else:
             expr = self.scanner.substr(stop)  # exclude ";"
@@ -1596,17 +1604,15 @@
                 left = parse_float()
             elif cmd == "r":
                 right = parse_float()
             elif cmd == "x":
                 pass  # ignore
             elif cmd == "q":
                 adjustment = paragraph_scanner.get()
-                align = CHAR_TO_ALIGN.get(
-                    adjustment, MTextParagraphAlignment.DEFAULT
-                )
+                align = CHAR_TO_ALIGN.get(adjustment, MTextParagraphAlignment.DEFAULT)
                 skip_commas()
             elif cmd == "t":
                 tab_stops = []  # type: ignore
                 while paragraph_scanner.has_data:  # parse to end
                     type_ = paragraph_scanner.peek()
                     if type_ == "r" or type_ == "c":
                         paragraph_scanner.consume()
@@ -1802,7 +1808,43 @@
 def safe_string(s: Optional[str], max_len: int = MAX_STR_LEN) -> str:
     """Returns a string with line breaks ``\\n`` replaced by ``\\P`` and the
     length limited to `max_len`.
     """
     if isinstance(s, str):
         return escape_dxf_line_endings(s)[:max_len]
     return ""
+
+
+VALID_HEIGHT_CHARS = set("0123456789.")
+
+
+def scale_mtext_inline_commands(content: str, factor: float) -> str:
+    """Scale all inline commands which define an absolute value by a `factor`."""
+
+    def _scale_leading_number(substr: str, prefix: str) -> str:
+        index: int = 0
+        try:
+            while substr[index] in VALID_HEIGHT_CHARS:
+                index += 1
+            if substr[index] == "x":  # relative factor
+                return f"{prefix}{substr}"
+        except IndexError:  # end of string
+            pass
+        try:
+            new_size = float(substr[:index]) * factor
+            value = f"{new_size:.3g}"
+        except ValueError:
+            value = ""  # return a valid construct
+        return rf"{prefix}{value}{substr[index:]}"
+
+    # So far only the "\H<value>;" command will be scaled.
+    # Fast check if scaling is required:
+    if r"\H" not in content:
+        return content
+
+    factor = abs(factor)
+    old_parts = content.split(r"\H")
+    new_parts: list[str] = [old_parts[0]]
+    for part in old_parts[1:]:
+        new_parts.append(_scale_leading_number(part, r"\H"))
+
+    return "".join(new_parts)
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/text_layout.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/text_size.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/zipmanager.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/zipmanager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/_iso_pattern.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/_iso_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/_matplotlib_font_support.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/_matplotlib_font_support.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf/tools/__init__.py` & `ezdxf-1.0.4b1/src/ezdxf/tools/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/src/ezdxf.egg-info/PKG-INFO` & `ezdxf-1.0.4b1/src/ezdxf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.0.3b0
+Version: 1.0.4b1
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
@@ -92,14 +92,15 @@
 - `MTextExplode` add-on for exploding MTEXT entities into single-line TEXT entities
 - `text2path` add-on to convert text into outline paths
 - `geo` add-on to support the [`__geo_interface__`](https://gist.github.com/sgillies/2217756)
 - `meshex` for exchanging meshes with other tools as STL, OFF or OBJ files
 - `openscad` add-on, an interface to [OpenSCAD](https://openscad.org)
 - `odafc` add-on, an interface to the [ODA File Converter](https://www.opendesign.com/guestfiles/oda_file_converter) 
   to read and write DWG files
+- `hpgl2` add-on for converting HPGL/2 plot files to DXF, SVG and PDF
 
 A simple example:
 
 ```Python
 import ezdxf
 from ezdxf import colors
 from ezdxf.enums import TextEntityAlignment
@@ -209,31 +210,47 @@
 Feedback is greatly appreciated.
 
 Manfred
 
 News
 ====
 
-Version 1.0.3b0 - dev
+Version 1.0.4b1 - dev
 ---------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
+- NEW: added setter to `BlockLayout.base_point` property
+- BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
+- BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
+  scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
+- PREVIEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG,  
+  final release in v1.1
+- PREVIEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF, final release in v1.1
+- PREVIEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG, final release in v1.1
+- PREVIEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF, final release in v1.1
+
+Version 1.0.3 - 2023-03-26
+--------------------------
+
+- Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: [#833](https://github.com/mozman/ezdxf/issues/833)
   logging non-unique entity handles when loading a DXF document as warnings, auditing 
   the document may fix this issue
 - NEW: improved auditing & fixing capabilities
 - NEW: `DXFTagStorage.graphic_properties()` returns the graphical properties for unknown
   or unsupported DXF entities
 - NEW: `GfxAttribs.from_dict()`
 - BUGFIX: audit process preserves dimensional constraints
 - BUGFIX: MTextExplode add-on created invalid text style table entries
 - PREVIEW: `ezdxf.addons.r12export` module to export any DXF document as a simple R12 
   file, final release in v1.1
 - PREVIEW: `ezdxf.r12strict` module to make DXF R12 drawing 100% compatible to Autodesk 
   products, final release in v1.1
+- PREVIEW: `ezdxf.transform` module to apply transformations to multiple DXF entities 
+  in a convenient and safe way, final release in v1.1
 
 Version 1.0.2 - 2023-02-15
 --------------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: `Drawing.validate()` also prints report of resolved issues
 - NEW: copy and transform support for `PDFUNDERLAY`, `DWFUNDERLAY` and `DGNUNDERLAY`
```

## Comparing `ezdxf-1.0.3b0/src/ezdxf.egg-info/SOURCES.txt` & `ezdxf-1.0.4b1/src/ezdxf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 integration_tests/test_read_write_modern_entites.py
 integration_tests/test_recover.py
 integration_tests/test_redraw_order.py
 integration_tests/test_rotated_block_attributes.py
 integration_tests/test_surface_entities.py
 integration_tests/test_write_fixed_meta_data.py
 integration_tests/test_write_without_handles.py
+integration_tests/test_xref_detach.py
 integration_tests/data/AC1003_LINE_Example.dxf
 integration_tests/data/ASCII_R12.dxf
 integration_tests/data/Leica_Disto_S910.dxf
 integration_tests/data/MODEL.dxf
 integration_tests/data/POLI-ALL210_12.DXF
 integration_tests/data/R12_with_trash_beyond_EOF.dxf
 integration_tests/data/XRECORD_0.bin
@@ -108,14 +109,15 @@
 src/ezdxf/py.typed
 src/ezdxf/query.py
 src/ezdxf/queryparser.py
 src/ezdxf/r12strict.py
 src/ezdxf/recover.py
 src/ezdxf/reorder.py
 src/ezdxf/shapefile.py
+src/ezdxf/transform.py
 src/ezdxf/units.py
 src/ezdxf/upright.py
 src/ezdxf/urecord.py
 src/ezdxf/version.py
 src/ezdxf/xref.py
 src/ezdxf/zoom.py
 src/ezdxf.egg-info/PKG-INFO
@@ -213,14 +215,28 @@
 src/ezdxf/addons/dwg/__init__.py
 src/ezdxf/addons/dwg/classes_section.py
 src/ezdxf/addons/dwg/const.py
 src/ezdxf/addons/dwg/crc.py
 src/ezdxf/addons/dwg/fileheader.py
 src/ezdxf/addons/dwg/header_section.py
 src/ezdxf/addons/dwg/loader.py
+src/ezdxf/addons/hpgl2/__init__.py
+src/ezdxf/addons/hpgl2/api.py
+src/ezdxf/addons/hpgl2/backend.py
+src/ezdxf/addons/hpgl2/compiler.py
+src/ezdxf/addons/hpgl2/deps.py
+src/ezdxf/addons/hpgl2/dxf_backend.py
+src/ezdxf/addons/hpgl2/interpreter.py
+src/ezdxf/addons/hpgl2/page.py
+src/ezdxf/addons/hpgl2/pdf_backend.py
+src/ezdxf/addons/hpgl2/plotter.py
+src/ezdxf/addons/hpgl2/polygon_buffer.py
+src/ezdxf/addons/hpgl2/properties.py
+src/ezdxf/addons/hpgl2/svg_backend.py
+src/ezdxf/addons/hpgl2/tokenizer.py
 src/ezdxf/entities/__init__.py
 src/ezdxf/entities/acad_proxy_entity.py
 src/ezdxf/entities/acad_table.py
 src/ezdxf/entities/acis.py
 src/ezdxf/entities/appdata.py
 src/ezdxf/entities/appid.py
 src/ezdxf/entities/arc.py
@@ -649,14 +665,16 @@
 tests/test_05_tools/test_530_acis_sab.py
 tests/test_05_tools/test_531_acis_entities.py
 tests/test_05_tools/test_532_acis_mesh.py
 tests/test_05_tools/test_533_shapefiles.py
 tests/test_05_tools/test_534_dwg_info.py
 tests/test_05_tools/test_535_xref_basic.py
 tests/test_05_tools/test_536_xref_conflict.py
+tests/test_05_tools/test_537_transform.py
+tests/test_05_tools/test_538_scale_mtext_inline_commands.py
 tests/test_06_math/conftest.py
 tests/test_06_math/test_600_base.py
 tests/test_06_math/test_601_bulge.py
 tests/test_06_math/test_602_vec3.py
 tests/test_06_math/test_603_vec2.py
 tests/test_06_math/test_604_banded_matrix.py
 tests/test_06_math/test_604_linalg.py
@@ -745,14 +763,16 @@
 tests/test_08_addons/test_814_text2path.py
 tests/test_08_addons/test_815_dxf_browser.py
 tests/test_08_addons/test_816_bin_packing.py
 tests/test_08_addons/test_817_genetic_algorithm.py
 tests/test_08_addons/test_818_meshex.py
 tests/test_08_addons/test_819_menger_sponge.py
 tests/test_08_addons/test_820_openscad.py
+tests/test_08_addons/test_821_hpgl2.py
+tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
 tests/test_09_cython_acceleration/test_901_acc_vec2.py
 tests/test_09_cython_acceleration/test_902_acc_vec3.py
 tests/test_09_cython_acceleration/test_903_acc_matrix44.py
 tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
 tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
 tests/test_09_cython_acceleration/test_906_acc_bspline.py
 tests/test_10_issues/test_issue_414_bbox_calculation.py
```

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_018_handle.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_018_handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_040_tags.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_040_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py` & `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_102_appdata.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_102_appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_103_reactors.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_103_reactors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_104_extension_dict.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_104_extension_dict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_105_xdata.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_105_xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_110_dxfentity.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_110_dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_112b_dxfobj.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_112b_dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_113_dxfclass.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_113_dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_114_factory.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_114_factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_116_dictionary.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_116_dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_120_style_table_entry.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_120_style_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_123_view_table_entry.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_123_view_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_125_image_def.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_125_image_def.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_127_raster_variables.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_127_raster_variables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_128_pdf_definition.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_128_pdf_definition.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_129_xrecord.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_129_xrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_130_id_buffer.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_130_id_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_131_field_list.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_131_field_list.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_132_layer_filter.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_132_layer_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_133_sun.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_133_sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_134_material.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_134_material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_135_geo_data.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_135_geo_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_136_vba_project.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_136_vba_project.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_137_sortentstable.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_137_sortentstable.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_139_user_record.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_139_user_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_140_block_record.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_140_block_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py` & `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/conftest.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_200_line.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_200_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_201_point.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_201_point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_202_circle.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_202_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_203_arc.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_203_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_204_shape.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_204_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_205_solid.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_205_solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_206_text.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_206_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_207_attdef.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_207_attdef.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_208_attrib.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_208_attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_209_vertex.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_209_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_210_polyline_1.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_210_polyline_2.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_211_viewport.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_211_viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_212_insert.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_212_insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_213_minsert.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_213_minsert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_214_block.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_214_block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_215_dimension.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_215_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_221_ellipse.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_221_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_222_xline.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_222_xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_223_ray.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_223_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_224_group.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_224_group.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_225_mtext.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_225_mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_226_spline.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_226_spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_228_mesh.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_228_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_231_underlay.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_231_underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_231_underlay_2.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_231_underlay_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_232_acis.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_232_acis_2.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_acis_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_232_surface.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_surface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_233_helix.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_233_helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_234_light.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_234_light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_235_leader.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_235_leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_236_multileader.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_236_multileader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_237_mline.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_237_mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_238_tolerance.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_238_tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_241_hyperlink.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_241_hyperlink.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_242_random_transform.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_242_random_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_243_replace_entity.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_243_replace_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_245_wipeout.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_245_wipeout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_246_spline_audit.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_246_spline_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_248_mpolygon.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_248_mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_251_upright.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_251_upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_253_ole2frame.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_253_ole2frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_02_dxf_graphics/test_254_get_font_name.py` & `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_254_get_font_name.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_300_layout.py` & `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_300_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py` & `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_302_block_references.py` & `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_302_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py` & `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py` & `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py` & `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py` & `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_307_groupby.py` & `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_307_groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_308_query.py` & `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_308_query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_309_query_parser.py` & `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_309_query_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py` & `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py` & `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_03_dxf_layouts/test_313_redraw_order.py` & `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_313_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_405_classes.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_405_classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_410_table.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_410_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_424_audit.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_424_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py` & `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/conftest.py` & `ezdxf-1.0.4b1/tests/test_05_tools/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_500_units.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_500_units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_501_truecolor.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_501_truecolor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_502_raw_color.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_502_raw_color.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_503_indexing.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_503_indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_504_suppress_zeros.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_504_suppress_zeros.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_507_dxf_pretty_printer.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_507_dxf_pretty_printer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_508_read_zip.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_508_read_zip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_509_comments.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_509_comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_510_byte_stream.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_510_byte_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_511_bit_stream.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_511_bit_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_512_pattern.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_512_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_513_reorder_entities.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_513_reorder_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_514_text.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_514_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_515_fonts.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_515_fonts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_516_zoom.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_516_zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_517_text_layout.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_517_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_519_mtext_editor.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_519_mtext_editor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_520_mtext_context.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_520_mtext_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_521_mtext_parser.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_521_mtext_parser.py`

 * *Files 15% similar despite different names*

```diff
@@ -677,27 +677,71 @@
             2,
             3,
             MTextParagraphAlignment.CENTER,
             (1, 2, 3),
         )
 
     def test_reset_arguments(self):
-        t0, t1 = list(
-            MTextParser(r"\pi1,l2,r3,qc,t1,2,3;word\pi*,l*,r*,q*,t;word")
-        )
+        t0, t1 = list(MTextParser(r"\pi1,l2,r3,qc,t1,2,3;word\pi*,l*,r*,q*,t;word"))
         assert t0.ctx.paragraph == (
             1,
             2,
             3,
             MTextParagraphAlignment.CENTER,
             (1, 2, 3),
         )
         assert t1.ctx.paragraph == ParagraphProperties()  # reset to default
 
     def test_invalid_tab_stops(self):
         tokens = list(MTextParser(r"\pi0,l0,tz;A"))
         t = tokens[0]
         assert t.ctx.paragraph.tab_stops == tuple()
 
+    def test_unknown_escape_sequence(self):
+        t0, t1 = list(MTextParser(r"word\Yword"))
+        assert t1.type == TokenType.WORD
+        assert t1.data == r"\Yword"
+
+
+class TestMTextParserYieldsPropertyChangeCommands:
+    def test_change_height(self):
+        t0, t1, t2 = list(MTextParser(r"word\H150;word", yield_property_commands=True))
+        assert t1.type == TokenType.PROPERTIES_CHANGED
+        assert t1.ctx.cap_height == 150
+        assert t1.data == r"\H150;"
+
+    def test_change_height_without_semicolon(self):
+        t0, t1, t2 = list(MTextParser(r"word\H150word", yield_property_commands=True))
+        assert t1.type == TokenType.PROPERTIES_CHANGED
+        assert t1.ctx.cap_height == 150
+        assert t1.data == r"\H150"
+
+    def test_change_char_tracking(self):
+        t0, t1, t2 = list(MTextParser(r"word\T150;word", yield_property_commands=True))
+        assert t1.type == TokenType.PROPERTIES_CHANGED
+        assert t1.ctx.char_tracking_factor == 150
+        assert t1.data == r"\T150;"
+
+    def test_change_paragraph(self):
+        t0, t1 = list(
+            MTextParser(r"\pxt4,c5,r6,7.5;word", yield_property_commands=True)
+        )
+        assert t0.type == TokenType.PROPERTIES_CHANGED
+        assert t0.data == r"\pxt4,c5,r6,7.5;"
+
+    def test_one_char_commands(self):
+        t0, t1, t2 = list(
+            MTextParser(r"\Lword\l", yield_property_commands=True)
+        )
+        assert t0.type == TokenType.PROPERTIES_CHANGED
+        assert t0.data == r"\L"
+        assert t2.type == TokenType.PROPERTIES_CHANGED
+        assert t2.data == r"\l"
+
+    def test_unknown_escape_sequence(self):
+        t0, t1 = list(MTextParser(r"word\Yword", yield_property_commands=True))
+        assert t1.type == TokenType.WORD
+        assert t1.data == r"\Yword"
+
 
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_522_text_scanner.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_522_text_scanner.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_523_text_size.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_523_text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_524_block_reference_manager.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_524_block_reference_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_525_transparency.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_525_transparency.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_526_explode.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_526_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_527_gfxattribs.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_527_gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_528_difftags.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_528_difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_529_acis_sat.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_529_acis_sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_530_acis_sab.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_530_acis_sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_531_acis_entities.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_531_acis_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_532_acis_mesh.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_532_acis_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_533_shapefiles.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_533_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_534_dwg_info.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_534_dwg_info.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_535_xref_basic.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_535_xref_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -476,21 +476,21 @@
             factory.is_bound(block_record.endblk, tdoc) is True
         ), "ENDBLK entity not bound to target doc"
 
     def test_load_block_layout_does_type_checking(self, sdoc):
         tdoc = ezdxf.new()
         loader = xref.Loader(sdoc, tdoc)
 
-        with pytest.raises(const.DXFTypeError):
+        with pytest.raises(xref.LayoutError):
             loader.load_block_layout(sdoc.modelspace())
 
-        with pytest.raises(const.DXFTypeError):
+        with pytest.raises(xref.LayoutError):
             loader.load_block_layout(sdoc.paperspace())
 
-        with pytest.raises(const.DXFTypeError):
+        with pytest.raises(xref.LayoutError):
             loader.load_block_layout(None)
 
     def test_load_block_reference(self, sdoc):
         tdoc = ezdxf.new()
         xref.load_modelspace(sdoc, tdoc)
         assert document_has_no_errors(tdoc) is True
```

## Comparing `ezdxf-1.0.3b0/tests/test_05_tools/test_536_xref_conflict.py` & `ezdxf-1.0.4b1/tests/test_05_tools/test_536_xref_conflict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/conftest.py` & `ezdxf-1.0.4b1/tests/test_06_math/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_600_base.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_600_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_601_bulge.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_601_bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_602_vec3.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_602_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_603_vec2.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_603_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_604_banded_matrix.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_604_banded_matrix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_604_linalg.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_604_linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_605_matrix44.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_605_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_606_convexhull.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_606_convexhull.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_607_perlin_noise.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_607_perlin_noise.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_608_intersection_line_line_2d.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_608_intersection_line_line_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_609_point_on_line.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_609_point_on_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_610_ocs.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_610_ocs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_611_ucs.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_611_ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_612_ucs_pass_trough.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_612_ucs_pass_trough.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_613_point_in_poygon.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_613_point_in_poygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_614_construct_3d.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_614_construct_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_615_rytz_axis.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_615_rytz_axis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_616_plane.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_616_plane.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_617_clockwise_orientation.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_617_clockwise_orientation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_618_clipping.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_618_clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_619_greiner_hormann.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_619_greiner_hormann.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_620_knot.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_620_knot.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_621_bspline.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_621_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_622_bsplineu.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_622_bsplineu.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_623_rbspline.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_623_rbspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_624_global_bspline_interpolation.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_624_global_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_626_local_bspline_interpolation.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_626_local_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_627_bspline_basis.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_627_bspline_basis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_629_bezier.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_629_bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_630a_bezier4p_base.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_630a_bezier4p_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_630b_bezier4p_functions.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_630b_bezier4p_functions.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_631_euler_spiral.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_631_euler_spiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_632_bezier3p.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_632_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_640_bbox.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_640_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_641_construction_ray.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_641_construction_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_642_construction_line.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_642_construction_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_643_construction_box.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_643_construction_box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_644_construction_circle.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_644_construction_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_645_construction_arc.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_645_construction_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_646_offset_vertices_2d.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_646_offset_vertices_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_647_transform_tools.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_647_transform_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_648_construction_ellipse.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_648_construction_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_649_nurbs_python_interface.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_649_nurbs_python_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_650_elliptic_arc_span.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_650_elliptic_arc_span.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_651_construction_polyline.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_651_construction_polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_652_approx_param_t.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_652_approx_param_t.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_653_polyline_intersection.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_653_polyline_intersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_654_rtree.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_654_rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_655_dbscan.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_655_dbscan.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_656_k_means.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_656_k_means.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_657_mapbox_earcut.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_657_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_658_bevel_tools.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_658_bevel_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_06_math/test_662_is_convex_polygon_2d.py` & `ezdxf-1.0.4b1/tests/test_06_math/test_662_is_convex_polygon_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_701_arrows.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_701_arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_702_render_forms.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_702_render_forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_703_mesh_builder.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_703_mesh_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_704_render_linear_dimension.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_704_render_linear_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_705_shape.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_705_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_707_trace.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_707_trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_708a_path.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_708a_path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_708b_path_tools.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_708b_path_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -784,7 +784,15 @@
     def test_parallelogram(self):
         p = from_vertices([(0, 0), (2, 0), (3, 1), (1, 1)])
         assert is_rectangular(p) is False
 
     def test_non_aligned_square(self):
         p = from_vertices(forms.rotate(forms.square(2), 30))
         assert is_rectangular(p, aligned=False) is True
+
+
+def test_polyline_with_bulge_value_greater_one():
+    msp = VirtualLayout()
+    pline = msp.add_lwpolyline([(0, 0, 0, 0, 2), (1, 0)])
+    p = make_path(pline, segments=12)
+
+    assert len(p) == 4
```

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_708c_matplotlib_path_tools.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_708c_matplotlib_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_708d_qpainter_path_tools.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_708d_qpainter_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_708e_path_shapes.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_708e_path_shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_708f_path_nesting.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_708f_path_nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_709_linetype_renderer.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_709_linetype_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_711_points.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_711_points.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_712_render_curved_dimension.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_712_render_curved_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_713_mleader_builder.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_713_mleader_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_714_mleader_render_engine.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_714_mleader_render_engine.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_715_hatching.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_715_hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py` & `ezdxf-1.0.4b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_800_mtext_surrogate.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_800_mtext_surrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_801_r12spline.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_801_r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_802_table_painter.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_802_table_painter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_803_entities_to_code.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_803_entities_to_code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_804_importer.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_804_importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_805_pycsg.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_805_pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_806_acadctb.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_806_acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_807_dwg_loader_basics.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_807_dwg_loader_basics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_810_drawing_properties.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_810_drawing_properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_811_drawing_frontend.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_811_drawing_frontend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_813_geo_interface.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_813_geo_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_814_text2path.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_814_text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_815_dxf_browser.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_815_dxf_browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_816_bin_packing.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_816_bin_packing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_817_genetic_algorithm.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_817_genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_818_meshex.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_818_meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_819_menger_sponge.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_819_menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_08_addons/test_820_openscad.py` & `ezdxf-1.0.4b1/tests/test_08_addons/test_820_openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py` & `ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py` & `ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py` & `ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py` & `ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py` & `ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py` & `ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_10_issues/test_issue_414_bbox_calculation.py` & `ezdxf-1.0.4b1/tests/test_10_issues/test_issue_414_bbox_calculation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py` & `ezdxf-1.0.4b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_10_issues/test_issue_574_flattening_error.py` & `ezdxf-1.0.4b1/tests/test_10_issues/test_issue_574_flattening_error.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py` & `ezdxf-1.0.4b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.3b0/tests/test_10_issues/test_issue_749_text_layout.py` & `ezdxf-1.0.4b1/tests/test_10_issues/test_issue_749_text_layout.py`

 * *Files identical despite different names*

