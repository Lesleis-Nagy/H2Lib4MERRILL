# -- test amatrix --
add_executable(test_amatrix test_amatrix.c)
target_include_directories(test_amatrix
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_amatrix h2lib)
add_test(NAME test_amatrix COMMAND test_amatrix)

# -- test ddcluster --
add_executable(test_ddcluster test_ddcluster.c)
target_include_directories(test_ddcluster
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_ddcluster h2lib)
add_test(NAME test_ddcluster COMMAND test_ddcluster)

# -- test eigen --
add_executable(test_eigen test_eigen.c)
target_include_directories(test_eigen
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_eigen h2lib)
add_test(NAME test_eigen COMMAND test_eigen)

# -- test h2compression --
add_executable(test_h2compression test_h2compression.c)
target_include_directories(test_h2compression
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_h2compression h2lib)
add_test(NAME test_h2compression COMMAND test_h2compression)

# -- test h2matrix --
add_executable(test_h2matrix test_h2matrix.c)
target_include_directories(test_h2matrix
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_h2matrix h2lib)
add_test(NAME test_h2matrix COMMAND test_h2matrix)

# -- test helmholtzbem3d --
add_executable(test_helmholtzbem3d test_helmholtzbem3d.c)
target_include_directories(test_helmholtzbem3d
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_helmholtzbem3d h2lib)
add_test(NAME test_helmholtzbem3d COMMAND test_helmholtzbem3d)

# -- test helmholtzbem3d_ocl --
add_executable(test_helmholtzbem3d_ocl test_helmholtzbem3d_ocl.c)
target_include_directories(test_helmholtzbem3d_ocl
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_helmholtzbem3d_ocl h2lib)
add_test(NAME test_helmholtzbem3d_ocl COMMAND test_helmholtzbem3d_ocl)

# -- test hmatrix --
add_executable(test_hmatrix test_hmatrix.c)
target_include_directories(test_hmatrix
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_hmatrix h2lib)
add_test(NAME test_hmatrix COMMAND test_hmatrix)

# -- test kernelmatrix --
add_executable(test_kernelmatrix test_kernelmatrix.c)
target_include_directories(test_kernelmatrix
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_kernelmatrix h2lib)
add_test(NAME test_kernelmatrix COMMAND test_kernelmatrix)

# -- test krylov --
add_executable(test_krylov test_krylov.c)
target_include_directories(test_krylov
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_krylov h2lib)
add_test(NAME test_krylov COMMAND test_krylov)

# -- test krylovsolvers --
add_executable(test_krylovsolvers test_krylovsolvers.c)
target_include_directories(test_krylovsolvers
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_krylovsolvers h2lib)
add_test(NAME test_krylovsolvers COMMAND test_krylovsolvers)

# -- test laplacebem2d --
add_executable(test_laplacebem2d test_laplacebem2d.c)
target_include_directories(test_laplacebem2d
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_laplacebem2d h2lib)
add_test(NAME test_laplacebem2d COMMAND test_laplacebem2d)

# -- test laplacebem3d --
add_executable(test_laplacebem3d test_laplacebem3d.c)
target_include_directories(test_laplacebem3d
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_laplacebem3d h2lib)
add_test(NAME test_laplacebem3d COMMAND test_laplacebem3d)

# -- test laplacebem3d_ocl --
add_executable(test_laplacebem3d_ocl test_laplacebem3d_ocl.c)
target_include_directories(test_laplacebem3d_ocl
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_laplacebem3d_ocl h2lib)
add_test(NAME test_laplacebem3d_ocl COMMAND test_laplacebem3d_ocl)

# -- test tet3d --
add_executable(test_tet3d test_tet3d.c)
target_include_directories(test_tet3d
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_tet3d h2lib)
add_test(NAME test_tet3d COMMAND test_tet3d)

# -- test tet3dp1 --
add_executable(test_tet3dp1 test_tet3dp1.c)
target_include_directories(test_tet3dp1
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_tet3dp1 h2lib)
add_test(NAME test_tet3dp1 COMMAND test_tet3dp1)

# -- test tet3drt0 --
add_executable(test_tet3drt0 test_tet3drt0.c)
target_include_directories(test_tet3drt0
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_tet3drt0 h2lib)
add_test(NAME test_tet3drt0 COMMAND test_tet3drt0)

# -- test tri2d --
add_executable(test_tri2d test_tri2d.c)
target_include_directories(test_tri2d
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_tri2d h2lib)
add_test(NAME test_tri2d COMMAND test_tri2d)

# -- test tri2dp1 --
add_executable(test_tri2dp1 test_tri2dp1.c)
target_include_directories(test_tri2dp1
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_tri2dp1 h2lib)
add_test(NAME test_tri2dp1 COMMAND test_tri2dp1)

# -- test tri2drt0 --
add_executable(test_tri2drt0 test_tri2drt0.c)
target_include_directories(test_tri2drt0
  PRIVATE ${H2LIB_INCLUDE_DIR})
target_link_libraries(test_tri2drt0 h2lib)
add_test(NAME test_tri2drt0 COMMAND test_tri2drt0)
