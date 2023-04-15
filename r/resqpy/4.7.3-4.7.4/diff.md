# Comparing `tmp/resqpy-4.7.3.tar.gz` & `tmp/resqpy-4.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resqpy-4.7.3.tar", max compression
+gzip compressed data, was "resqpy-4.7.4.tar", max compression
```

## Comparing `resqpy-4.7.3.tar` & `resqpy-4.7.4.tar`

### file list

```diff
@@ -1,197 +1,197 @@
--rw-r--r--   0        0        0     1059 2023-04-13 05:34:52.752595 resqpy-4.7.3/LICENSE
--rw-r--r--   0        0        0     2893 2023-04-13 05:34:52.752595 resqpy-4.7.3/README.md
--rw-r--r--   0        0        0     3227 2023-04-13 05:35:08.921415 resqpy-4.7.3/pyproject.toml
--rw-r--r--   0        0        0      555 2023-04-13 05:35:08.921415 resqpy-4.7.3/resqpy/__init__.py
--rw-r--r--   0        0        0    24782 2023-04-13 05:34:52.764596 resqpy-4.7.3/resqpy/crs.py
--rw-r--r--   0        0        0     1982 2023-04-13 05:34:52.764596 resqpy-4.7.3/resqpy/derived_model/__init__.py
--rw-r--r--   0        0        0     6410 2023-04-13 05:34:52.764596 resqpy-4.7.3/resqpy/derived_model/_add_edges_per_column_property_array.py
--rw-r--r--   0        0        0    20540 2023-04-13 05:34:52.764596 resqpy-4.7.3/resqpy/derived_model/_add_faults.py
--rw-r--r--   0        0        0     6417 2023-04-13 05:34:52.764596 resqpy-4.7.3/resqpy/derived_model/_add_one_blocked_well_property.py
--rw-r--r--   0        0        0     8657 2023-04-13 05:34:52.764596 resqpy-4.7.3/resqpy/derived_model/_add_one_grid_property_array.py
--rw-r--r--   0        0        0     2431 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_add_single_cell_grid.py
--rw-r--r--   0        0        0     5495 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_add_wells_from_ascii_file.py
--rw-r--r--   0        0        0     6037 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_add_zone_by_layer_property.py
--rw-r--r--   0        0        0    11586 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_coarsened_grid.py
--rw-r--r--   0        0        0    10201 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_common.py
--rw-r--r--   0        0        0     3730 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_copy_grid.py
--rw-r--r--   0        0        0    11731 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_drape_to_surface.py
--rw-r--r--   0        0        0    16391 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_extract_box.py
--rw-r--r--   0        0        0    22969 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_extract_box_for_well.py
--rw-r--r--   0        0        0    20325 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_fault_throw_scaling.py
--rw-r--r--   0        0        0     7157 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_gather_ensemble.py
--rw-r--r--   0        0        0    17929 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_interpolated_grid.py
--rw-r--r--   0        0        0     9876 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_local_depth_adjustment.py
--rw-r--r--   0        0        0    20513 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_refined_grid.py
--rw-r--r--   0        0        0     5166 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_tilted_grid.py
--rw-r--r--   0        0        0     4792 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_unsplit_grid.py
--rw-r--r--   0        0        0    18825 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_zonal_grid.py
--rw-r--r--   0        0        0     4358 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/derived_model/_zone_layer_ranges_from_array.py
--rw-r--r--   0        0        0      996 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/fault/__init__.py
--rw-r--r--   0        0        0    29402 2023-04-13 05:34:52.768596 resqpy-4.7.3/resqpy/fault/_gcs_functions.py
--rw-r--r--   0        0        0   109110 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/fault/_grid_connection_set.py
--rw-r--r--   0        0        0      692 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/__init__.py
--rw-r--r--   0        0        0    20689 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_cell_properties.py
--rw-r--r--   0        0        0    10120 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_connection_sets.py
--rw-r--r--   0        0        0    19936 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_create_grid_xml.py
--rw-r--r--   0        0        0    32064 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_defined_geometry.py
--rw-r--r--   0        0        0    28203 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_extract_functions.py
--rw-r--r--   0        0        0    16516 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_face_functions.py
--rw-r--r--   0        0        0    12236 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_faults.py
--rw-r--r--   0        0        0   127766 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_grid.py
--rw-r--r--   0        0        0     3544 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_grid_types.py
--rw-r--r--   0        0        0      338 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_intervals_info.py
--rw-r--r--   0        0        0      604 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_moved_functions.py
--rw-r--r--   0        0        0     7243 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_pillars.py
--rw-r--r--   0        0        0     5386 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_pixel_maps.py
--rw-r--r--   0        0        0    65440 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_points_functions.py
--rw-r--r--   0        0        0    40520 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_regular_grid.py
--rw-r--r--   0        0        0    19413 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_transmissibility.py
--rw-r--r--   0        0        0     7944 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_write_hdf5_from_caches.py
--rw-r--r--   0        0        0     6147 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_write_nexus_corp.py
--rw-r--r--   0        0        0    13087 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid/_xyz.py
--rw-r--r--   0        0        0     2593 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid_surface/__init__.py
--rw-r--r--   0        0        0    35739 2023-04-13 05:34:52.772596 resqpy-4.7.3/resqpy/grid_surface/_blocked_well_populate.py
--rw-r--r--   0        0        0    64016 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/grid_surface/_find_faces.py
--rw-r--r--   0        0        0    26056 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/grid_surface/_grid_skin.py
--rw-r--r--   0        0        0    14379 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/grid_surface/_grid_surface.py
--rw-r--r--   0        0        0    22498 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/grid_surface/_trajectory_intersects.py
--rw-r--r--   0        0        0    39760 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/grid_surface/grid_surface_cuda.py
--rw-r--r--   0        0        0      539 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/lines/__init__.py
--rw-r--r--   0        0        0    11960 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/lines/_common.py
--rw-r--r--   0        0        0    41425 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/lines/_polyline.py
--rw-r--r--   0        0        0    26366 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/lines/_polyline_set.py
--rw-r--r--   0        0        0      378 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/model/__init__.py
--rw-r--r--   0        0        0    30171 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/model/_catalogue.py
--rw-r--r--   0        0        0     2840 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/model/_context.py
--rw-r--r--   0        0        0    34159 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/model/_forestry.py
--rw-r--r--   0        0        0     3371 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/model/_grids.py
--rw-r--r--   0        0        0    14172 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/model/_hdf5.py
--rw-r--r--   0        0        0   102627 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/model/_model.py
--rw-r--r--   0        0        0    23589 2023-04-13 05:34:52.776596 resqpy-4.7.3/resqpy/model/_xml.py
--rw-r--r--   0        0        0      909 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/multi_processing/__init__.py
--rw-r--r--   0        0        0     7017 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/multi_processing/_multiprocessing.py
--rw-r--r--   0        0        0       72 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/multi_processing/wrappers/__init__.py
--rw-r--r--   0        0        0     5952 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/multi_processing/wrappers/blocked_well_mp.py
--rw-r--r--   0        0        0    21156 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/multi_processing/wrappers/grid_surface_mp.py
--rw-r--r--   0        0        0     5793 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/multi_processing/wrappers/mesh_mp.py
--rw-r--r--   0        0        0       84 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/__init__.py
--rw-r--r--   0        0        0     2147 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/ab_toolbox.py
--rw-r--r--   0        0        0     7521 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/base.py
--rw-r--r--   0        0        0    20925 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/box_utilities.py
--rw-r--r--   0        0        0     5935 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/class_dict.py
--rw-r--r--   0        0        0     9285 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/consolidation.py
--rw-r--r--   0        0        0     5177 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/data/build.py
--rw-r--r--   0        0        0   498136 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/data/properties.json
--rw-r--r--   0        0        0    19836 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/dataframe.py
--rw-r--r--   0        0        0      307 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/exceptions.py
--rw-r--r--   0        0        0     1313 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/factors.py
--rw-r--r--   0        0        0    24541 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/fine_coarse.py
--rw-r--r--   0        0        0    27398 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/grid_functions.py
--rw-r--r--   0        0        0    20158 2023-04-13 05:34:52.780597 resqpy-4.7.3/resqpy/olio/intersection.py
--rw-r--r--   0        0        0     8408 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/keyword_files.py
--rw-r--r--   0        0        0    19210 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/load_data.py
--rw-r--r--   0        0        0     6628 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/point_inclusion.py
--rw-r--r--   0        0        0     1103 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/random_seed.py
--rw-r--r--   0        0        0     5441 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/read_nexus_fault.py
--rw-r--r--   0        0        0    17083 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/relperm.py
--rw-r--r--   0        0        0    12189 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/simple_lines.py
--rw-r--r--   0        0        0      760 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/time.py
--rw-r--r--   0        0        0      822 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/trademark.py
--rw-r--r--   0        0        0    61188 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/transmission.py
--rw-r--r--   0        0        0    44288 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/triangulation.py
--rw-r--r--   0        0        0     7324 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/uuid.py
--rw-r--r--   0        0        0    45231 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/vdb.py
--rw-r--r--   0        0        0    46253 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/vector_utilities.py
--rw-r--r--   0        0        0     6185 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/volume.py
--rw-r--r--   0        0        0    26220 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/wellspec_keywords.py
--rw-r--r--   0        0        0     5142 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/write_data.py
--rw-r--r--   0        0        0    19055 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/write_hdf5.py
--rw-r--r--   0        0        0    24925 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/xml_et.py
--rw-r--r--   0        0        0     1824 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/xml_namespaces.py
--rw-r--r--   0        0        0     5709 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/olio/zmap_reader.py
--rw-r--r--   0        0        0     2206 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/organize/__init__.py
--rw-r--r--   0        0        0     2937 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/organize/_utils.py
--rw-r--r--   0        0        0     1685 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/organize/boundary_feature.py
--rw-r--r--   0        0        0     5190 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/organize/boundary_feature_interpretation.py
--rw-r--r--   0        0        0     6186 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/organize/earth_model_interpretation.py
--rw-r--r--   0        0        0    12457 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/organize/fault_interpretation.py
--rw-r--r--   0        0        0     2757 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/organize/fluid_boundary_feature.py
--rw-r--r--   0        0        0     1702 2023-04-13 05:34:52.784597 resqpy-4.7.3/resqpy/organize/frontier_feature.py
--rw-r--r--   0        0        0     4498 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/organize/generic_interpretation.py
--rw-r--r--   0        0        0     3771 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/organize/genetic_boundary_feature.py
--rw-r--r--   0        0        0     8605 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/organize/geobody_boundary_interpretation.py
--rw-r--r--   0        0        0     1836 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/organize/geobody_feature.py
--rw-r--r--   0        0        0     8052 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/organize/geobody_interpretation.py
--rw-r--r--   0        0        0     1739 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/organize/geologic_unit_feature.py
--rw-r--r--   0        0        0     8346 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/organize/horizon_interpretation.py
--rw-r--r--   0        0        0     2697 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/organize/organization_feature.py
--rw-r--r--   0        0        0     5565 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/organize/rock_fluid_unit_feature.py
--rw-r--r--   0        0        0     2675 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/organize/tectonic_boundary_feature.py
--rw-r--r--   0        0        0     1843 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/organize/wellbore_feature.py
--rw-r--r--   0        0        0     6973 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/organize/wellbore_interpretation.py
--rw-r--r--   0        0        0     2155 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/property/__init__.py
--rw-r--r--   0        0        0    16509 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/property/_collection_add_part.py
--rw-r--r--   0        0        0    13021 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/property/_collection_create_xml.py
--rw-r--r--   0        0        0    30025 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/property/_collection_get_attributes.py
--rw-r--r--   0        0        0     5368 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/property/_collection_support.py
--rw-r--r--   0        0        0    24426 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/property/_property.py
--rw-r--r--   0        0        0    66946 2023-04-13 05:34:52.788597 resqpy-4.7.3/resqpy/property/grid_property_collection.py
--rw-r--r--   0        0        0   143259 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/property/property_collection.py
--rw-r--r--   0        0        0    36127 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/property/property_common.py
--rw-r--r--   0        0        0     5557 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/property/property_kind.py
--rw-r--r--   0        0        0     7737 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/property/string_lookup.py
--rw-r--r--   0        0        0     1077 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/property/well_interval_property.py
--rw-r--r--   0        0        0     1577 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/property/well_interval_property_collection.py
--rw-r--r--   0        0        0     1205 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/property/well_log.py
--rw-r--r--   0        0        0     7633 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/property/well_log_collection.py
--rw-r--r--   0        0        0      713 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/rq_import/__init__.py
--rw-r--r--   0        0        0     4493 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/rq_import/_add_ab_properties.py
--rw-r--r--   0        0        0     6067 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/rq_import/_add_surfaces.py
--rw-r--r--   0        0        0    32019 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/rq_import/_grid_from_cp.py
--rw-r--r--   0        0        0    34317 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/rq_import/_import_nexus.py
--rw-r--r--   0        0        0     6306 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/rq_import/_import_vdb_all_grids.py
--rw-r--r--   0        0        0    21372 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/rq_import/_import_vdb_ensemble.py
--rw-r--r--   0        0        0     1311 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/strata/__init__.py
--rw-r--r--   0        0        0     8861 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/strata/_binary_contact_interpretation.py
--rw-r--r--   0        0        0    10381 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/strata/_geologic_unit_interpretation.py
--rw-r--r--   0        0        0     1772 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/strata/_strata_common.py
--rw-r--r--   0        0        0     6797 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/strata/_stratigraphic_column.py
--rw-r--r--   0        0        0    13322 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/strata/_stratigraphic_column_rank.py
--rw-r--r--   0        0        0     7432 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/strata/_stratigraphic_unit_feature.py
--rw-r--r--   0        0        0    10167 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/strata/_stratigraphic_unit_interpretation.py
--rw-r--r--   0        0        0      696 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/surface/__init__.py
--rw-r--r--   0        0        0     2331 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/surface/_base_surface.py
--rw-r--r--   0        0        0     3082 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/surface/_combined_surface.py
--rw-r--r--   0        0        0    42192 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/surface/_mesh.py
--rw-r--r--   0        0        0    26120 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/surface/_pointset.py
--rw-r--r--   0        0        0    56386 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/surface/_surface.py
--rw-r--r--   0        0        0    24102 2023-04-13 05:34:52.792597 resqpy-4.7.3/resqpy/surface/_tri_mesh.py
--rw-r--r--   0        0        0    25907 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/surface/_triangulated_patch.py
--rw-r--r--   0        0        0     1074 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/time_series/__init__.py
--rw-r--r--   0        0        0     8595 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/time_series/_any_time_series.py
--rw-r--r--   0        0        0     6617 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/time_series/_from_nexus_summary.py
--rw-r--r--   0        0        0     6366 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/time_series/_functions.py
--rw-r--r--   0        0        0     3311 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/time_series/_geologic_time_series.py
--rw-r--r--   0        0        0     2759 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/time_series/_time_duration.py
--rw-r--r--   0        0        0    10818 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/time_series/_time_series.py
--rw-r--r--   0        0        0      603 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/unstructured/__init__.py
--rw-r--r--   0        0        0    15328 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/unstructured/_hexa_grid.py
--rw-r--r--   0        0        0    35856 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/unstructured/_prism_grid.py
--rw-r--r--   0        0        0     7862 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/unstructured/_pyramid_grid.py
--rw-r--r--   0        0        0    10208 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/unstructured/_tetra_grid.py
--rw-r--r--   0        0        0    51550 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/unstructured/_unstructured_grid.py
--rw-r--r--   0        0        0     1135 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/weights_and_measures/__init__.py
--rw-r--r--   0        0        0     4811 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/weights_and_measures/nexus_units.py
--rw-r--r--   0        0        0    16186 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/weights_and_measures/weights_and_measures.py
--rw-r--r--   0        0        0      990 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/well/__init__.py
--rw-r--r--   0        0        0   186259 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/well/_blocked_well.py
--rw-r--r--   0        0        0    22138 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/well/_deviation_survey.py
--rw-r--r--   0        0        0     7154 2023-04-13 05:34:52.796597 resqpy-4.7.3/resqpy/well/_md_datum.py
--rw-r--r--   0        0        0    48693 2023-04-13 05:34:52.800598 resqpy-4.7.3/resqpy/well/_trajectory.py
--rw-r--r--   0        0        0    15192 2023-04-13 05:34:52.800598 resqpy-4.7.3/resqpy/well/_wellbore_frame.py
--rw-r--r--   0        0        0     8403 2023-04-13 05:34:52.800598 resqpy-4.7.3/resqpy/well/_wellbore_marker.py
--rw-r--r--   0        0        0    20933 2023-04-13 05:34:52.800598 resqpy-4.7.3/resqpy/well/_wellbore_marker_frame.py
--rw-r--r--   0        0        0    22556 2023-04-13 05:34:52.800598 resqpy-4.7.3/resqpy/well/blocked_well_frame.py
--rw-r--r--   0        0        0    24743 2023-04-13 05:34:52.800598 resqpy-4.7.3/resqpy/well/well_object_funcs.py
--rw-r--r--   0        0        0     5969 2023-04-13 05:34:52.800598 resqpy-4.7.3/resqpy/well/well_utils.py
--rw-r--r--   0        0        0     4156 1970-01-01 00:00:00.000000 resqpy-4.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-04-15 11:54:37.774578 resqpy-4.7.4/LICENSE
+-rw-r--r--   0        0        0     2893 2023-04-15 11:54:37.774578 resqpy-4.7.4/README.md
+-rw-r--r--   0        0        0     3227 2023-04-15 11:54:53.150790 resqpy-4.7.4/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-04-15 11:54:53.150790 resqpy-4.7.4/resqpy/__init__.py
+-rw-r--r--   0        0        0    24782 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/crs.py
+-rw-r--r--   0        0        0     1982 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/__init__.py
+-rw-r--r--   0        0        0     6410 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_edges_per_column_property_array.py
+-rw-r--r--   0        0        0    20540 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_faults.py
+-rw-r--r--   0        0        0     6417 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_one_blocked_well_property.py
+-rw-r--r--   0        0        0     8657 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_one_grid_property_array.py
+-rw-r--r--   0        0        0     2431 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_single_cell_grid.py
+-rw-r--r--   0        0        0     5495 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_wells_from_ascii_file.py
+-rw-r--r--   0        0        0     6037 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_add_zone_by_layer_property.py
+-rw-r--r--   0        0        0    11586 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_coarsened_grid.py
+-rw-r--r--   0        0        0    10201 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_common.py
+-rw-r--r--   0        0        0     3730 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_copy_grid.py
+-rw-r--r--   0        0        0    11731 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_drape_to_surface.py
+-rw-r--r--   0        0        0    16391 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_extract_box.py
+-rw-r--r--   0        0        0    22969 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_extract_box_for_well.py
+-rw-r--r--   0        0        0    20325 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_fault_throw_scaling.py
+-rw-r--r--   0        0        0     7157 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_gather_ensemble.py
+-rw-r--r--   0        0        0    17929 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_interpolated_grid.py
+-rw-r--r--   0        0        0     9876 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_local_depth_adjustment.py
+-rw-r--r--   0        0        0    20513 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_refined_grid.py
+-rw-r--r--   0        0        0     5166 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_tilted_grid.py
+-rw-r--r--   0        0        0     4792 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_unsplit_grid.py
+-rw-r--r--   0        0        0    18825 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_zonal_grid.py
+-rw-r--r--   0        0        0     4358 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/derived_model/_zone_layer_ranges_from_array.py
+-rw-r--r--   0        0        0      996 2023-04-15 11:54:37.786578 resqpy-4.7.4/resqpy/fault/__init__.py
+-rw-r--r--   0        0        0    29402 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/fault/_gcs_functions.py
+-rw-r--r--   0        0        0   109110 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/fault/_grid_connection_set.py
+-rw-r--r--   0        0        0      692 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/__init__.py
+-rw-r--r--   0        0        0    20689 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_cell_properties.py
+-rw-r--r--   0        0        0    10120 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_connection_sets.py
+-rw-r--r--   0        0        0    19936 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_create_grid_xml.py
+-rw-r--r--   0        0        0    32064 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_defined_geometry.py
+-rw-r--r--   0        0        0    28203 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_extract_functions.py
+-rw-r--r--   0        0        0    16516 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_face_functions.py
+-rw-r--r--   0        0        0    12236 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_faults.py
+-rw-r--r--   0        0        0   127766 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_grid.py
+-rw-r--r--   0        0        0     3544 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_grid_types.py
+-rw-r--r--   0        0        0      338 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_intervals_info.py
+-rw-r--r--   0        0        0      604 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_moved_functions.py
+-rw-r--r--   0        0        0     7243 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_pillars.py
+-rw-r--r--   0        0        0     5386 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_pixel_maps.py
+-rw-r--r--   0        0        0    65440 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_points_functions.py
+-rw-r--r--   0        0        0    40520 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_regular_grid.py
+-rw-r--r--   0        0        0    19413 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_transmissibility.py
+-rw-r--r--   0        0        0     7944 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_write_hdf5_from_caches.py
+-rw-r--r--   0        0        0     6147 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_write_nexus_corp.py
+-rw-r--r--   0        0        0    13087 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid/_xyz.py
+-rw-r--r--   0        0        0     2593 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid_surface/__init__.py
+-rw-r--r--   0        0        0    35739 2023-04-15 11:54:37.790578 resqpy-4.7.4/resqpy/grid_surface/_blocked_well_populate.py
+-rw-r--r--   0        0        0    64016 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/grid_surface/_find_faces.py
+-rw-r--r--   0        0        0    26056 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/grid_surface/_grid_skin.py
+-rw-r--r--   0        0        0    14379 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/grid_surface/_grid_surface.py
+-rw-r--r--   0        0        0    22498 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/grid_surface/_trajectory_intersects.py
+-rw-r--r--   0        0        0    39760 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/grid_surface/grid_surface_cuda.py
+-rw-r--r--   0        0        0      539 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/lines/__init__.py
+-rw-r--r--   0        0        0    11960 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/lines/_common.py
+-rw-r--r--   0        0        0    41425 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/lines/_polyline.py
+-rw-r--r--   0        0        0    26366 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/lines/_polyline_set.py
+-rw-r--r--   0        0        0      378 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/__init__.py
+-rw-r--r--   0        0        0    30171 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_catalogue.py
+-rw-r--r--   0        0        0     2840 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_context.py
+-rw-r--r--   0        0        0    34159 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_forestry.py
+-rw-r--r--   0        0        0     3371 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_grids.py
+-rw-r--r--   0        0        0    14172 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_hdf5.py
+-rw-r--r--   0        0        0   103055 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_model.py
+-rw-r--r--   0        0        0    23589 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/model/_xml.py
+-rw-r--r--   0        0        0      909 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/multi_processing/__init__.py
+-rw-r--r--   0        0        0     7017 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/multi_processing/_multiprocessing.py
+-rw-r--r--   0        0        0       72 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/multi_processing/wrappers/__init__.py
+-rw-r--r--   0        0        0     5952 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/multi_processing/wrappers/blocked_well_mp.py
+-rw-r--r--   0        0        0    21156 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/multi_processing/wrappers/grid_surface_mp.py
+-rw-r--r--   0        0        0     5793 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/multi_processing/wrappers/mesh_mp.py
+-rw-r--r--   0        0        0       84 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/olio/__init__.py
+-rw-r--r--   0        0        0     2147 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/olio/ab_toolbox.py
+-rw-r--r--   0        0        0     7521 2023-04-15 11:54:37.794578 resqpy-4.7.4/resqpy/olio/base.py
+-rw-r--r--   0        0        0    20925 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/box_utilities.py
+-rw-r--r--   0        0        0     5935 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/class_dict.py
+-rw-r--r--   0        0        0     9285 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/consolidation.py
+-rw-r--r--   0        0        0     5177 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/data/build.py
+-rw-r--r--   0        0        0   498136 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/data/properties.json
+-rw-r--r--   0        0        0    19836 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/dataframe.py
+-rw-r--r--   0        0        0      307 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/exceptions.py
+-rw-r--r--   0        0        0     1313 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/factors.py
+-rw-r--r--   0        0        0    24541 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/fine_coarse.py
+-rw-r--r--   0        0        0    27398 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/grid_functions.py
+-rw-r--r--   0        0        0    20158 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/intersection.py
+-rw-r--r--   0        0        0     8408 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/keyword_files.py
+-rw-r--r--   0        0        0    19210 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/load_data.py
+-rw-r--r--   0        0        0     6628 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/point_inclusion.py
+-rw-r--r--   0        0        0     1103 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/random_seed.py
+-rw-r--r--   0        0        0     5441 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/read_nexus_fault.py
+-rw-r--r--   0        0        0    17083 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/relperm.py
+-rw-r--r--   0        0        0    12189 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/simple_lines.py
+-rw-r--r--   0        0        0      760 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/time.py
+-rw-r--r--   0        0        0      822 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/trademark.py
+-rw-r--r--   0        0        0    61188 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/transmission.py
+-rw-r--r--   0        0        0    44288 2023-04-15 11:54:37.798578 resqpy-4.7.4/resqpy/olio/triangulation.py
+-rw-r--r--   0        0        0     7324 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/uuid.py
+-rw-r--r--   0        0        0    45231 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/vdb.py
+-rw-r--r--   0        0        0    46253 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/vector_utilities.py
+-rw-r--r--   0        0        0     6185 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/volume.py
+-rw-r--r--   0        0        0    26220 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/wellspec_keywords.py
+-rw-r--r--   0        0        0     5142 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/write_data.py
+-rw-r--r--   0        0        0    19055 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/write_hdf5.py
+-rw-r--r--   0        0        0    24925 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/xml_et.py
+-rw-r--r--   0        0        0     1824 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/xml_namespaces.py
+-rw-r--r--   0        0        0     5709 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/olio/zmap_reader.py
+-rw-r--r--   0        0        0     2206 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/__init__.py
+-rw-r--r--   0        0        0     2937 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/_utils.py
+-rw-r--r--   0        0        0     1685 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/boundary_feature.py
+-rw-r--r--   0        0        0     5190 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/boundary_feature_interpretation.py
+-rw-r--r--   0        0        0     6186 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/earth_model_interpretation.py
+-rw-r--r--   0        0        0    12457 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/fault_interpretation.py
+-rw-r--r--   0        0        0     2757 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/fluid_boundary_feature.py
+-rw-r--r--   0        0        0     1702 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/frontier_feature.py
+-rw-r--r--   0        0        0     4498 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/generic_interpretation.py
+-rw-r--r--   0        0        0     3771 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/genetic_boundary_feature.py
+-rw-r--r--   0        0        0     8605 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/geobody_boundary_interpretation.py
+-rw-r--r--   0        0        0     1836 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/geobody_feature.py
+-rw-r--r--   0        0        0     8052 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/geobody_interpretation.py
+-rw-r--r--   0        0        0     1739 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/geologic_unit_feature.py
+-rw-r--r--   0        0        0     8346 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/horizon_interpretation.py
+-rw-r--r--   0        0        0     2697 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/organization_feature.py
+-rw-r--r--   0        0        0     5565 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/rock_fluid_unit_feature.py
+-rw-r--r--   0        0        0     2675 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/tectonic_boundary_feature.py
+-rw-r--r--   0        0        0     1843 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/wellbore_feature.py
+-rw-r--r--   0        0        0     6973 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/organize/wellbore_interpretation.py
+-rw-r--r--   0        0        0     2155 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/property/__init__.py
+-rw-r--r--   0        0        0    16509 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/property/_collection_add_part.py
+-rw-r--r--   0        0        0    13021 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/property/_collection_create_xml.py
+-rw-r--r--   0        0        0    30025 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/property/_collection_get_attributes.py
+-rw-r--r--   0        0        0     5368 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/property/_collection_support.py
+-rw-r--r--   0        0        0    24426 2023-04-15 11:54:37.802578 resqpy-4.7.4/resqpy/property/_property.py
+-rw-r--r--   0        0        0    66946 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/grid_property_collection.py
+-rw-r--r--   0        0        0   143259 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/property_collection.py
+-rw-r--r--   0        0        0    36127 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/property_common.py
+-rw-r--r--   0        0        0     5557 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/property_kind.py
+-rw-r--r--   0        0        0     7737 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/string_lookup.py
+-rw-r--r--   0        0        0     1077 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/well_interval_property.py
+-rw-r--r--   0        0        0     1577 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/well_interval_property_collection.py
+-rw-r--r--   0        0        0     1205 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/well_log.py
+-rw-r--r--   0        0        0     7633 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/property/well_log_collection.py
+-rw-r--r--   0        0        0      713 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/__init__.py
+-rw-r--r--   0        0        0     4493 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/_add_ab_properties.py
+-rw-r--r--   0        0        0     6067 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/_add_surfaces.py
+-rw-r--r--   0        0        0    32019 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/_grid_from_cp.py
+-rw-r--r--   0        0        0    34317 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/_import_nexus.py
+-rw-r--r--   0        0        0     6306 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/_import_vdb_all_grids.py
+-rw-r--r--   0        0        0    21372 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/rq_import/_import_vdb_ensemble.py
+-rw-r--r--   0        0        0     1311 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/__init__.py
+-rw-r--r--   0        0        0     8861 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_binary_contact_interpretation.py
+-rw-r--r--   0        0        0    10381 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_geologic_unit_interpretation.py
+-rw-r--r--   0        0        0     1772 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_strata_common.py
+-rw-r--r--   0        0        0     6797 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_stratigraphic_column.py
+-rw-r--r--   0        0        0    13322 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_stratigraphic_column_rank.py
+-rw-r--r--   0        0        0     7432 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_stratigraphic_unit_feature.py
+-rw-r--r--   0        0        0    10167 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/strata/_stratigraphic_unit_interpretation.py
+-rw-r--r--   0        0        0      696 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/surface/__init__.py
+-rw-r--r--   0        0        0     2331 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/surface/_base_surface.py
+-rw-r--r--   0        0        0     3082 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/surface/_combined_surface.py
+-rw-r--r--   0        0        0    42192 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/surface/_mesh.py
+-rw-r--r--   0        0        0    26120 2023-04-15 11:54:37.806578 resqpy-4.7.4/resqpy/surface/_pointset.py
+-rw-r--r--   0        0        0    56386 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/surface/_surface.py
+-rw-r--r--   0        0        0    24102 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/surface/_tri_mesh.py
+-rw-r--r--   0        0        0    25907 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/surface/_triangulated_patch.py
+-rw-r--r--   0        0        0     1074 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/__init__.py
+-rw-r--r--   0        0        0     8595 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/_any_time_series.py
+-rw-r--r--   0        0        0     6617 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/_from_nexus_summary.py
+-rw-r--r--   0        0        0     6366 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/_functions.py
+-rw-r--r--   0        0        0     3311 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/_geologic_time_series.py
+-rw-r--r--   0        0        0     2759 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/_time_duration.py
+-rw-r--r--   0        0        0    10818 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/time_series/_time_series.py
+-rw-r--r--   0        0        0      603 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/unstructured/__init__.py
+-rw-r--r--   0        0        0    15328 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/unstructured/_hexa_grid.py
+-rw-r--r--   0        0        0    35856 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/unstructured/_prism_grid.py
+-rw-r--r--   0        0        0     7862 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/unstructured/_pyramid_grid.py
+-rw-r--r--   0        0        0    10208 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/unstructured/_tetra_grid.py
+-rw-r--r--   0        0        0    51550 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/unstructured/_unstructured_grid.py
+-rw-r--r--   0        0        0     1135 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/weights_and_measures/__init__.py
+-rw-r--r--   0        0        0     4811 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/weights_and_measures/nexus_units.py
+-rw-r--r--   0        0        0    16186 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/weights_and_measures/weights_and_measures.py
+-rw-r--r--   0        0        0      990 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/well/__init__.py
+-rw-r--r--   0        0        0   186258 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/well/_blocked_well.py
+-rw-r--r--   0        0        0    22138 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/well/_deviation_survey.py
+-rw-r--r--   0        0        0     7154 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/well/_md_datum.py
+-rw-r--r--   0        0        0    48693 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/well/_trajectory.py
+-rw-r--r--   0        0        0    15192 2023-04-15 11:54:37.810578 resqpy-4.7.4/resqpy/well/_wellbore_frame.py
+-rw-r--r--   0        0        0     8403 2023-04-15 11:54:37.814578 resqpy-4.7.4/resqpy/well/_wellbore_marker.py
+-rw-r--r--   0        0        0    20933 2023-04-15 11:54:37.814578 resqpy-4.7.4/resqpy/well/_wellbore_marker_frame.py
+-rw-r--r--   0        0        0    22555 2023-04-15 11:54:37.814578 resqpy-4.7.4/resqpy/well/blocked_well_frame.py
+-rw-r--r--   0        0        0    24743 2023-04-15 11:54:37.814578 resqpy-4.7.4/resqpy/well/well_object_funcs.py
+-rw-r--r--   0        0        0     5969 2023-04-15 11:54:37.814578 resqpy-4.7.4/resqpy/well/well_utils.py
+-rw-r--r--   0        0        0     4156 1970-01-01 00:00:00.000000 resqpy-4.7.4/PKG-INFO
```

### Comparing `resqpy-4.7.3/LICENSE` & `resqpy-4.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/README.md` & `resqpy-4.7.4/README.md`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/pyproject.toml` & `resqpy-4.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [build-system]
 requires = ["poetry>=1.0.2", "poetry-dynamic-versioning"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "resqpy"
-version = "4.7.3" # Set at build time
+version = "4.7.4" # Set at build time
 description = "Python API for working with RESQML models"
 authors = ["BP"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bp/resqpy"
 documentation = "https://resqpy.readthedocs.io/en/latest/"
 keywords = ["RESQML"]
```

### Comparing `resqpy-4.7.3/resqpy/__init__.py` & `resqpy-4.7.4/resqpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,10 +24,10 @@
     weights_and_measures
     well
     olio
 """
 
 import logging
 
-__version__ = "4.7.3"  # Set at build time
+__version__ = "4.7.4"  # Set at build time
 log = logging.getLogger(__name__)
 log.info(f"Imported resqpy version {__version__}")
```

### Comparing `resqpy-4.7.3/resqpy/crs.py` & `resqpy-4.7.4/resqpy/crs.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/__init__.py` & `resqpy-4.7.4/resqpy/derived_model/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_add_edges_per_column_property_array.py` & `resqpy-4.7.4/resqpy/derived_model/_add_edges_per_column_property_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_add_faults.py` & `resqpy-4.7.4/resqpy/derived_model/_add_faults.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_add_one_blocked_well_property.py` & `resqpy-4.7.4/resqpy/derived_model/_add_one_blocked_well_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_add_one_grid_property_array.py` & `resqpy-4.7.4/resqpy/derived_model/_add_one_grid_property_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_add_single_cell_grid.py` & `resqpy-4.7.4/resqpy/derived_model/_add_single_cell_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_add_wells_from_ascii_file.py` & `resqpy-4.7.4/resqpy/derived_model/_add_wells_from_ascii_file.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_add_zone_by_layer_property.py` & `resqpy-4.7.4/resqpy/derived_model/_add_zone_by_layer_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_coarsened_grid.py` & `resqpy-4.7.4/resqpy/derived_model/_coarsened_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_common.py` & `resqpy-4.7.4/resqpy/derived_model/_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_copy_grid.py` & `resqpy-4.7.4/resqpy/derived_model/_copy_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_drape_to_surface.py` & `resqpy-4.7.4/resqpy/derived_model/_drape_to_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_extract_box.py` & `resqpy-4.7.4/resqpy/derived_model/_extract_box.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_extract_box_for_well.py` & `resqpy-4.7.4/resqpy/derived_model/_extract_box_for_well.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_fault_throw_scaling.py` & `resqpy-4.7.4/resqpy/derived_model/_fault_throw_scaling.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_gather_ensemble.py` & `resqpy-4.7.4/resqpy/derived_model/_gather_ensemble.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_interpolated_grid.py` & `resqpy-4.7.4/resqpy/derived_model/_interpolated_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_local_depth_adjustment.py` & `resqpy-4.7.4/resqpy/derived_model/_local_depth_adjustment.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_refined_grid.py` & `resqpy-4.7.4/resqpy/derived_model/_refined_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_tilted_grid.py` & `resqpy-4.7.4/resqpy/derived_model/_tilted_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_unsplit_grid.py` & `resqpy-4.7.4/resqpy/derived_model/_unsplit_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_zonal_grid.py` & `resqpy-4.7.4/resqpy/derived_model/_zonal_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/derived_model/_zone_layer_ranges_from_array.py` & `resqpy-4.7.4/resqpy/derived_model/_zone_layer_ranges_from_array.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/fault/__init__.py` & `resqpy-4.7.4/resqpy/fault/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/fault/_gcs_functions.py` & `resqpy-4.7.4/resqpy/fault/_gcs_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/fault/_grid_connection_set.py` & `resqpy-4.7.4/resqpy/fault/_grid_connection_set.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/__init__.py` & `resqpy-4.7.4/resqpy/grid/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_cell_properties.py` & `resqpy-4.7.4/resqpy/grid/_cell_properties.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_connection_sets.py` & `resqpy-4.7.4/resqpy/grid/_connection_sets.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_create_grid_xml.py` & `resqpy-4.7.4/resqpy/grid/_create_grid_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_defined_geometry.py` & `resqpy-4.7.4/resqpy/grid/_defined_geometry.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_extract_functions.py` & `resqpy-4.7.4/resqpy/grid/_extract_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_face_functions.py` & `resqpy-4.7.4/resqpy/grid/_face_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_faults.py` & `resqpy-4.7.4/resqpy/grid/_faults.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_grid.py` & `resqpy-4.7.4/resqpy/grid/_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_grid_types.py` & `resqpy-4.7.4/resqpy/grid/_grid_types.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_moved_functions.py` & `resqpy-4.7.4/resqpy/grid/_moved_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_pillars.py` & `resqpy-4.7.4/resqpy/grid/_pillars.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_pixel_maps.py` & `resqpy-4.7.4/resqpy/grid/_pixel_maps.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_points_functions.py` & `resqpy-4.7.4/resqpy/grid/_points_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_regular_grid.py` & `resqpy-4.7.4/resqpy/grid/_regular_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_transmissibility.py` & `resqpy-4.7.4/resqpy/grid/_transmissibility.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_write_hdf5_from_caches.py` & `resqpy-4.7.4/resqpy/grid/_write_hdf5_from_caches.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_write_nexus_corp.py` & `resqpy-4.7.4/resqpy/grid/_write_nexus_corp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid/_xyz.py` & `resqpy-4.7.4/resqpy/grid/_xyz.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid_surface/__init__.py` & `resqpy-4.7.4/resqpy/grid_surface/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid_surface/_blocked_well_populate.py` & `resqpy-4.7.4/resqpy/grid_surface/_blocked_well_populate.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid_surface/_find_faces.py` & `resqpy-4.7.4/resqpy/grid_surface/_find_faces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid_surface/_grid_skin.py` & `resqpy-4.7.4/resqpy/grid_surface/_grid_skin.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid_surface/_grid_surface.py` & `resqpy-4.7.4/resqpy/grid_surface/_grid_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid_surface/_trajectory_intersects.py` & `resqpy-4.7.4/resqpy/grid_surface/_trajectory_intersects.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/grid_surface/grid_surface_cuda.py` & `resqpy-4.7.4/resqpy/grid_surface/grid_surface_cuda.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/lines/__init__.py` & `resqpy-4.7.4/resqpy/lines/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/lines/_common.py` & `resqpy-4.7.4/resqpy/lines/_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/lines/_polyline.py` & `resqpy-4.7.4/resqpy/lines/_polyline.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/lines/_polyline_set.py` & `resqpy-4.7.4/resqpy/lines/_polyline_set.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/model/_catalogue.py` & `resqpy-4.7.4/resqpy/model/_catalogue.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/model/_context.py` & `resqpy-4.7.4/resqpy/model/_context.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/model/_forestry.py` & `resqpy-4.7.4/resqpy/model/_forestry.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/model/_grids.py` & `resqpy-4.7.4/resqpy/model/_grids.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/model/_hdf5.py` & `resqpy-4.7.4/resqpy/model/_hdf5.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/model/_model.py` & `resqpy-4.7.4/resqpy/model/_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -788,14 +788,25 @@
         returns:
            list of pairs, each being (string, int) representing part type, ie. resqml object class, without leading
            obj underscore, and count
         """
 
         return m_c._parts_count_by_type(self, type_of_interest = type_of_interest)
 
+    def parts_count_dict(self):
+        """Returns a dictionary mapping from RESQML object type to count of parts.
+
+        returns:
+           dict mapping string to int with key being RESQML class and value being count of number of parts
+
+        note:
+           only RESQML classes with at least one object present in the model will be included in the dictionary
+        """
+        return dict(self.parts_count_by_type())
+
     def parts_list_filtered_by_related_uuid(self, parts_list, uuid, uuid_is_source = None, related_mode = None):
         """From a list of parts, returns a list of those parts which have a relationship with the given uuid.
 
         arguments:
            parts_list (list of strings): input list of parts from which a selection is made
            uuid (uuid.UUID): the uuid of a part for which related parts are required
            uuid_is_source (boolean, default None): if None, relationships in either direction qualify;
```

### Comparing `resqpy-4.7.3/resqpy/model/_xml.py` & `resqpy-4.7.4/resqpy/model/_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/multi_processing/__init__.py` & `resqpy-4.7.4/resqpy/multi_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/multi_processing/_multiprocessing.py` & `resqpy-4.7.4/resqpy/multi_processing/_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/multi_processing/wrappers/blocked_well_mp.py` & `resqpy-4.7.4/resqpy/multi_processing/wrappers/blocked_well_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/multi_processing/wrappers/grid_surface_mp.py` & `resqpy-4.7.4/resqpy/multi_processing/wrappers/grid_surface_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/multi_processing/wrappers/mesh_mp.py` & `resqpy-4.7.4/resqpy/multi_processing/wrappers/mesh_mp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/ab_toolbox.py` & `resqpy-4.7.4/resqpy/olio/ab_toolbox.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/base.py` & `resqpy-4.7.4/resqpy/olio/base.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/box_utilities.py` & `resqpy-4.7.4/resqpy/olio/box_utilities.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/class_dict.py` & `resqpy-4.7.4/resqpy/olio/class_dict.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/consolidation.py` & `resqpy-4.7.4/resqpy/olio/consolidation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/data/build.py` & `resqpy-4.7.4/resqpy/olio/data/build.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/data/properties.json` & `resqpy-4.7.4/resqpy/olio/data/properties.json`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/dataframe.py` & `resqpy-4.7.4/resqpy/olio/dataframe.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/factors.py` & `resqpy-4.7.4/resqpy/olio/factors.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/fine_coarse.py` & `resqpy-4.7.4/resqpy/olio/fine_coarse.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/grid_functions.py` & `resqpy-4.7.4/resqpy/olio/grid_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/intersection.py` & `resqpy-4.7.4/resqpy/olio/intersection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/keyword_files.py` & `resqpy-4.7.4/resqpy/olio/keyword_files.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/load_data.py` & `resqpy-4.7.4/resqpy/olio/load_data.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/point_inclusion.py` & `resqpy-4.7.4/resqpy/olio/point_inclusion.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/random_seed.py` & `resqpy-4.7.4/resqpy/olio/random_seed.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/read_nexus_fault.py` & `resqpy-4.7.4/resqpy/olio/read_nexus_fault.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/relperm.py` & `resqpy-4.7.4/resqpy/olio/relperm.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/simple_lines.py` & `resqpy-4.7.4/resqpy/olio/simple_lines.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/time.py` & `resqpy-4.7.4/resqpy/olio/time.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/trademark.py` & `resqpy-4.7.4/resqpy/olio/trademark.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/transmission.py` & `resqpy-4.7.4/resqpy/olio/transmission.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/triangulation.py` & `resqpy-4.7.4/resqpy/olio/triangulation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/uuid.py` & `resqpy-4.7.4/resqpy/olio/uuid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/vdb.py` & `resqpy-4.7.4/resqpy/olio/vdb.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/vector_utilities.py` & `resqpy-4.7.4/resqpy/olio/vector_utilities.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/volume.py` & `resqpy-4.7.4/resqpy/olio/volume.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/wellspec_keywords.py` & `resqpy-4.7.4/resqpy/olio/wellspec_keywords.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/write_data.py` & `resqpy-4.7.4/resqpy/olio/write_data.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/write_hdf5.py` & `resqpy-4.7.4/resqpy/olio/write_hdf5.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/xml_et.py` & `resqpy-4.7.4/resqpy/olio/xml_et.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/xml_namespaces.py` & `resqpy-4.7.4/resqpy/olio/xml_namespaces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/olio/zmap_reader.py` & `resqpy-4.7.4/resqpy/olio/zmap_reader.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/__init__.py` & `resqpy-4.7.4/resqpy/organize/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/_utils.py` & `resqpy-4.7.4/resqpy/organize/_utils.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/boundary_feature.py` & `resqpy-4.7.4/resqpy/organize/boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/boundary_feature_interpretation.py` & `resqpy-4.7.4/resqpy/organize/boundary_feature_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/earth_model_interpretation.py` & `resqpy-4.7.4/resqpy/organize/earth_model_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/fault_interpretation.py` & `resqpy-4.7.4/resqpy/organize/fault_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/fluid_boundary_feature.py` & `resqpy-4.7.4/resqpy/organize/fluid_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/frontier_feature.py` & `resqpy-4.7.4/resqpy/organize/frontier_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/generic_interpretation.py` & `resqpy-4.7.4/resqpy/organize/generic_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/genetic_boundary_feature.py` & `resqpy-4.7.4/resqpy/organize/genetic_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/geobody_boundary_interpretation.py` & `resqpy-4.7.4/resqpy/organize/geobody_boundary_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/geobody_feature.py` & `resqpy-4.7.4/resqpy/organize/geobody_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/geobody_interpretation.py` & `resqpy-4.7.4/resqpy/organize/geobody_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/geologic_unit_feature.py` & `resqpy-4.7.4/resqpy/organize/geologic_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/horizon_interpretation.py` & `resqpy-4.7.4/resqpy/organize/horizon_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/organization_feature.py` & `resqpy-4.7.4/resqpy/organize/organization_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/rock_fluid_unit_feature.py` & `resqpy-4.7.4/resqpy/organize/rock_fluid_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/tectonic_boundary_feature.py` & `resqpy-4.7.4/resqpy/organize/tectonic_boundary_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/wellbore_feature.py` & `resqpy-4.7.4/resqpy/organize/wellbore_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/organize/wellbore_interpretation.py` & `resqpy-4.7.4/resqpy/organize/wellbore_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/__init__.py` & `resqpy-4.7.4/resqpy/property/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/_collection_add_part.py` & `resqpy-4.7.4/resqpy/property/_collection_add_part.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/_collection_create_xml.py` & `resqpy-4.7.4/resqpy/property/_collection_create_xml.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/_collection_get_attributes.py` & `resqpy-4.7.4/resqpy/property/_collection_get_attributes.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/_collection_support.py` & `resqpy-4.7.4/resqpy/property/_collection_support.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/_property.py` & `resqpy-4.7.4/resqpy/property/_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/grid_property_collection.py` & `resqpy-4.7.4/resqpy/property/grid_property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/property_collection.py` & `resqpy-4.7.4/resqpy/property/property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/property_common.py` & `resqpy-4.7.4/resqpy/property/property_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/property_kind.py` & `resqpy-4.7.4/resqpy/property/property_kind.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/string_lookup.py` & `resqpy-4.7.4/resqpy/property/string_lookup.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/well_interval_property.py` & `resqpy-4.7.4/resqpy/property/well_interval_property.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/well_interval_property_collection.py` & `resqpy-4.7.4/resqpy/property/well_interval_property_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/well_log.py` & `resqpy-4.7.4/resqpy/property/well_log.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/property/well_log_collection.py` & `resqpy-4.7.4/resqpy/property/well_log_collection.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/rq_import/__init__.py` & `resqpy-4.7.4/resqpy/rq_import/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/rq_import/_add_ab_properties.py` & `resqpy-4.7.4/resqpy/rq_import/_add_ab_properties.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/rq_import/_add_surfaces.py` & `resqpy-4.7.4/resqpy/rq_import/_add_surfaces.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/rq_import/_grid_from_cp.py` & `resqpy-4.7.4/resqpy/rq_import/_grid_from_cp.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/rq_import/_import_nexus.py` & `resqpy-4.7.4/resqpy/rq_import/_import_nexus.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/rq_import/_import_vdb_all_grids.py` & `resqpy-4.7.4/resqpy/rq_import/_import_vdb_all_grids.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/rq_import/_import_vdb_ensemble.py` & `resqpy-4.7.4/resqpy/rq_import/_import_vdb_ensemble.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/strata/__init__.py` & `resqpy-4.7.4/resqpy/strata/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/strata/_binary_contact_interpretation.py` & `resqpy-4.7.4/resqpy/strata/_binary_contact_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/strata/_geologic_unit_interpretation.py` & `resqpy-4.7.4/resqpy/strata/_geologic_unit_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/strata/_strata_common.py` & `resqpy-4.7.4/resqpy/strata/_strata_common.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/strata/_stratigraphic_column.py` & `resqpy-4.7.4/resqpy/strata/_stratigraphic_column.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/strata/_stratigraphic_column_rank.py` & `resqpy-4.7.4/resqpy/strata/_stratigraphic_column_rank.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/strata/_stratigraphic_unit_feature.py` & `resqpy-4.7.4/resqpy/strata/_stratigraphic_unit_feature.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/strata/_stratigraphic_unit_interpretation.py` & `resqpy-4.7.4/resqpy/strata/_stratigraphic_unit_interpretation.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/surface/__init__.py` & `resqpy-4.7.4/resqpy/surface/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/surface/_base_surface.py` & `resqpy-4.7.4/resqpy/surface/_base_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/surface/_combined_surface.py` & `resqpy-4.7.4/resqpy/surface/_combined_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/surface/_mesh.py` & `resqpy-4.7.4/resqpy/surface/_mesh.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/surface/_pointset.py` & `resqpy-4.7.4/resqpy/surface/_pointset.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/surface/_surface.py` & `resqpy-4.7.4/resqpy/surface/_surface.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/surface/_tri_mesh.py` & `resqpy-4.7.4/resqpy/surface/_tri_mesh.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/surface/_triangulated_patch.py` & `resqpy-4.7.4/resqpy/surface/_triangulated_patch.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/time_series/__init__.py` & `resqpy-4.7.4/resqpy/time_series/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/time_series/_any_time_series.py` & `resqpy-4.7.4/resqpy/time_series/_any_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/time_series/_from_nexus_summary.py` & `resqpy-4.7.4/resqpy/time_series/_from_nexus_summary.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/time_series/_functions.py` & `resqpy-4.7.4/resqpy/time_series/_functions.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/time_series/_geologic_time_series.py` & `resqpy-4.7.4/resqpy/time_series/_geologic_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/time_series/_time_duration.py` & `resqpy-4.7.4/resqpy/time_series/_time_duration.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/time_series/_time_series.py` & `resqpy-4.7.4/resqpy/time_series/_time_series.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/unstructured/__init__.py` & `resqpy-4.7.4/resqpy/unstructured/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/unstructured/_hexa_grid.py` & `resqpy-4.7.4/resqpy/unstructured/_hexa_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/unstructured/_prism_grid.py` & `resqpy-4.7.4/resqpy/unstructured/_prism_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/unstructured/_pyramid_grid.py` & `resqpy-4.7.4/resqpy/unstructured/_pyramid_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/unstructured/_tetra_grid.py` & `resqpy-4.7.4/resqpy/unstructured/_tetra_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/unstructured/_unstructured_grid.py` & `resqpy-4.7.4/resqpy/unstructured/_unstructured_grid.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/weights_and_measures/__init__.py` & `resqpy-4.7.4/resqpy/weights_and_measures/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/weights_and_measures/nexus_units.py` & `resqpy-4.7.4/resqpy/weights_and_measures/nexus_units.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/weights_and_measures/weights_and_measures.py` & `resqpy-4.7.4/resqpy/weights_and_measures/weights_and_measures.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/well/__init__.py` & `resqpy-4.7.4/resqpy/well/__init__.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/well/_blocked_well.py` & `resqpy-4.7.4/resqpy/well/_blocked_well.py`

 * *Files 0% similar despite different names*

```diff
@@ -1760,15 +1760,15 @@
         """
 
         # note: 'active' ia a static property kind used to indicate that a cell is perforated or otherwise
         # open to flow at some time, so needs to appear somewhere in well specification data for flow simulation;
         # 'well connection open' is a dynamic indicator used to identify time periods when a connection is open
         # handled_property_kinds = [
         #     'active', 'well connection open', 'length', 'permeability length', 'skin', 'wellbore radius',
-        #     'non darcy flow coefficient']
+        #     'nonDarcy flow coefficient']
 
         return bwf.add_blocked_well_properties_from_wellbore_frame(self,
                                                                    frame_uuid = frame_uuid,
                                                                    property_kinds_list = property_kinds_list,
                                                                    realization = realization,
                                                                    set_length = set_length,
                                                                    set_perforation_fraction = set_perforation_fraction,
```

### Comparing `resqpy-4.7.3/resqpy/well/_deviation_survey.py` & `resqpy-4.7.4/resqpy/well/_deviation_survey.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/well/_md_datum.py` & `resqpy-4.7.4/resqpy/well/_md_datum.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/well/_trajectory.py` & `resqpy-4.7.4/resqpy/well/_trajectory.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/well/_wellbore_frame.py` & `resqpy-4.7.4/resqpy/well/_wellbore_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/well/_wellbore_marker.py` & `resqpy-4.7.4/resqpy/well/_wellbore_marker.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/well/_wellbore_marker_frame.py` & `resqpy-4.7.4/resqpy/well/_wellbore_marker_frame.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/well/blocked_well_frame.py` & `resqpy-4.7.4/resqpy/well/blocked_well_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     """
 
     # note: 'active' ia a static property kind used to indicate that a cell is perforated or otherwise
     # open to flow at some time, so needs to appear somewhere in well specification data for flow simulation;
     # 'well connection open' is a dynamic indicator used to identify time periods when a connection is open
     handled_property_kinds = [
         'active', 'well connection open', 'length', 'permeability length', 'skin', 'wellbore radius',
-        'non darcy flow coefficient'
+        'nonDarcy flow coefficient'
     ]
 
     def pk_pc_and_ts(pc, pk):
         """Returns a selective property collection based on property kind and a time series uuid if used."""
         pk_pc = rqp.selective_version_of_collection(pc, property_kind = pk)
         ts_uuids = pk_pc.time_series_uuid_list(sort_list = False)
         assert 0 <= len(ts_uuids) <= 1
@@ -371,15 +371,15 @@
                                                     uom = skin_uom,
                                                     property_kind = 'skin',
                                                     time_index = skin_pc.time_index_for_part(skin_part),
                                                     time_series_uuid = ts_uuid,
                                                     realization = realization,
                                                     indexable_element = 'cells')
 
-    # TODO: non darcy flow coefficient
+    # TODO: non Darcy flow coefficient
     # D factor is complicated: it appears in the inflow equation as a rate dependent adjustment to skin
 
     wb_pc.write_hdf5_for_imported_list()
     uuids = wb_pc.create_xml_for_imported_list_and_add_parts_to_model()
 
     if set_frame_interval:
         bw.model.create_reciprocal_relationship_uuids(uuids[0], 'sourceObject', frame_uuid, 'destinationObject')
```

### Comparing `resqpy-4.7.3/resqpy/well/well_object_funcs.py` & `resqpy-4.7.4/resqpy/well/well_object_funcs.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/resqpy/well/well_utils.py` & `resqpy-4.7.4/resqpy/well/well_utils.py`

 * *Files identical despite different names*

### Comparing `resqpy-4.7.3/PKG-INFO` & `resqpy-4.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resqpy
-Version: 4.7.3
+Version: 4.7.4
 Summary: Python API for working with RESQML models
 Home-page: https://github.com/bp/resqpy
 License: MIT
 Keywords: RESQML
 Author: BP
 Requires-Python: >=3.8.1,<3.11
 Classifier: Development Status :: 5 - Production/Stable
```

