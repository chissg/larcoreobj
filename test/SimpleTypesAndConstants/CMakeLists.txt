# ======================================================================
#
# Testing
#
# ======================================================================

find_package(Boost REQUIRED)

cet_test( geo_types_test USE_BOOST_UNIT )
cet_test( readout_types_test USE_BOOST_UNIT )
cet_test( geo_types_fhicl_test USE_BOOST_UNIT
  LIBRARIES PRIVATE
    fhiclcpp::fhiclcpp fhiclcpp::types
    cetlib_except::cetlib_except
  )
cet_test( readout_types_fhicl_test USE_BOOST_UNIT
  LIBRARIES PRIVATE
    fhiclcpp::fhiclcpp fhiclcpp::types
    cetlib_except::cetlib_except
  )
cet_test( testPhysicalConstants )
