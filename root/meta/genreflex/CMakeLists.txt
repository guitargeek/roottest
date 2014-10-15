ROOTTEST_ADD_TESTDIRS()

ROOTTEST_GENERATE_REFLEX_DICTIONARY(typedefSelection typedefSelection.h SELECTION typedefSelection_selection.xml)

ROOTTEST_ADD_TEST(roottest-root-meta-genreflex-typedefSelection
                  MACRO execTypedefSelection.C
                  OUTREF execTypedefSelection.ref
                  DEPENDS ${GENERATE_REFLEX_TEST})

ROOTTEST_GENERATE_REFLEX_DICTIONARY(stlPatternSelection stlPatternSelection.h SELECTION stlPatternSelection_selection.xml)

ROOTTEST_ADD_TEST(roottest-root-meta-genreflex-stlPatternSelection
                  MACRO execstlPatternSelection.C
                  OUTREF execstlPatternSelection.ref
                  DEPENDS ${GENERATE_REFLEX_TEST})

ROOTTEST_GENERATE_REFLEX_DICTIONARY(complicatedAllocator complicatedAllocator.h SELECTION complicatedAllocator_selection.xml)

ROOTTEST_ADD_TEST(roottest-root-meta-genreflex-CheckComplicatedAllocator
                  MACRO execCheckComplicatedAllocator.C
                  OUTREF execCheckComplicatedAllocator.ref
                  DEPENDS ${GENERATE_REFLEX_TEST})

ROOTTEST_GENERATE_REFLEX_DICTIONARY(ns ns.h SELECTION ns_selection.xml)

ROOTTEST_ADD_TEST(roottest-root-meta-genreflex-ns
                  MACRO execns.C
                  OUTREF execns.ref
                  DEPENDS ${GENERATE_REFLEX_TEST})