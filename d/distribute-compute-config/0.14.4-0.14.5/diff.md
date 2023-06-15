# Comparing `tmp/distribute_compute_config-0.14.4.tar.gz` & `tmp/distribute_compute_config-0.14.5.tar.gz`

## Comparing `distribute_compute_config-0.14.4.tar` & `distribute_compute_config-0.14.5.tar`

### file list

```diff
@@ -1,189 +1,189 @@
--rw-r--r--   0        0        0     1939 1970-01-01 00:00:00.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/Cargo.toml
--rw-r--r--   0     1001      123     1345 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/.github/workflows/gh-pages.yml
--rw-r--r--   0     1001      123      330 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/.github/workflows/paper-compile.yml
--rw-r--r--   0     1001      123     1512 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/.github/workflows/python.yml
--rw-r--r--   0     1001      123      320 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/.gitignore
--rw-r--r--   0     1001      123    57725 2023-06-15 01:05:00.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/Cargo.lock
--rw-r--r--   0     1001      123    35149 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/LICENSE
--rw-r--r--   0     1001      123      708 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/README.md
--rw-r--r--   0     1001      123        5 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/.gitignore
--rw-r--r--   0     1001      123      264 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/README.md
--rw-r--r--   0     1001      123      110 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/book.toml
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/hit3d-utils-exe
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/hit3d.x
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/plots/energy_helicity.py
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/plots/proposal_plots.py
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/plots/viscous_dissapation.py
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/vtk-analysis-exe
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/example_jobset_name_build_ouput-node-1.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/example_jobset_name_build_ouput-node-2.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/example_jobset_name_build_ouput-node-3.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/job_1/stdout.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/job_2/stdout.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/job_3/stdout.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/example_jobset_name_build_ouput-node-1.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/example_jobset_name_build_ouput-node-2.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/example_jobset_name_build_ouput-node-3.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/job_1/stdout.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/job_2/stdout.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/job_3/stdout.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/pull/README.md
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/README.md
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case1/flowfield.vtk
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case1/statistics.csv
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case2/flowfield.vtk
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case2/statistics.csv
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case3/flowfield.vtk
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case3/statistics.csv
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/python-root-folder-structure/STREAmS/README.md
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/python-root-folder-structure/STREAmS/src/main.f90
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/python-root-folder-structure/build.py
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/python-root-folder-structure/initial_files/file1.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/python-root-folder-structure/initial_files/file2.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/python-root-folder-structure/input/file1.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/python-root-folder-structure/input/file2.txt
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/examples/python-root-folder-structure/input/file3.txt
--rw-r--r--   0     1001      123     9012 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/figs/apptainer_config_flowchart.svg
--rw-r--r--   0     1001      123   286904 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/figs/architecture.png
--rw-r--r--   0     1001      123   896850 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/figs/architecture.xcf
--rw-r--r--   0     1001      123    14375 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/figs/input_outputs.svg
--rw-r--r--   0     1001      123    15607 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/figs/state_machine.svg
--rw-r--r--   0     1001      123     1012 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/SUMMARY.md
--rw-r--r--   0     1001      123     1030 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/admin_setup.md
--rw-r--r--   0     1001      123     2155 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/apptainer-input-files.md
--rw-r--r--   0     1001      123     4603 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/apptainer-introduction.md
--rw-r--r--   0     1001      123     1946 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/apptainer-mutable-filesystem.md
--rw-r--r--   0     1001      123      460 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/apptainer-packaging-solvers.md
--rw-r--r--   0     1001      123     3440 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/apptainer-running-locally.md
--rw-r--r--   0     1001      123      642 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/apptainer-storing-results.md
--rw-r--r--   0     1001      123     6225 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/apptainer.md
--rw-r--r--   0     1001      123      682 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/capabilities.md
--rw-r--r--   0     1001      123     8641 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/commands.md
--rw-r--r--   0     1001      123     1405 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/compute_node_setup.md
--rw-r--r--   0     1001      123     7642 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/configuration.md
--rw-r--r--   0     1001      123    93139 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/figs/apptainer_config_flowchart.png
--rw-r--r--   0     1001      123    63775 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/figs/input_outputs.png
--rw-r--r--   0     1001      123     1848 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/head_node_setup.md
--rw-r--r--   0     1001      123      613 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/install.md
--rw-r--r--   0     1001      123     3417 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/introduction.md
--rw-r--r--   0     1001      123     1589 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/overview.md
--rw-r--r--   0     1001      123     1628 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/python-build-scripts.md
--rw-r--r--   0     1001      123     3378 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/python-execution-scripts.md
--rw-r--r--   0     1001      123      176 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/python-full-example.md
--rw-r--r--   0     1001      123     3142 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/python-input-files.md
--rw-r--r--   0     1001      123     1033 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/python-storing-results.md
--rw-r--r--   0     1001      123     5566 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/python.md
--rw-r--r--   0     1001      123      367 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/python_api.md
--rw-r--r--   0     1001      123      682 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/examples/apptainer/build.apptainer
--rw-r--r--   0     1001      123      693 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/examples/apptainer/build.py
--rw-r--r--   0     1001      123       50 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/examples/apptainer/dataset_always.csv
--rw-r--r--   0     1001      123       50 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/examples/apptainer/dataset_sometimes.csv
--rw-r--r--   0     1001      123      481 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/examples/apptainer/distribute-jobs.yaml
--rw-r--r--   0     1001      123      956 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/examples/apptainer/run.py
--rw-r--r--   0     1001      123      693 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/examples/python/build.py
--rw-r--r--   0     1001      123       50 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/examples/python/dataset_always.csv
--rw-r--r--   0     1001      123       50 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/examples/python/dataset_sometimes.csv
--rw-r--r--   0     1001      123      543 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/examples/python/distribute-jobs.yaml
--rw-r--r--   0     1001      123      921 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/examples/python/run.py
--rw-r--r--   0     1001      123      404 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/install/distribute-compute.service
--rw-r--r--   0     1001      123      510 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/install/distribute-server.service
--rw-r--r--   0     1001      123      470 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/install/setup-root.sh
--rw-r--r--   0     1001      123      699 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/install/setup.sh
--rw-r--r--   0     1001      123      219 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/install/update.sh
--rw-r--r--   0     1001      123      323 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/justfile
--rw-r--r--   0     1001      123    63775 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/paper/input_outputs.png
--rw-r--r--   0     1001      123    67552 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/paper/node_layout.png
--rw-r--r--   0     1001      123    18914 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/paper/node_layout.svg
--rw-r--r--   0     1001      123     1420 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/paper/paper.bib
--rw-r--r--   0     1001      123     6333 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/paper/paper.md
--rw-r--r--   0     1001      123     4357 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/add.rs
--rw-r--r--   0     1001      123     2991 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/bin/distribute.rs
--rw-r--r--   0     1001      123     9727 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/cli.rs
--rw-r--r--   0     1001      123    13238 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/client/execute.rs
--rw-r--r--   0     1001      123    14350 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/client/mod.rs
--rw-r--r--   0     1001      123     7240 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/client/utils.rs
--rw-r--r--   0     1001      123     8290 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/config/apptainer.rs
--rw-r--r--   0     1001      123     7181 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/config/common.rs
--rw-r--r--   0     1001      123     2677 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/config/hashing.rs
--rw-r--r--   0     1001      123    21876 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/config/mod.rs
--rw-r--r--   0     1001      123     7562 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/config/python.rs
--rw-r--r--   0     1001      123     2650 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/config/requirements.rs
--rw-r--r--   0     1001      123    16061 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/error.rs
--rw-r--r--   0     1001      123      648 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/kill.rs
--rw-r--r--   0     1001      123     6327 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/lib.rs
--rw-r--r--   0     1001      123     1993 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/node_status.rs
--rw-r--r--   0     1001      123     5782 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/pause/mod.rs
--rw-r--r--   0     1001      123     8185 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/pause/unix.rs
--rw-r--r--   0     1001      123     1221 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/prelude.rs
--rw-r--r--   0     1001      123    11560 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/built.rs
--rw-r--r--   0     1001      123    10356 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/compiling.rs
--rw-r--r--   0     1001      123    24595 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/executing.rs
--rw-r--r--   0     1001      123     9723 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/mod.rs
--rw-r--r--   0     1001      123     8065 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/prepare_build.rs
--rw-r--r--   0     1001      123     7655 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/send_files/mod.rs
--rw-r--r--   0     1001      123    13968 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/send_files/receiver.rs
--rw-r--r--   0     1001      123    13724 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/send_files/sender.rs
--rw-r--r--   0     1001      123    12649 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/uninit.rs
--rw-r--r--   0     1001      123     6599 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/pull.rs
--rw-r--r--   0     1001      123     2089 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/run_local.rs
--rw-r--r--   0     1001      123     5820 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/job_pool.rs
--rw-r--r--   0     1001      123     1587 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/matrix.rs
--rw-r--r--   0     1001      123     5646 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/mod.rs
--rw-r--r--   0     1001      123    14370 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/node.rs
--rw-r--r--   0     1001      123     7584 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/pool_data.rs
--rw-r--r--   0     1001      123    34089 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/schedule.rs
--rw-r--r--   0     1001      123    23451 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/user_conn.rs
--rw-r--r--   0     1001      123     4624 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/server_status.rs
--rw-r--r--   0     1001      123    11657 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/slurm.rs
--rw-r--r--   0     1001      123     3413 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/template.rs
--rw-r--r--   0     1001      123    21028 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/src/transport.rs
--rw-r--r--   0     1001      123     1761 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/static/example-jobs-apptainer.yaml
--rw-r--r--   0     1001      123     2232 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/static/example-jobs-python.yaml
--rw-r--r--   0     1001      123      614 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/static/example-nodes.yaml
--rw-r--r--   0     1001      123      165 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/apptainer_local/apptainer_local.apt
--rw-r--r--   0     1001      123      447 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/apptainer_local/build.sh
--rw-r--r--   0     1001      123      686 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/apptainer_local/distribute-jobs.yaml
--rw-r--r--   0     1001      123       69 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/apptainer_local/hello.txt
--rw-r--r--   0     1001      123        3 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/apptainer_local/input_1.txt
--rw-r--r--   0     1001      123        3 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/apptainer_local/input_2.txt
--rw-r--r--   0     1001      123      715 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/apptainer_local/run.py
--rw-r--r--   0     1001      123     3528 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/apptainer_local.rs
--rw-r--r--   0     1001      123      695 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/cancel_job/distribute-jobs.yaml
--rw-r--r--   0     1001      123      117 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/cancel_job/distribute-nodes.yaml
--rw-r--r--   0     1001      123     4158 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/cancel_job.rs
--rw-r--r--   0     1001      123      117 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/check_deallocate_jobs/distribute-nodes.yaml
--rw-r--r--   0     1001      123     5304 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/check_deallocate_jobs.rs
--rw-r--r--   0     1001      123      242 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/check_pull/distribute-jobs.yaml
--rw-r--r--   0     1001      123       10 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/check_pull/distribute-nodes.yaml
--rw-r--r--   0     1001      123     6073 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/check_pull.rs
--rw-r--r--   0     1001      123      309 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/failed_keepalive/distribute-jobs.yaml
--rw-r--r--   0     1001      123      117 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/failed_keepalive/distribute-nodes.yaml
--rw-r--r--   0     1001      123     4939 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/failed_keepalive.rs
--rw-r--r--   0     1001      123      141 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/filter_files/README.md
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/filter_files/nested_folder/another_file.txt
--rw-r--r--   0     1001      123      396 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/many_jobsets_single_sif/distribute-jobs.yaml
--rw-r--r--   0     1001      123      117 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/many_jobsets_single_sif/distribute-nodes.yaml
--rw-r--r--   0     1001      123     7320 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/many_jobsets_single_sif.rs
--rw-r--r--   0     1001      123      242 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/pull_large_file/distribute-jobs.yaml
--rw-r--r--   0     1001      123       10 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/pull_large_file/distribute-nodes.yaml
--rw-r--r--   0     1001      123        0 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/python_sleep/build.py
--rw-r--r--   0     1001      123       29 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/python_sleep/sleep30s.py
--rw-r--r--   0     1001      123       30 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/tests/python_sleep/sleep500s.py
--rwxr-xr-x   0     1001      123      523 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/local_dependencies/distribute/update_python_version.sh
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 distribute_compute_config-0.14.4/Cargo.toml
--rw-r--r--   0     1001      123      162 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/.readthedocs.yaml
--rw-r--r--   0     1001      123       80 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/MANIFEST.in
--rw-r--r--   0     1001      123      605 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/README.md
--rw-r--r--   0     1001      123     1233 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/distribute_compute_config.pyi
--rw-r--r--   0     1001      123      638 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/docs/Makefile
--rw-r--r--   0     1001      123      804 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/docs/make.bat
--rw-r--r--   0     1001      123     1542 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/docs/source/api.rst
--rw-r--r--   0     1001      123     1923 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/docs/source/conf.py
--rw-r--r--   0     1001      123     3545 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/docs/source/example.rst
--rw-r--r--   0     1001      123      836 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/docs/source/index.rst
--rw-r--r--   0     1001      123      176 2023-06-15 01:03:04.000000 distribute_compute_config-0.14.4/pyproject.toml
--rw-r--r--   0     1001      123    14869 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/src/lib.rs
--rw-r--r--   0     1001      123     2307 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/src/validate_bindings.py
--rw-r--r--   0     1001      123     2082 2023-06-15 01:02:59.000000 distribute_compute_config-0.14.4/src/wrap.rs
--rw-r--r--   0     1001      123    17765 2023-06-15 01:04:59.000000 distribute_compute_config-0.14.4/Cargo.lock
--rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 distribute_compute_config-0.14.4/PKG-INFO
+-rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/Cargo.toml
+-rw-r--r--   0     1001      123     1345 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/.github/workflows/gh-pages.yml
+-rw-r--r--   0     1001      123      330 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/.github/workflows/paper-compile.yml
+-rw-r--r--   0     1001      123     1512 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/.github/workflows/python.yml
+-rw-r--r--   0     1001      123      320 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/.gitignore
+-rw-r--r--   0     1001      123    58205 2023-06-15 23:15:11.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/Cargo.lock
+-rw-r--r--   0     1001      123    35149 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/LICENSE
+-rw-r--r--   0     1001      123      708 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/README.md
+-rw-r--r--   0     1001      123        5 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/.gitignore
+-rw-r--r--   0     1001      123      264 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/README.md
+-rw-r--r--   0     1001      123      110 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/book.toml
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/hit3d-utils-exe
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/hit3d.x
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/plots/energy_helicity.py
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/plots/proposal_plots.py
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/plots/viscous_dissapation.py
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/apptainer-hit3d-example/vtk-analysis-exe
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/example_jobset_name_build_ouput-node-1.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/example_jobset_name_build_ouput-node-2.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/example_jobset_name_build_ouput-node-3.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/job_1/stdout.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/job_2/stdout.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_01/job_3/stdout.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/example_jobset_name_build_ouput-node-1.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/example_jobset_name_build_ouput-node-2.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/example_jobset_name_build_ouput-node-3.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/job_1/stdout.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/job_2/stdout.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/config-folder-structure/example_namespace/job_batch_02/job_3/stdout.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/pull/README.md
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/README.md
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case1/flowfield.vtk
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case1/statistics.csv
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case2/flowfield.vtk
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case2/statistics.csv
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case3/flowfield.vtk
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/pull/brooks_openfoam_cases/incompressible_5second_cases/case3/statistics.csv
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/python-root-folder-structure/STREAmS/README.md
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/python-root-folder-structure/STREAmS/src/main.f90
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/python-root-folder-structure/build.py
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/python-root-folder-structure/initial_files/file1.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/python-root-folder-structure/initial_files/file2.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/python-root-folder-structure/input/file1.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/python-root-folder-structure/input/file2.txt
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/examples/python-root-folder-structure/input/file3.txt
+-rw-r--r--   0     1001      123     9012 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/figs/apptainer_config_flowchart.svg
+-rw-r--r--   0     1001      123   286904 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/figs/architecture.png
+-rw-r--r--   0     1001      123   896850 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/figs/architecture.xcf
+-rw-r--r--   0     1001      123    14375 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/figs/input_outputs.svg
+-rw-r--r--   0     1001      123    15607 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/figs/state_machine.svg
+-rw-r--r--   0     1001      123     1012 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/SUMMARY.md
+-rw-r--r--   0     1001      123     1030 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/admin_setup.md
+-rw-r--r--   0     1001      123     2155 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/apptainer-input-files.md
+-rw-r--r--   0     1001      123     4603 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/apptainer-introduction.md
+-rw-r--r--   0     1001      123     1946 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/apptainer-mutable-filesystem.md
+-rw-r--r--   0     1001      123      460 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/apptainer-packaging-solvers.md
+-rw-r--r--   0     1001      123     3440 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/apptainer-running-locally.md
+-rw-r--r--   0     1001      123      642 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/apptainer-storing-results.md
+-rw-r--r--   0     1001      123     6225 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/apptainer.md
+-rw-r--r--   0     1001      123      682 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/capabilities.md
+-rw-r--r--   0     1001      123     8641 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/commands.md
+-rw-r--r--   0     1001      123     1405 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/compute_node_setup.md
+-rw-r--r--   0     1001      123     7642 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/configuration.md
+-rw-r--r--   0     1001      123    93139 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/figs/apptainer_config_flowchart.png
+-rw-r--r--   0     1001      123    63775 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/figs/input_outputs.png
+-rw-r--r--   0     1001      123     1848 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/head_node_setup.md
+-rw-r--r--   0     1001      123      613 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/install.md
+-rw-r--r--   0     1001      123     3417 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/introduction.md
+-rw-r--r--   0     1001      123     1589 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/overview.md
+-rw-r--r--   0     1001      123     1628 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/python-build-scripts.md
+-rw-r--r--   0     1001      123     3378 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/python-execution-scripts.md
+-rw-r--r--   0     1001      123      176 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/python-full-example.md
+-rw-r--r--   0     1001      123     3142 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/python-input-files.md
+-rw-r--r--   0     1001      123     1033 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/python-storing-results.md
+-rw-r--r--   0     1001      123     5566 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/python.md
+-rw-r--r--   0     1001      123      367 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/python_api.md
+-rw-r--r--   0     1001      123      682 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/examples/apptainer/build.apptainer
+-rw-r--r--   0     1001      123      693 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/examples/apptainer/build.py
+-rw-r--r--   0     1001      123       50 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/examples/apptainer/dataset_always.csv
+-rw-r--r--   0     1001      123       50 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/examples/apptainer/dataset_sometimes.csv
+-rw-r--r--   0     1001      123      481 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/examples/apptainer/distribute-jobs.yaml
+-rw-r--r--   0     1001      123      956 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/examples/apptainer/run.py
+-rw-r--r--   0     1001      123      693 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/examples/python/build.py
+-rw-r--r--   0     1001      123       50 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/examples/python/dataset_always.csv
+-rw-r--r--   0     1001      123       50 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/examples/python/dataset_sometimes.csv
+-rw-r--r--   0     1001      123      543 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/examples/python/distribute-jobs.yaml
+-rw-r--r--   0     1001      123      921 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/examples/python/run.py
+-rw-r--r--   0     1001      123      404 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/install/distribute-compute.service
+-rw-r--r--   0     1001      123      510 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/install/distribute-server.service
+-rw-r--r--   0     1001      123      470 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/install/setup-root.sh
+-rw-r--r--   0     1001      123      699 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/install/setup.sh
+-rw-r--r--   0     1001      123      219 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/install/update.sh
+-rw-r--r--   0     1001      123      323 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/justfile
+-rw-r--r--   0     1001      123    63775 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/paper/input_outputs.png
+-rw-r--r--   0     1001      123    67552 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/paper/node_layout.png
+-rw-r--r--   0     1001      123    18914 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/paper/node_layout.svg
+-rw-r--r--   0     1001      123     1420 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/paper/paper.bib
+-rw-r--r--   0     1001      123     6333 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/paper/paper.md
+-rw-r--r--   0     1001      123     4357 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/add.rs
+-rw-r--r--   0     1001      123     3074 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/bin/distribute.rs
+-rw-r--r--   0     1001      123     9727 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/cli.rs
+-rw-r--r--   0     1001      123    13238 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/client/execute.rs
+-rw-r--r--   0     1001      123    14350 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/client/mod.rs
+-rw-r--r--   0     1001      123     7240 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/client/utils.rs
+-rw-r--r--   0     1001      123     8290 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/config/apptainer.rs
+-rw-r--r--   0     1001      123     7181 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/config/common.rs
+-rw-r--r--   0     1001      123     2677 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/config/hashing.rs
+-rw-r--r--   0     1001      123    21876 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/config/mod.rs
+-rw-r--r--   0     1001      123     7562 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/config/python.rs
+-rw-r--r--   0     1001      123     2650 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/config/requirements.rs
+-rw-r--r--   0     1001      123    16061 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/error.rs
+-rw-r--r--   0     1001      123      648 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/kill.rs
+-rw-r--r--   0     1001      123     6327 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/lib.rs
+-rw-r--r--   0     1001      123     1993 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/node_status.rs
+-rw-r--r--   0     1001      123     5782 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/pause/mod.rs
+-rw-r--r--   0     1001      123     8185 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/pause/unix.rs
+-rw-r--r--   0     1001      123     1221 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/prelude.rs
+-rw-r--r--   0     1001      123    11560 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/built.rs
+-rw-r--r--   0     1001      123    10356 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/compiling.rs
+-rw-r--r--   0     1001      123    24595 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/executing.rs
+-rw-r--r--   0     1001      123     9723 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/mod.rs
+-rw-r--r--   0     1001      123     8065 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/prepare_build.rs
+-rw-r--r--   0     1001      123     7655 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/send_files/mod.rs
+-rw-r--r--   0     1001      123    13968 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/send_files/receiver.rs
+-rw-r--r--   0     1001      123    13724 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/send_files/sender.rs
+-rw-r--r--   0     1001      123    12649 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/uninit.rs
+-rw-r--r--   0     1001      123     6599 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/pull.rs
+-rw-r--r--   0     1001      123     2089 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/run_local.rs
+-rw-r--r--   0     1001      123     5820 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/job_pool.rs
+-rw-r--r--   0     1001      123     1587 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/matrix.rs
+-rw-r--r--   0     1001      123     5646 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/mod.rs
+-rw-r--r--   0     1001      123    14370 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/node.rs
+-rw-r--r--   0     1001      123     7584 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/pool_data.rs
+-rw-r--r--   0     1001      123    34089 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/schedule.rs
+-rw-r--r--   0     1001      123    23451 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/user_conn.rs
+-rw-r--r--   0     1001      123     4624 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/server_status.rs
+-rw-r--r--   0     1001      123    11657 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/slurm.rs
+-rw-r--r--   0     1001      123     3413 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/template.rs
+-rw-r--r--   0     1001      123    21028 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/src/transport.rs
+-rw-r--r--   0     1001      123     1761 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/static/example-jobs-apptainer.yaml
+-rw-r--r--   0     1001      123     2232 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/static/example-jobs-python.yaml
+-rw-r--r--   0     1001      123      614 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/static/example-nodes.yaml
+-rw-r--r--   0     1001      123      165 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/apptainer_local/apptainer_local.apt
+-rw-r--r--   0     1001      123      447 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/apptainer_local/build.sh
+-rw-r--r--   0     1001      123      686 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/apptainer_local/distribute-jobs.yaml
+-rw-r--r--   0     1001      123       69 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/apptainer_local/hello.txt
+-rw-r--r--   0     1001      123        3 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/apptainer_local/input_1.txt
+-rw-r--r--   0     1001      123        3 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/apptainer_local/input_2.txt
+-rw-r--r--   0     1001      123      715 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/apptainer_local/run.py
+-rw-r--r--   0     1001      123     3528 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/apptainer_local.rs
+-rw-r--r--   0     1001      123      695 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/cancel_job/distribute-jobs.yaml
+-rw-r--r--   0     1001      123      117 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/cancel_job/distribute-nodes.yaml
+-rw-r--r--   0     1001      123     4158 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/cancel_job.rs
+-rw-r--r--   0     1001      123      117 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/check_deallocate_jobs/distribute-nodes.yaml
+-rw-r--r--   0     1001      123     5304 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/check_deallocate_jobs.rs
+-rw-r--r--   0     1001      123      242 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/check_pull/distribute-jobs.yaml
+-rw-r--r--   0     1001      123       10 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/check_pull/distribute-nodes.yaml
+-rw-r--r--   0     1001      123     6073 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/check_pull.rs
+-rw-r--r--   0     1001      123      309 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/failed_keepalive/distribute-jobs.yaml
+-rw-r--r--   0     1001      123      117 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/failed_keepalive/distribute-nodes.yaml
+-rw-r--r--   0     1001      123     4939 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/failed_keepalive.rs
+-rw-r--r--   0     1001      123      141 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/filter_files/README.md
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/filter_files/nested_folder/another_file.txt
+-rw-r--r--   0     1001      123      396 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/many_jobsets_single_sif/distribute-jobs.yaml
+-rw-r--r--   0     1001      123      117 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/many_jobsets_single_sif/distribute-nodes.yaml
+-rw-r--r--   0     1001      123     7320 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/many_jobsets_single_sif.rs
+-rw-r--r--   0     1001      123      242 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/pull_large_file/distribute-jobs.yaml
+-rw-r--r--   0     1001      123       10 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/pull_large_file/distribute-nodes.yaml
+-rw-r--r--   0     1001      123        0 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/python_sleep/build.py
+-rw-r--r--   0     1001      123       29 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/python_sleep/sleep30s.py
+-rw-r--r--   0     1001      123       30 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/tests/python_sleep/sleep500s.py
+-rwxr-xr-x   0     1001      123      523 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/local_dependencies/distribute/update_python_version.sh
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 distribute_compute_config-0.14.5/Cargo.toml
+-rw-r--r--   0     1001      123      162 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/.readthedocs.yaml
+-rw-r--r--   0     1001      123       80 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/MANIFEST.in
+-rw-r--r--   0     1001      123      605 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/README.md
+-rw-r--r--   0     1001      123     1233 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/distribute_compute_config.pyi
+-rw-r--r--   0     1001      123      638 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/docs/Makefile
+-rw-r--r--   0     1001      123      804 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/docs/make.bat
+-rw-r--r--   0     1001      123     1542 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/docs/source/api.rst
+-rw-r--r--   0     1001      123     1923 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/docs/source/conf.py
+-rw-r--r--   0     1001      123     3545 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/docs/source/example.rst
+-rw-r--r--   0     1001      123      836 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/docs/source/index.rst
+-rw-r--r--   0     1001      123      176 2023-06-15 23:15:03.000000 distribute_compute_config-0.14.5/pyproject.toml
+-rw-r--r--   0     1001      123    14869 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/src/lib.rs
+-rw-r--r--   0     1001      123     2307 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/src/validate_bindings.py
+-rw-r--r--   0     1001      123     2082 2023-06-15 23:15:00.000000 distribute_compute_config-0.14.5/src/wrap.rs
+-rw-r--r--   0     1001      123    17765 2023-06-15 23:15:09.000000 distribute_compute_config-0.14.5/Cargo.lock
+-rw-r--r--   0        0        0      755 1970-01-01 00:00:00.000000 distribute_compute_config-0.14.5/PKG-INFO
```

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/Cargo.toml` & `distribute_compute_config-0.14.5/local_dependencies/distribute/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "distribute"
-version = "0.14.4"
+version = "0.14.5"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 crate-type = ["cdylib", "rlib"]
 
 [dependencies]
@@ -25,28 +25,29 @@
 signal-hook = { version = "0.3.9", default_features = false, optional = true }
 regex = { version = "1.8.4", optional = true }
 clap = { version = "4.3.4", features = ["derive"], optional = true }
 base16 = "0.2.1"
 tracing = { version = "0.1.37", optional = true }
 tracing-subscriber = { version = "0.3.17", features = ["time", "std", "local-time"], optional = true }
 getset = "0.1.2"
+mimalloc = { version = "0.1.37", optional = true }
 
 [dependencies.matrix-notify]
 default_features = false
 git = "https://github.com/fluid-Dynamics-Group/matrix-notify"
 rev = "d88dd6518ec3ce1e5bb1992ecf1e229be5b98016"
 
 [dependencies.pyo3]
 version = "0.17.3" 
 features = ["extension-module"]
 optional = true
 
 [features]
 default = ["cli"]
-cli = ["clap", "regex", "signal-hook", "sha1", "tokio-stream", "num_cpus", "nix", "futures", "chrono", "tokio", "walkdir", "bincode", "matrix-notify/cli", "tracing", "tracing-subscriber"]
+cli = ["clap", "regex", "signal-hook", "sha1", "tokio-stream", "num_cpus", "nix", "futures", "chrono", "tokio", "walkdir", "bincode", "matrix-notify/cli", "tracing", "tracing-subscriber", "mimalloc"]
 python = ["pyo3", "matrix-notify/userid"]
 config = ["matrix-notify/userid"]
 
 [[bin]]
 name = "distribute"
 required-features = ["cli"]
```

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/.github/workflows/gh-pages.yml` & `distribute_compute_config-0.14.5/local_dependencies/distribute/.github/workflows/gh-pages.yml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/.github/workflows/python.yml` & `distribute_compute_config-0.14.5/local_dependencies/distribute/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/Cargo.lock` & `distribute_compute_config-0.14.5/local_dependencies/distribute/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -346,24 +346,25 @@
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
 name = "distribute"
-version = "0.14.4"
+version = "0.14.5"
 dependencies = [
  "base16",
  "bincode",
  "chrono",
  "clap",
  "derive_more",
  "futures",
  "getset",
  "matrix-notify",
+ "mimalloc",
  "nix",
  "num_cpus",
  "pyo3",
  "regex",
  "serde",
  "serde_json",
  "serde_yaml",
@@ -807,14 +808,24 @@
 [[package]]
 name = "libc"
 version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
+name = "libmimalloc-sys"
+version = "0.1.33"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f4ac0e912c8ef1b735e92369695618dc5b1819f5a7bf3f167301a3ba1cea515e"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
@@ -879,14 +890,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "mimalloc"
+version = "0.1.37"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e2894987a3459f3ffb755608bd82188f8ed00d0ae077f1edea29c068d639d98"
+dependencies = [
+ "libmimalloc-sys",
+]
+
+[[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "mime_guess"
```

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/LICENSE` & `distribute_compute_config-0.14.5/local_dependencies/distribute/LICENSE`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/README.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/README.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/figs/apptainer_config_flowchart.svg` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/figs/apptainer_config_flowchart.svg`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/figs/architecture.png` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/figs/architecture.png`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/figs/architecture.xcf` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/figs/architecture.xcf`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/figs/input_outputs.svg` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/figs/input_outputs.svg`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/figs/state_machine.svg` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/figs/state_machine.svg`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/SUMMARY.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/SUMMARY.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/admin_setup.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/admin_setup.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/apptainer-input-files.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/apptainer-input-files.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/apptainer-introduction.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/apptainer-introduction.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/apptainer-mutable-filesystem.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/apptainer-mutable-filesystem.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/apptainer-running-locally.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/apptainer-running-locally.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/apptainer-storing-results.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/apptainer-storing-results.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/apptainer.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/apptainer.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/capabilities.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/capabilities.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/commands.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/commands.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/compute_node_setup.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/compute_node_setup.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/configuration.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/configuration.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/figs/apptainer_config_flowchart.png` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/figs/apptainer_config_flowchart.png`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/figs/input_outputs.png` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/figs/input_outputs.png`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/head_node_setup.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/head_node_setup.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/install.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/install.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/introduction.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/introduction.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/overview.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/overview.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/python-build-scripts.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/python-build-scripts.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/python-execution-scripts.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/python-execution-scripts.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/python-input-files.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/python-input-files.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/python-storing-results.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/python-storing-results.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/docs/src/python.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/docs/src/python.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/examples/apptainer/build.apptainer` & `distribute_compute_config-0.14.5/local_dependencies/distribute/examples/apptainer/build.apptainer`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/examples/apptainer/build.py` & `distribute_compute_config-0.14.5/local_dependencies/distribute/examples/apptainer/build.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/examples/apptainer/run.py` & `distribute_compute_config-0.14.5/local_dependencies/distribute/examples/apptainer/run.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/examples/python/build.py` & `distribute_compute_config-0.14.5/local_dependencies/distribute/examples/python/build.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/examples/python/distribute-jobs.yaml` & `distribute_compute_config-0.14.5/local_dependencies/distribute/examples/python/distribute-jobs.yaml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/examples/python/run.py` & `distribute_compute_config-0.14.5/local_dependencies/distribute/examples/python/run.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/install/setup.sh` & `distribute_compute_config-0.14.5/local_dependencies/distribute/install/setup.sh`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/paper/input_outputs.png` & `distribute_compute_config-0.14.5/local_dependencies/distribute/paper/input_outputs.png`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/paper/node_layout.png` & `distribute_compute_config-0.14.5/local_dependencies/distribute/paper/node_layout.png`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/paper/node_layout.svg` & `distribute_compute_config-0.14.5/local_dependencies/distribute/paper/node_layout.svg`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/paper/paper.bib` & `distribute_compute_config-0.14.5/local_dependencies/distribute/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/paper/paper.md` & `distribute_compute_config-0.14.5/local_dependencies/distribute/paper/paper.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/add.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/add.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/bin/distribute.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/bin/distribute.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 use distribute::cli;
 use distribute::Error;
 use std::fs;
 
 use clap::Parser;
 
+use mimalloc::MiMalloc;
+
+#[global_allocator]
+static GLOBAL: MiMalloc = MiMalloc;
+
+
 #[tokio::main(flavor = "multi_thread", worker_threads = 4)]
 async fn main() {
     if let Err(e) = wrap_main().await {
         println!("{}", e);
     }
 }
```

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/cli.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/cli.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/client/execute.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/client/execute.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/client/mod.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/client/mod.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/client/utils.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/client/utils.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/config/apptainer.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/config/apptainer.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/config/common.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/config/common.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/config/hashing.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/config/hashing.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/config/mod.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/config/mod.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/config/python.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/config/python.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/config/requirements.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/config/requirements.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/error.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/error.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/kill.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/kill.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/lib.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/lib.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/node_status.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/node_status.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/pause/mod.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/pause/mod.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/pause/unix.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/pause/unix.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/prelude.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/built.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/built.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/compiling.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/compiling.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/executing.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/executing.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/mod.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/mod.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/prepare_build.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/prepare_build.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/send_files/mod.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/send_files/mod.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/send_files/receiver.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/send_files/receiver.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/send_files/sender.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/send_files/sender.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/protocol/uninit.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/protocol/uninit.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/pull.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/pull.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/run_local.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/run_local.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/job_pool.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/job_pool.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/matrix.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/matrix.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/mod.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/mod.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/node.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/node.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/pool_data.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/pool_data.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/schedule.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/schedule.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/server/user_conn.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/server/user_conn.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/server_status.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/server_status.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/slurm.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/slurm.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/template.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/template.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/src/transport.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/src/transport.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/static/example-jobs-apptainer.yaml` & `distribute_compute_config-0.14.5/local_dependencies/distribute/static/example-jobs-apptainer.yaml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/static/example-jobs-python.yaml` & `distribute_compute_config-0.14.5/local_dependencies/distribute/static/example-jobs-python.yaml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/static/example-nodes.yaml` & `distribute_compute_config-0.14.5/local_dependencies/distribute/static/example-nodes.yaml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/tests/apptainer_local/distribute-jobs.yaml` & `distribute_compute_config-0.14.5/local_dependencies/distribute/tests/apptainer_local/distribute-jobs.yaml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/tests/apptainer_local/run.py` & `distribute_compute_config-0.14.5/local_dependencies/distribute/tests/apptainer_local/run.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/tests/apptainer_local.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/tests/apptainer_local.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/tests/cancel_job/distribute-jobs.yaml` & `distribute_compute_config-0.14.5/local_dependencies/distribute/tests/cancel_job/distribute-jobs.yaml`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/tests/cancel_job.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/tests/cancel_job.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/tests/check_deallocate_jobs.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/tests/check_deallocate_jobs.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/tests/check_pull.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/tests/check_pull.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/tests/failed_keepalive.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/tests/failed_keepalive.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/tests/many_jobsets_single_sif.rs` & `distribute_compute_config-0.14.5/local_dependencies/distribute/tests/many_jobsets_single_sif.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/local_dependencies/distribute/update_python_version.sh` & `distribute_compute_config-0.14.5/local_dependencies/distribute/update_python_version.sh`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/README.md` & `distribute_compute_config-0.14.5/README.md`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/distribute_compute_config.pyi` & `distribute_compute_config-0.14.5/distribute_compute_config.pyi`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/docs/Makefile` & `distribute_compute_config-0.14.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/docs/make.bat` & `distribute_compute_config-0.14.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/docs/source/api.rst` & `distribute_compute_config-0.14.5/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/docs/source/conf.py` & `distribute_compute_config-0.14.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/docs/source/example.rst` & `distribute_compute_config-0.14.5/docs/source/example.rst`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/docs/source/index.rst` & `distribute_compute_config-0.14.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/src/lib.rs` & `distribute_compute_config-0.14.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/src/validate_bindings.py` & `distribute_compute_config-0.14.5/src/validate_bindings.py`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/src/wrap.rs` & `distribute_compute_config-0.14.5/src/wrap.rs`

 * *Files identical despite different names*

### Comparing `distribute_compute_config-0.14.4/Cargo.lock` & `distribute_compute_config-0.14.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
  "quote",
  "rustc_version",
  "syn 1.0.107",
 ]
 
 [[package]]
 name = "distribute"
-version = "0.14.4"
+version = "0.14.5"
 dependencies = [
  "base16",
  "derive_more",
  "getset",
  "matrix-notify",
  "pyo3",
  "serde",
```

### Comparing `distribute_compute_config-0.14.4/PKG-INFO` & `distribute_compute_config-0.14.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distribute_compute_config
-Version: 0.14.4
+Version: 0.14.5
 Summary: 
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # pybind
 
 Python bindings to `distribute` for automated creation of configuration files
```

