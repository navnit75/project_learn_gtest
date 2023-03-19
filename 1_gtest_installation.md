## GTEST Installation 
```bash
#1. Clone the repo first 
git clone https://github.com/google/googletest.git

#2. Cd to the cloned directory 
mkdir build
cmake ..
sudo make

#3. Copy all the library files build to /usr/lib/
cd lib
sudo cp * /usr/lib/

#4. Copy the gmock include files to /usr/local/include
cd ../../googlemock/include
cp -r gmock /usr/local/include/

#5. Copy the gtest include files to /usr/local/include
cd ../../googletest/include/
cp -r gtest /usr/local/include/
```

## Test Structure 
1. Arrange
    - Test Setup 
    - Set all input and preconditions 
2. Act
    - Call the method under test
3. Assert
    - Check that the results are correct 


## Appendix
1. Tree for the cloned file for the reference 
```bash
.
├── appveyor.yml
├── build
│   ├── CMakeCache.txt
│   ├── CMakeFiles
│   │   ├── 3.10.2
│   │   │   ├── CMakeCCompiler.cmake
│   │   │   ├── CMakeCXXCompiler.cmake
│   │   │   ├── CMakeDetermineCompilerABI_C.bin
│   │   │   ├── CMakeDetermineCompilerABI_CXX.bin
│   │   │   ├── CMakeSystem.cmake
│   │   │   ├── CompilerIdC
│   │   │   │   ├── a.out
│   │   │   │   ├── CMakeCCompilerId.c
│   │   │   │   └── tmp
│   │   │   └── CompilerIdCXX
│   │   │       ├── a.out
│   │   │       ├── CMakeCXXCompilerId.cpp
│   │   │       └── tmp
│   │   ├── cmake.check_cache
│   │   ├── CMakeDirectoryInformation.cmake
│   │   ├── CMakeError.log
│   │   ├── CMakeOutput.log
│   │   ├── CMakeTmp
│   │   ├── feature_tests.bin
│   │   ├── feature_tests.c
│   │   ├── feature_tests.cxx
│   │   ├── Makefile2
│   │   ├── Makefile.cmake
│   │   ├── progress.marks
│   │   └── TargetDirectories.txt
│   ├── cmake_install.cmake
│   ├── CTestTestfile.cmake
│   ├── googlemock
│   │   ├── CMakeFiles
│   │   │   ├── CMakeDirectoryInformation.cmake
│   │   │   ├── gmock.dir
│   │   │   │   ├── __
│   │   │   │   │   └── googletest
│   │   │   │   │       └── src
│   │   │   │   │           └── gtest-all.cc.o
│   │   │   │   ├── build.make
│   │   │   │   ├── cmake_clean.cmake
│   │   │   │   ├── cmake_clean_target.cmake
│   │   │   │   ├── CXX.includecache
│   │   │   │   ├── DependInfo.cmake
│   │   │   │   ├── depend.internal
│   │   │   │   ├── depend.make
│   │   │   │   ├── flags.make
│   │   │   │   ├── link.txt
│   │   │   │   ├── progress.make
│   │   │   │   └── src
│   │   │   │       └── gmock-all.cc.o
│   │   │   ├── gmock_main.dir
│   │   │   │   ├── __
│   │   │   │   │   └── googletest
│   │   │   │   │       └── src
│   │   │   │   │           └── gtest-all.cc.o
│   │   │   │   ├── build.make
│   │   │   │   ├── cmake_clean.cmake
│   │   │   │   ├── cmake_clean_target.cmake
│   │   │   │   ├── CXX.includecache
│   │   │   │   ├── DependInfo.cmake
│   │   │   │   ├── depend.internal
│   │   │   │   ├── depend.make
│   │   │   │   ├── flags.make
│   │   │   │   ├── link.txt
│   │   │   │   ├── progress.make
│   │   │   │   └── src
│   │   │   │       ├── gmock-all.cc.o
│   │   │   │       └── gmock_main.cc.o
│   │   │   └── progress.marks
│   │   ├── cmake_install.cmake
│   │   ├── CTestTestfile.cmake
│   │   ├── gtest
│   │   │   ├── CMakeFiles
│   │   │   │   ├── CMakeDirectoryInformation.cmake
│   │   │   │   ├── gtest.dir
│   │   │   │   │   ├── build.make
│   │   │   │   │   ├── cmake_clean.cmake
│   │   │   │   │   ├── cmake_clean_target.cmake
│   │   │   │   │   ├── CXX.includecache
│   │   │   │   │   ├── DependInfo.cmake
│   │   │   │   │   ├── depend.internal
│   │   │   │   │   ├── depend.make
│   │   │   │   │   ├── flags.make
│   │   │   │   │   ├── link.txt
│   │   │   │   │   ├── progress.make
│   │   │   │   │   └── src
│   │   │   │   │       └── gtest-all.cc.o
│   │   │   │   ├── gtest_main.dir
│   │   │   │   │   ├── build.make
│   │   │   │   │   ├── cmake_clean.cmake
│   │   │   │   │   ├── cmake_clean_target.cmake
│   │   │   │   │   ├── CXX.includecache
│   │   │   │   │   ├── DependInfo.cmake
│   │   │   │   │   ├── depend.internal
│   │   │   │   │   ├── depend.make
│   │   │   │   │   ├── flags.make
│   │   │   │   │   ├── link.txt
│   │   │   │   │   ├── progress.make
│   │   │   │   │   └── src
│   │   │   │   │       └── gtest_main.cc.o
│   │   │   │   └── progress.marks
│   │   │   ├── cmake_install.cmake
│   │   │   ├── CTestTestfile.cmake
│   │   │   ├── libgtest.a
│   │   │   ├── libgtest_main.a
│   │   │   └── Makefile
│   │   ├── libgmock.a
│   │   ├── libgmock_main.a
│   │   └── Makefile
│   ├── install_manifest.txt
│   └── Makefile
├── CMakeLists.txt
├── googlemock
│   ├── build-aux
│   ├── CHANGES
│   ├── CMakeLists.txt
│   ├── configure.ac
│   ├── CONTRIBUTORS
│   ├── docs
│   │   ├── CheatSheet.md
│   │   ├── CookBook.md
│   │   ├── DesignDoc.md
│   │   ├── DevGuide.md
│   │   ├── Documentation.md
│   │   ├── ForDummies.md
│   │   ├── FrequentlyAskedQuestions.md
│   │   ├── KnownIssues.md
│   │   ├── v1_5
│   │   │   ├── CheatSheet.md
│   │   │   ├── CookBook.md
│   │   │   ├── Documentation.md
│   │   │   ├── ForDummies.md
│   │   │   └── FrequentlyAskedQuestions.md
│   │   ├── v1_6
│   │   │   ├── CheatSheet.md
│   │   │   ├── CookBook.md
│   │   │   ├── Documentation.md
│   │   │   ├── ForDummies.md
│   │   │   └── FrequentlyAskedQuestions.md
│   │   └── v1_7
│   │       ├── CheatSheet.md
│   │       ├── CookBook.md
│   │       ├── Documentation.md
│   │       ├── ForDummies.md
│   │       └── FrequentlyAskedQuestions.md
│   ├── include
│   │   └── gmock
│   │       ├── gmock-actions.h
│   │       ├── gmock-cardinalities.h
│   │       ├── gmock-generated-actions.h
│   │       ├── gmock-generated-actions.h.pump
│   │       ├── gmock-generated-function-mockers.h
│   │       ├── gmock-generated-function-mockers.h.pump
│   │       ├── gmock-generated-matchers.h
│   │       ├── gmock-generated-matchers.h.pump
│   │       ├── gmock-generated-nice-strict.h
│   │       ├── gmock-generated-nice-strict.h.pump
│   │       ├── gmock.h
│   │       ├── gmock-matchers.h
│   │       ├── gmock-more-actions.h
│   │       ├── gmock-more-matchers.h
│   │       ├── gmock-spec-builders.h
│   │       └── internal
│   │           ├── custom
│   │           │   ├── gmock-generated-actions.h
│   │           │   ├── gmock-generated-actions.h.pump
│   │           │   ├── gmock-matchers.h
│   │           │   └── gmock-port.h
│   │           ├── gmock-generated-internal-utils.h
│   │           ├── gmock-generated-internal-utils.h.pump
│   │           ├── gmock-internal-utils.h
│   │           └── gmock-port.h
│   ├── LICENSE
│   ├── make
│   │   └── Makefile
│   ├── Makefile.am
│   ├── msvc
│   │   ├── 2005
│   │   │   ├── gmock_config.vsprops
│   │   │   ├── gmock_main.vcproj
│   │   │   ├── gmock.sln
│   │   │   ├── gmock_test.vcproj
│   │   │   └── gmock.vcproj
│   │   ├── 2010
│   │   │   ├── gmock_config.props
│   │   │   ├── gmock_main.vcxproj
│   │   │   ├── gmock.sln
│   │   │   ├── gmock_test.vcxproj
│   │   │   └── gmock.vcxproj
│   │   └── 2015
│   │       ├── gmock_config.props
│   │       ├── gmock_main.vcxproj
│   │       ├── gmock.sln
│   │       ├── gmock_test.vcxproj
│   │       └── gmock.vcxproj
│   ├── README.md
│   ├── scripts
│   │   ├── fuse_gmock_files.py
│   │   ├── generator
│   │   │   ├── cpp
│   │   │   │   ├── ast.py
│   │   │   │   ├── gmock_class.py
│   │   │   │   ├── gmock_class_test.py
│   │   │   │   ├── __init__.py
│   │   │   │   ├── keywords.py
│   │   │   │   ├── tokenize.py
│   │   │   │   └── utils.py
│   │   │   ├── gmock_gen.py
│   │   │   ├── LICENSE
│   │   │   ├── README
│   │   │   └── README.cppclean
│   │   ├── gmock-config.in
│   │   ├── gmock_doctor.py
│   │   ├── upload_gmock.py
│   │   └── upload.py
│   ├── src
│   │   ├── gmock-all.cc
│   │   ├── gmock-cardinalities.cc
│   │   ├── gmock.cc
│   │   ├── gmock-internal-utils.cc
│   │   ├── gmock_main.cc
│   │   ├── gmock-matchers.cc
│   │   └── gmock-spec-builders.cc
│   └── test
│       ├── gmock-actions_test.cc
│       ├── gmock_all_test.cc
│       ├── gmock-cardinalities_test.cc
│       ├── gmock_ex_test.cc
│       ├── gmock-generated-actions_test.cc
│       ├── gmock-generated-function-mockers_test.cc
│       ├── gmock-generated-internal-utils_test.cc
│       ├── gmock-generated-matchers_test.cc
│       ├── gmock-internal-utils_test.cc
│       ├── gmock_leak_test_.cc
│       ├── gmock_leak_test.py
│       ├── gmock_link2_test.cc
│       ├── gmock_link_test.cc
│       ├── gmock_link_test.h
│       ├── gmock-matchers_test.cc
│       ├── gmock-more-actions_test.cc
│       ├── gmock-nice-strict_test.cc
│       ├── gmock_output_test_.cc
│       ├── gmock_output_test_golden.txt
│       ├── gmock_output_test.py
│       ├── gmock-port_test.cc
│       ├── gmock-spec-builders_test.cc
│       ├── gmock_stress_test.cc
│       ├── gmock_test.cc
│       └── gmock_test_utils.py
├── googletest
│   ├── build-aux
│   ├── CHANGES
│   ├── cmake
│   │   └── internal_utils.cmake
│   ├── CMakeLists.txt
│   ├── codegear
│   │   ├── gtest_all.cc
│   │   ├── gtest.cbproj
│   │   ├── gtest.groupproj
│   │   ├── gtest_link.cc
│   │   ├── gtest_main.cbproj
│   │   └── gtest_unittest.cbproj
│   ├── configure.ac
│   ├── CONTRIBUTORS
│   ├── docs
│   │   ├── AdvancedGuide.md
│   │   ├── DevGuide.md
│   │   ├── Documentation.md
│   │   ├── FAQ.md
│   │   ├── Primer.md
│   │   ├── PumpManual.md
│   │   ├── Samples.md
│   │   ├── V1_5_AdvancedGuide.md
│   │   ├── V1_5_Documentation.md
│   │   ├── V1_5_FAQ.md
│   │   ├── V1_5_Primer.md
│   │   ├── V1_5_PumpManual.md
│   │   ├── V1_5_XcodeGuide.md
│   │   ├── V1_6_AdvancedGuide.md
│   │   ├── V1_6_Documentation.md
│   │   ├── V1_6_FAQ.md
│   │   ├── V1_6_Primer.md
│   │   ├── V1_6_PumpManual.md
│   │   ├── V1_6_Samples.md
│   │   ├── V1_6_XcodeGuide.md
│   │   ├── V1_7_AdvancedGuide.md
│   │   ├── V1_7_Documentation.md
│   │   ├── V1_7_FAQ.md
│   │   ├── V1_7_Primer.md
│   │   ├── V1_7_PumpManual.md
│   │   ├── V1_7_Samples.md
│   │   ├── V1_7_XcodeGuide.md
│   │   └── XcodeGuide.md
│   ├── include
│   │   └── gtest
│   │       ├── gtest-death-test.h
│   │       ├── gtest.h
│   │       ├── gtest-message.h
│   │       ├── gtest-param-test.h
│   │       ├── gtest-param-test.h.pump
│   │       ├── gtest_pred_impl.h
│   │       ├── gtest-printers.h
│   │       ├── gtest_prod.h
│   │       ├── gtest-spi.h
│   │       ├── gtest-test-part.h
│   │       ├── gtest-typed-test.h
│   │       └── internal
│   │           ├── custom
│   │           │   ├── gtest.h
│   │           │   ├── gtest-port.h
│   │           │   └── gtest-printers.h
│   │           ├── gtest-death-test-internal.h
│   │           ├── gtest-filepath.h
│   │           ├── gtest-internal.h
│   │           ├── gtest-linked_ptr.h
│   │           ├── gtest-param-util-generated.h
│   │           ├── gtest-param-util-generated.h.pump
│   │           ├── gtest-param-util.h
│   │           ├── gtest-port-arch.h
│   │           ├── gtest-port.h
│   │           ├── gtest-string.h
│   │           ├── gtest-tuple.h
│   │           ├── gtest-tuple.h.pump
│   │           ├── gtest-type-util.h
│   │           └── gtest-type-util.h.pump
│   ├── LICENSE
│   ├── m4
│   │   ├── acx_pthread.m4
│   │   └── gtest.m4
│   ├── make
│   │   └── Makefile
│   ├── Makefile.am
│   ├── msvc
│   │   ├── gtest_main-md.vcproj
│   │   ├── gtest_main.vcproj
│   │   ├── gtest-md.sln
│   │   ├── gtest-md.vcproj
│   │   ├── gtest_prod_test-md.vcproj
│   │   ├── gtest_prod_test.vcproj
│   │   ├── gtest.sln
│   │   ├── gtest_unittest-md.vcproj
│   │   ├── gtest_unittest.vcproj
│   │   └── gtest.vcproj
│   ├── README.md
│   ├── samples
│   │   ├── prime_tables.h
│   │   ├── sample10_unittest.cc
│   │   ├── sample1.cc
│   │   ├── sample1.h
│   │   ├── sample1_unittest.cc
│   │   ├── sample2.cc
│   │   ├── sample2.h
│   │   ├── sample2_unittest.cc
│   │   ├── sample3-inl.h
│   │   ├── sample3_unittest.cc
│   │   ├── sample4.cc
│   │   ├── sample4.h
│   │   ├── sample4_unittest.cc
│   │   ├── sample5_unittest.cc
│   │   ├── sample6_unittest.cc
│   │   ├── sample7_unittest.cc
│   │   ├── sample8_unittest.cc
│   │   └── sample9_unittest.cc
│   ├── scripts
│   │   ├── common.py
│   │   ├── fuse_gtest_files.py
│   │   ├── gen_gtest_pred_impl.py
│   │   ├── gtest-config.in
│   │   ├── pump.py
│   │   ├── release_docs.py
│   │   ├── test
│   │   │   └── Makefile
│   │   ├── upload_gtest.py
│   │   └── upload.py
│   ├── src
│   │   ├── gtest-all.cc
│   │   ├── gtest.cc
│   │   ├── gtest-death-test.cc
│   │   ├── gtest-filepath.cc
│   │   ├── gtest-internal-inl.h
│   │   ├── gtest_main.cc
│   │   ├── gtest-port.cc
│   │   ├── gtest-printers.cc
│   │   ├── gtest-test-part.cc
│   │   └── gtest-typed-test.cc
│   ├── test
│   │   ├── gtest_all_test.cc
│   │   ├── gtest_break_on_failure_unittest_.cc
│   │   ├── gtest_break_on_failure_unittest.py
│   │   ├── gtest_catch_exceptions_test_.cc
│   │   ├── gtest_catch_exceptions_test.py
│   │   ├── gtest_color_test_.cc
│   │   ├── gtest_color_test.py
│   │   ├── gtest-death-test_ex_test.cc
│   │   ├── gtest-death-test_test.cc
│   │   ├── gtest_environment_test.cc
│   │   ├── gtest_env_var_test_.cc
│   │   ├── gtest_env_var_test.py
│   │   ├── gtest-filepath_test.cc
│   │   ├── gtest_filter_unittest_.cc
│   │   ├── gtest_filter_unittest.py
│   │   ├── gtest_help_test_.cc
│   │   ├── gtest_help_test.py
│   │   ├── gtest-linked_ptr_test.cc
│   │   ├── gtest-listener_test.cc
│   │   ├── gtest_list_tests_unittest_.cc
│   │   ├── gtest_list_tests_unittest.py
│   │   ├── gtest_main_unittest.cc
│   │   ├── gtest-message_test.cc
│   │   ├── gtest_no_test_unittest.cc
│   │   ├── gtest-options_test.cc
│   │   ├── gtest_output_test_.cc
│   │   ├── gtest_output_test_golden_lin.txt
│   │   ├── gtest_output_test.py
│   │   ├── gtest-param-test2_test.cc
│   │   ├── gtest-param-test_test.cc
│   │   ├── gtest-param-test_test.h
│   │   ├── gtest-port_test.cc
│   │   ├── gtest_pred_impl_unittest.cc
│   │   ├── gtest_premature_exit_test.cc
│   │   ├── gtest-printers_test.cc
│   │   ├── gtest_prod_test.cc
│   │   ├── gtest_repeat_test.cc
│   │   ├── gtest_shuffle_test_.cc
│   │   ├── gtest_shuffle_test.py
│   │   ├── gtest_sole_header_test.cc
│   │   ├── gtest_stress_test.cc
│   │   ├── gtest-test-part_test.cc
│   │   ├── gtest_test_utils.py
│   │   ├── gtest_throw_on_failure_ex_test.cc
│   │   ├── gtest_throw_on_failure_test_.cc
│   │   ├── gtest_throw_on_failure_test.py
│   │   ├── gtest-tuple_test.cc
│   │   ├── gtest-typed-test2_test.cc
│   │   ├── gtest-typed-test_test.cc
│   │   ├── gtest-typed-test_test.h
│   │   ├── gtest_uninitialized_test_.cc
│   │   ├── gtest_uninitialized_test.py
│   │   ├── gtest-unittest-api_test.cc
│   │   ├── gtest_unittest.cc
│   │   ├── gtest_xml_outfile1_test_.cc
│   │   ├── gtest_xml_outfile2_test_.cc
│   │   ├── gtest_xml_outfiles_test.py
│   │   ├── gtest_xml_output_unittest_.cc
│   │   ├── gtest_xml_output_unittest.py
│   │   ├── gtest_xml_test_utils.py
│   │   ├── production.cc
│   │   └── production.h
│   └── xcode
│       ├── Config
│       │   ├── DebugProject.xcconfig
│       │   ├── FrameworkTarget.xcconfig
│       │   ├── General.xcconfig
│       │   ├── ReleaseProject.xcconfig
│       │   ├── StaticLibraryTarget.xcconfig
│       │   └── TestTarget.xcconfig
│       ├── gtest.xcodeproj
│       │   └── project.pbxproj
│       ├── Resources
│       │   └── Info.plist
│       ├── Samples
│       │   └── FrameworkSample
│       │       ├── Info.plist
│       │       ├── runtests.sh
│       │       ├── widget.cc
│       │       ├── WidgetFramework.xcodeproj
│       │       │   └── project.pbxproj
│       │       ├── widget.h
│       │       └── widget_test.cc
│       └── Scripts
│           ├── runtests.sh
│           └── versiongenerate.py
├── README.md
└── travis.sh
```
