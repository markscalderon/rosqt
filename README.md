# rosqt
to run this code in ROS Kinetic, we must modify the file "/usr/include/boost/type_traits/detail/has_binary_operator.hpp"
The line before (aprox 50) namespace BOOST_JOIN(BOOST_TT_TRAIT_NAME,_impl) {
we add:
 #ifndef Q_MOC_RUN
close this macro with #endif, it will add before the close brace in the line <b>} // namespace detail</b>

The new code is in the project


