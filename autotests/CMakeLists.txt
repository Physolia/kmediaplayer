find_package(Qt${QT_MAJOR_VERSION}Test ${REQUIRED_QT_VERSION} REQUIRED NO_MODULE)
include(ECMMarkAsTest)
include(ECMAddTests)

ecm_add_tests(
   playertest.cpp
   viewtest.cpp
   LINK_LIBRARIES Qt${QT_MAJOR_VERSION}::Test KF5::MediaPlayer
)

