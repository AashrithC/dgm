+ set -e
+ '[' '!' -d build ']'
+ mkdir build
+ cd build
+ cmake -DEXERCISM_RUN_ALL_TESTS=1 -G 'Unix Makefiles' ..
-- The CXX compiler identification is GNU 11.4.0
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++ - skipped
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Configuring done
-- Generating done
-- Build files have been written to: /testbed/build
+ make
[ 25%] Building CXX object CMakeFiles/grade-school.dir/grade_school_test.cpp.o
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp: In function 'void ____C_A_T_C_H____T_E_S_T____2()':
/testbed/grade_school_test.cpp:26:22: error: no match for 'operator==' (operand types are 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' and 'const std::vector<std::__cxx11::basic_string<char> >')
   26 |     REQUIRE(expected == actual);
      |             ~~~~~~~~ ^~ ~~~~~~
      |             |           |
      |             |           const std::vector<std::__cxx11::basic_string<char> >
      |             const std::map<int, std::vector<std::__cxx11::basic_string<char> > >
In file included from /usr/include/c++/11/bits/stl_algobase.h:64,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_pair.h:466:5: note: candidate: 'template<class _T1, class _T2> constexpr bool std::operator==(const std::pair<_T1, _T2>&, const std::pair<_T1, _T2>&)'
  466 |     operator==(const pair<_T1, _T2>& __x, const pair<_T1, _T2>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_pair.h:466:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::pair<_T1, _T2>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:420:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_Iterator>&)'
  420 |     operator==(const reverse_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:420:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:459:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_IteratorR>&)'
  459 |     operator==(const reverse_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:459:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorR>&)'
 1585 |     operator==(const move_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorL>&)'
 1648 |     operator==(const move_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:218:5: note: candidate: 'template<class _T1, class _T2> bool std::operator==(const std::allocator<_Tp1>&, const std::allocator<_T2>&)'
  218 |     operator==(const allocator<_T1>&, const allocator<_T2>&)
      |     ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:218:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::allocator<_Tp1>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:67,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_vector.h:1892:5: note: candidate: 'template<class _Tp, class _Alloc> bool std::operator==(const std::vector<_Tp, _Alloc>&, const std::vector<_Tp, _Alloc>&)'
 1892 |     operator==(const vector<_Tp, _Alloc>& __x, const vector<_Tp, _Alloc>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_vector.h:1892:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::vector<_Tp, _Alloc>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/char_traits.h:40,
                 from /usr/include/c++/11/string:40,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/postypes.h:222:5: note: candidate: 'template<class _StateT> bool std::operator==(const std::fpos<_StateT>&, const std::fpos<_StateT>&)'
  222 |     operator==(const fpos<_StateT>& __lhs, const fpos<_StateT>& __rhs)
      |     ^~~~~~~~
/usr/include/c++/11/bits/postypes.h:222:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::fpos<_StateT>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:535:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::basic_string_view<_CharT, _Traits>)'
  535 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:535:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:541:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >)'
  541 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:541:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:564:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >, std::basic_string_view<_CharT, _Traits>)'
  564 |     operator==(__type_identity_t<basic_string_view<_CharT, _Traits>> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:564:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'std::vector<std::__cxx11::basic_string<char> >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6226:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6226 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6234:5: note: candidate: 'template<class _CharT> typename __gnu_cxx::__enable_if<std::__is_char<_Tp>::__value, bool>::__type std::operator==(const std::__cxx11::basic_string<_CharT>&, const std::__cxx11::basic_string<_CharT>&)'
 6234 |     operator==(const basic_string<_CharT>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6234:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6248:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const _CharT*)'
 6248 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6248:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6289:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const _CharT*, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6289 |     operator==(const _CharT* __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6289:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   mismatched types 'const _CharT*' and 'std::map<int, std::vector<std::__cxx11::basic_string<char> > >'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/tuple:39,
                 from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/array:276:5: note: candidate: 'template<class _Tp, long unsigned int _Nm> bool std::operator==(const std::array<_Tp, _Nm>&, const std::array<_Tp, _Nm>&)'
  276 |     operator==(const array<_Tp, _Nm>& __one, const array<_Tp, _Nm>& __two)
      |     ^~~~~~~~
/usr/include/c++/11/array:276:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::array<_Tp, _Nm>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/tuple:1524:5: note: candidate: 'template<class ... _TElements, class ... _UElements> constexpr bool std::operator==(const std::tuple<_Tps ...>&, const std::tuple<_Args2 ...>&)'
 1524 |     operator==(const tuple<_TElements...>& __t,
      |     ^~~~~~~~
/usr/include/c++/11/tuple:1524:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::tuple<_Tps ...>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_map.h:1463:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::map<_Key, _Tp, _Compare, _Allocator>&, const std::map<_Key, _Tp, _Compare, _Allocator>&)'
 1463 |     operator==(const map<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_map.h:1463:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::map<_Key, _Tp, _Compare, _Allocator>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:62,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::multimap<_Key, _Tp, _Compare, _Allocator>&, const std::multimap<_Key, _Tp, _Compare, _Allocator>&)'
 1128 |     operator==(const multimap<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::multimap<_Key, _Tp, _Compare, _Allocator>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:718:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(const std::function<_Res(_ArgTypes ...)>&, std::nullptr_t)'
  718 |     operator==(const function<_Res(_Args...)>& __f, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:718:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:725:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(std::nullptr_t, const std::function<_Res(_ArgTypes ...)>&)'
  725 |     operator==(nullptr_t, const function<_Res(_Args...)>& __f) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:725:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2134:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2134 |     operator==(const unordered_map<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2134:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2148:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2148 |     operator==(const unordered_multimap<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2148:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/locale_facets.h:48,
                 from /usr/include/c++/11/bits/basic_ios.h:37,
                 from /usr/include/c++/11/ios:44,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note: candidate: 'template<class _CharT, class _Traits> bool std::operator==(const std::istreambuf_iterator<_CharT, _Traits>&, const std::istreambuf_iterator<_CharT, _Traits>&)'
  226 |     operator==(const istreambuf_iterator<_CharT, _Traits>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::istreambuf_iterator<_CharT, _Traits>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:753:5: note: candidate: 'template<class _Tp, class _Dp, class _Up, class _Ep> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, const std::unique_ptr<_Up, _Ep>&)'
  753 |     operator==(const unique_ptr<_Tp, _Dp>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:753:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:760:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, std::nullptr_t)'
  760 |     operator==(const unique_ptr<_Tp, _Dp>& __x, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:760:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:767:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(std::nullptr_t, const std::unique_ptr<_Tp, _Dp>&)'
  767 |     operator==(nullptr_t, const unique_ptr<_Tp, _Dp>& __x) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:767:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note: candidate: 'template<class _Tp1, class _Tp2, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp1, _Lp>&, const std::__shared_ptr<_Tp2, _Lp>&)'
 1410 |     operator==(const __shared_ptr<_Tp1, _Lp>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp1, _Lp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp, _Lp>&, std::nullptr_t)'
 1416 |     operator==(const __shared_ptr<_Tp, _Lp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(std::nullptr_t, const std::__shared_ptr<_Tp, _Lp>&)'
 1436 |     operator==(nullptr_t, const __shared_ptr<_Tp, _Lp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:437:5: note: candidate: 'template<class _Tp, class _Up> bool std::operator==(const std::shared_ptr<_Tp>&, const std::shared_ptr<_Tp>&)'
  437 |     operator==(const shared_ptr<_Tp>& __a, const shared_ptr<_Up>& __b) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:437:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:443:5: note: candidate: 'template<class _Tp> bool std::operator==(const std::shared_ptr<_Tp>&, std::nullptr_t)'
  443 |     operator==(const shared_ptr<_Tp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:443:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:464:5: note: candidate: 'template<class _Tp> bool std::operator==(std::nullptr_t, const std::shared_ptr<_Tp>&)'
  464 |     operator==(nullptr_t, const shared_ptr<_Tp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:464:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::shared_ptr<_Tp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/random:51,
                 from /testbed/test/catch.hpp:4590,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/random.tcc:1899:5: note: candidate: 'template<class _RealType1> bool std::operator==(const std::normal_distribution<_RealType>&, const std::normal_distribution<_RealType>&)'
 1899 |     operator==(const std::normal_distribution<_RealType>& __d1,
      |     ^~~~~~~~
/usr/include/c++/11/bits/random.tcc:1899:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::normal_distribution<_RealType>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::__cxx11::basic_string<char> >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note: candidate: 'template<class _IteratorL, class _IteratorR, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_IteratorL, _Container>&, const __gnu_cxx::__normal_iterator<_IteratorR, _Container>&)'
 1155 |     operator==(const __normal_iterator<_IteratorL, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_IteratorL, _Container>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note: candidate: 'template<class _Iterator, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_Iterator, _Container>&, const __gnu_cxx::__normal_iterator<_Iterator, _Container>&)'
 1163 |     operator==(const __normal_iterator<_Iterator, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_Iterator, _Container>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<char>&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/ios_base.h:46,
                 from /usr/include/c++/11/ios:42,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/system_error:362:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_code&)'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:362:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:368:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_condition&)'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:368:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:376:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_condition&)'
  376 |   operator==(const error_condition& __lhs,
      |   ^~~~~~~~
/usr/include/c++/11/system_error:376:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  376 |   operator==(const error_condition& __lhs,
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:408:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_code&)'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:408:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::__cxx11::basic_string<char> >&, const std::allocator<std::__cxx11::basic_string<char> >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::__cxx11::basic_string<char> >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<char>&, const std::allocator<char>&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<char>&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:22: error: no match for 'operator==' (operand types are 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' and 'const std::vector<std::__cxx11::basic_string<char> >')
   26 |     REQUIRE(expected == actual);
      |             ~~~~~~~~ ^~ ~~~~~~
      |             |           |
      |             |           const std::vector<std::__cxx11::basic_string<char> >
      |             const std::map<int, std::vector<std::__cxx11::basic_string<char> > >
In file included from /usr/include/c++/11/bits/stl_algobase.h:64,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_pair.h:466:5: note: candidate: 'template<class _T1, class _T2> constexpr bool std::operator==(const std::pair<_T1, _T2>&, const std::pair<_T1, _T2>&)'
  466 |     operator==(const pair<_T1, _T2>& __x, const pair<_T1, _T2>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_pair.h:466:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::pair<_T1, _T2>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:420:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_Iterator>&)'
  420 |     operator==(const reverse_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:420:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:459:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_IteratorR>&)'
  459 |     operator==(const reverse_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:459:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorR>&)'
 1585 |     operator==(const move_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorL>&)'
 1648 |     operator==(const move_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:218:5: note: candidate: 'template<class _T1, class _T2> bool std::operator==(const std::allocator<_Tp1>&, const std::allocator<_T2>&)'
  218 |     operator==(const allocator<_T1>&, const allocator<_T2>&)
      |     ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:218:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::allocator<_Tp1>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:67,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_vector.h:1892:5: note: candidate: 'template<class _Tp, class _Alloc> bool std::operator==(const std::vector<_Tp, _Alloc>&, const std::vector<_Tp, _Alloc>&)'
 1892 |     operator==(const vector<_Tp, _Alloc>& __x, const vector<_Tp, _Alloc>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_vector.h:1892:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::vector<_Tp, _Alloc>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/char_traits.h:40,
                 from /usr/include/c++/11/string:40,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/postypes.h:222:5: note: candidate: 'template<class _StateT> bool std::operator==(const std::fpos<_StateT>&, const std::fpos<_StateT>&)'
  222 |     operator==(const fpos<_StateT>& __lhs, const fpos<_StateT>& __rhs)
      |     ^~~~~~~~
/usr/include/c++/11/bits/postypes.h:222:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::fpos<_StateT>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:535:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::basic_string_view<_CharT, _Traits>)'
  535 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:535:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:541:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >)'
  541 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:541:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:564:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >, std::basic_string_view<_CharT, _Traits>)'
  564 |     operator==(__type_identity_t<basic_string_view<_CharT, _Traits>> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:564:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'std::vector<std::__cxx11::basic_string<char> >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6226:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6226 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6234:5: note: candidate: 'template<class _CharT> typename __gnu_cxx::__enable_if<std::__is_char<_Tp>::__value, bool>::__type std::operator==(const std::__cxx11::basic_string<_CharT>&, const std::__cxx11::basic_string<_CharT>&)'
 6234 |     operator==(const basic_string<_CharT>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6234:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6248:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const _CharT*)'
 6248 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6248:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6289:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const _CharT*, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6289 |     operator==(const _CharT* __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6289:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   mismatched types 'const _CharT*' and 'std::map<int, std::vector<std::__cxx11::basic_string<char> > >'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/tuple:39,
                 from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/array:276:5: note: candidate: 'template<class _Tp, long unsigned int _Nm> bool std::operator==(const std::array<_Tp, _Nm>&, const std::array<_Tp, _Nm>&)'
  276 |     operator==(const array<_Tp, _Nm>& __one, const array<_Tp, _Nm>& __two)
      |     ^~~~~~~~
/usr/include/c++/11/array:276:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::array<_Tp, _Nm>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/tuple:1524:5: note: candidate: 'template<class ... _TElements, class ... _UElements> constexpr bool std::operator==(const std::tuple<_Tps ...>&, const std::tuple<_Args2 ...>&)'
 1524 |     operator==(const tuple<_TElements...>& __t,
      |     ^~~~~~~~
/usr/include/c++/11/tuple:1524:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::tuple<_Tps ...>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_map.h:1463:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::map<_Key, _Tp, _Compare, _Allocator>&, const std::map<_Key, _Tp, _Compare, _Allocator>&)'
 1463 |     operator==(const map<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_map.h:1463:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::map<_Key, _Tp, _Compare, _Allocator>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:62,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::multimap<_Key, _Tp, _Compare, _Allocator>&, const std::multimap<_Key, _Tp, _Compare, _Allocator>&)'
 1128 |     operator==(const multimap<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::multimap<_Key, _Tp, _Compare, _Allocator>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:718:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(const std::function<_Res(_ArgTypes ...)>&, std::nullptr_t)'
  718 |     operator==(const function<_Res(_Args...)>& __f, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:718:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:725:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(std::nullptr_t, const std::function<_Res(_ArgTypes ...)>&)'
  725 |     operator==(nullptr_t, const function<_Res(_Args...)>& __f) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:725:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2134:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2134 |     operator==(const unordered_map<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2134:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2148:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2148 |     operator==(const unordered_multimap<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2148:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/locale_facets.h:48,
                 from /usr/include/c++/11/bits/basic_ios.h:37,
                 from /usr/include/c++/11/ios:44,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note: candidate: 'template<class _CharT, class _Traits> bool std::operator==(const std::istreambuf_iterator<_CharT, _Traits>&, const std::istreambuf_iterator<_CharT, _Traits>&)'
  226 |     operator==(const istreambuf_iterator<_CharT, _Traits>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::istreambuf_iterator<_CharT, _Traits>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:753:5: note: candidate: 'template<class _Tp, class _Dp, class _Up, class _Ep> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, const std::unique_ptr<_Up, _Ep>&)'
  753 |     operator==(const unique_ptr<_Tp, _Dp>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:753:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:760:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, std::nullptr_t)'
  760 |     operator==(const unique_ptr<_Tp, _Dp>& __x, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:760:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:767:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(std::nullptr_t, const std::unique_ptr<_Tp, _Dp>&)'
  767 |     operator==(nullptr_t, const unique_ptr<_Tp, _Dp>& __x) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:767:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note: candidate: 'template<class _Tp1, class _Tp2, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp1, _Lp>&, const std::__shared_ptr<_Tp2, _Lp>&)'
 1410 |     operator==(const __shared_ptr<_Tp1, _Lp>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp1, _Lp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp, _Lp>&, std::nullptr_t)'
 1416 |     operator==(const __shared_ptr<_Tp, _Lp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(std::nullptr_t, const std::__shared_ptr<_Tp, _Lp>&)'
 1436 |     operator==(nullptr_t, const __shared_ptr<_Tp, _Lp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:437:5: note: candidate: 'template<class _Tp, class _Up> bool std::operator==(const std::shared_ptr<_Tp>&, const std::shared_ptr<_Tp>&)'
  437 |     operator==(const shared_ptr<_Tp>& __a, const shared_ptr<_Up>& __b) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:437:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:443:5: note: candidate: 'template<class _Tp> bool std::operator==(const std::shared_ptr<_Tp>&, std::nullptr_t)'
  443 |     operator==(const shared_ptr<_Tp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:443:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:464:5: note: candidate: 'template<class _Tp> bool std::operator==(std::nullptr_t, const std::shared_ptr<_Tp>&)'
  464 |     operator==(nullptr_t, const shared_ptr<_Tp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:464:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::shared_ptr<_Tp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/random:51,
                 from /testbed/test/catch.hpp:4590,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/random.tcc:1899:5: note: candidate: 'template<class _RealType1> bool std::operator==(const std::normal_distribution<_RealType>&, const std::normal_distribution<_RealType>&)'
 1899 |     operator==(const std::normal_distribution<_RealType>& __d1,
      |     ^~~~~~~~
/usr/include/c++/11/bits/random.tcc:1899:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::normal_distribution<_RealType>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::__cxx11::basic_string<char> >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note: candidate: 'template<class _IteratorL, class _IteratorR, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_IteratorL, _Container>&, const __gnu_cxx::__normal_iterator<_IteratorR, _Container>&)'
 1155 |     operator==(const __normal_iterator<_IteratorL, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_IteratorL, _Container>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note: candidate: 'template<class _Iterator, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_Iterator, _Container>&, const __gnu_cxx::__normal_iterator<_Iterator, _Container>&)'
 1163 |     operator==(const __normal_iterator<_Iterator, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_Iterator, _Container>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<char>&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:26:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   26 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/ios_base.h:46,
                 from /usr/include/c++/11/ios:42,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/system_error:362:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_code&)'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:362:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:368:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_condition&)'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:368:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:376:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_condition&)'
  376 |   operator==(const error_condition& __lhs,
      |   ^~~~~~~~
/usr/include/c++/11/system_error:376:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  376 |   operator==(const error_condition& __lhs,
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:408:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_code&)'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:408:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::__cxx11::basic_string<char> >&, const std::allocator<std::__cxx11::basic_string<char> >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::__cxx11::basic_string<char> >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<char>&, const std::allocator<char>&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<char>&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp: In function 'void ____C_A_T_C_H____T_E_S_T____4()':
/testbed/grade_school_test.cpp:39:22: error: no match for 'operator==' (operand types are 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' and 'const std::vector<std::__cxx11::basic_string<char> >')
   39 |     REQUIRE(expected == actual);
      |             ~~~~~~~~ ^~ ~~~~~~
      |             |           |
      |             |           const std::vector<std::__cxx11::basic_string<char> >
      |             const std::map<int, std::vector<std::__cxx11::basic_string<char> > >
In file included from /usr/include/c++/11/bits/stl_algobase.h:64,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_pair.h:466:5: note: candidate: 'template<class _T1, class _T2> constexpr bool std::operator==(const std::pair<_T1, _T2>&, const std::pair<_T1, _T2>&)'
  466 |     operator==(const pair<_T1, _T2>& __x, const pair<_T1, _T2>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_pair.h:466:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::pair<_T1, _T2>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:420:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_Iterator>&)'
  420 |     operator==(const reverse_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:420:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:459:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_IteratorR>&)'
  459 |     operator==(const reverse_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:459:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorR>&)'
 1585 |     operator==(const move_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorL>&)'
 1648 |     operator==(const move_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:218:5: note: candidate: 'template<class _T1, class _T2> bool std::operator==(const std::allocator<_Tp1>&, const std::allocator<_T2>&)'
  218 |     operator==(const allocator<_T1>&, const allocator<_T2>&)
      |     ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:218:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::allocator<_Tp1>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:67,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_vector.h:1892:5: note: candidate: 'template<class _Tp, class _Alloc> bool std::operator==(const std::vector<_Tp, _Alloc>&, const std::vector<_Tp, _Alloc>&)'
 1892 |     operator==(const vector<_Tp, _Alloc>& __x, const vector<_Tp, _Alloc>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_vector.h:1892:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::vector<_Tp, _Alloc>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/char_traits.h:40,
                 from /usr/include/c++/11/string:40,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/postypes.h:222:5: note: candidate: 'template<class _StateT> bool std::operator==(const std::fpos<_StateT>&, const std::fpos<_StateT>&)'
  222 |     operator==(const fpos<_StateT>& __lhs, const fpos<_StateT>& __rhs)
      |     ^~~~~~~~
/usr/include/c++/11/bits/postypes.h:222:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::fpos<_StateT>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:535:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::basic_string_view<_CharT, _Traits>)'
  535 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:535:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:541:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >)'
  541 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:541:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:564:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >, std::basic_string_view<_CharT, _Traits>)'
  564 |     operator==(__type_identity_t<basic_string_view<_CharT, _Traits>> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:564:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'std::vector<std::__cxx11::basic_string<char> >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6226:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6226 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6234:5: note: candidate: 'template<class _CharT> typename __gnu_cxx::__enable_if<std::__is_char<_Tp>::__value, bool>::__type std::operator==(const std::__cxx11::basic_string<_CharT>&, const std::__cxx11::basic_string<_CharT>&)'
 6234 |     operator==(const basic_string<_CharT>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6234:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6248:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const _CharT*)'
 6248 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6248:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6289:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const _CharT*, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6289 |     operator==(const _CharT* __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6289:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   mismatched types 'const _CharT*' and 'std::map<int, std::vector<std::__cxx11::basic_string<char> > >'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/tuple:39,
                 from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/array:276:5: note: candidate: 'template<class _Tp, long unsigned int _Nm> bool std::operator==(const std::array<_Tp, _Nm>&, const std::array<_Tp, _Nm>&)'
  276 |     operator==(const array<_Tp, _Nm>& __one, const array<_Tp, _Nm>& __two)
      |     ^~~~~~~~
/usr/include/c++/11/array:276:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::array<_Tp, _Nm>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/tuple:1524:5: note: candidate: 'template<class ... _TElements, class ... _UElements> constexpr bool std::operator==(const std::tuple<_Tps ...>&, const std::tuple<_Args2 ...>&)'
 1524 |     operator==(const tuple<_TElements...>& __t,
      |     ^~~~~~~~
/usr/include/c++/11/tuple:1524:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::tuple<_Tps ...>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_map.h:1463:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::map<_Key, _Tp, _Compare, _Allocator>&, const std::map<_Key, _Tp, _Compare, _Allocator>&)'
 1463 |     operator==(const map<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_map.h:1463:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::map<_Key, _Tp, _Compare, _Allocator>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:62,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::multimap<_Key, _Tp, _Compare, _Allocator>&, const std::multimap<_Key, _Tp, _Compare, _Allocator>&)'
 1128 |     operator==(const multimap<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::multimap<_Key, _Tp, _Compare, _Allocator>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:718:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(const std::function<_Res(_ArgTypes ...)>&, std::nullptr_t)'
  718 |     operator==(const function<_Res(_Args...)>& __f, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:718:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:725:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(std::nullptr_t, const std::function<_Res(_ArgTypes ...)>&)'
  725 |     operator==(nullptr_t, const function<_Res(_Args...)>& __f) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:725:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2134:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2134 |     operator==(const unordered_map<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2134:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2148:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2148 |     operator==(const unordered_multimap<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2148:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/locale_facets.h:48,
                 from /usr/include/c++/11/bits/basic_ios.h:37,
                 from /usr/include/c++/11/ios:44,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note: candidate: 'template<class _CharT, class _Traits> bool std::operator==(const std::istreambuf_iterator<_CharT, _Traits>&, const std::istreambuf_iterator<_CharT, _Traits>&)'
  226 |     operator==(const istreambuf_iterator<_CharT, _Traits>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::istreambuf_iterator<_CharT, _Traits>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:753:5: note: candidate: 'template<class _Tp, class _Dp, class _Up, class _Ep> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, const std::unique_ptr<_Up, _Ep>&)'
  753 |     operator==(const unique_ptr<_Tp, _Dp>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:753:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:760:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, std::nullptr_t)'
  760 |     operator==(const unique_ptr<_Tp, _Dp>& __x, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:760:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:767:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(std::nullptr_t, const std::unique_ptr<_Tp, _Dp>&)'
  767 |     operator==(nullptr_t, const unique_ptr<_Tp, _Dp>& __x) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:767:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note: candidate: 'template<class _Tp1, class _Tp2, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp1, _Lp>&, const std::__shared_ptr<_Tp2, _Lp>&)'
 1410 |     operator==(const __shared_ptr<_Tp1, _Lp>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp1, _Lp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp, _Lp>&, std::nullptr_t)'
 1416 |     operator==(const __shared_ptr<_Tp, _Lp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(std::nullptr_t, const std::__shared_ptr<_Tp, _Lp>&)'
 1436 |     operator==(nullptr_t, const __shared_ptr<_Tp, _Lp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:437:5: note: candidate: 'template<class _Tp, class _Up> bool std::operator==(const std::shared_ptr<_Tp>&, const std::shared_ptr<_Tp>&)'
  437 |     operator==(const shared_ptr<_Tp>& __a, const shared_ptr<_Up>& __b) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:437:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:443:5: note: candidate: 'template<class _Tp> bool std::operator==(const std::shared_ptr<_Tp>&, std::nullptr_t)'
  443 |     operator==(const shared_ptr<_Tp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:443:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:464:5: note: candidate: 'template<class _Tp> bool std::operator==(std::nullptr_t, const std::shared_ptr<_Tp>&)'
  464 |     operator==(nullptr_t, const shared_ptr<_Tp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:464:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::shared_ptr<_Tp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/random:51,
                 from /testbed/test/catch.hpp:4590,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/random.tcc:1899:5: note: candidate: 'template<class _RealType1> bool std::operator==(const std::normal_distribution<_RealType>&, const std::normal_distribution<_RealType>&)'
 1899 |     operator==(const std::normal_distribution<_RealType>& __d1,
      |     ^~~~~~~~
/usr/include/c++/11/bits/random.tcc:1899:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::normal_distribution<_RealType>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::__cxx11::basic_string<char> >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note: candidate: 'template<class _IteratorL, class _IteratorR, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_IteratorL, _Container>&, const __gnu_cxx::__normal_iterator<_IteratorR, _Container>&)'
 1155 |     operator==(const __normal_iterator<_IteratorL, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_IteratorL, _Container>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note: candidate: 'template<class _Iterator, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_Iterator, _Container>&, const __gnu_cxx::__normal_iterator<_Iterator, _Container>&)'
 1163 |     operator==(const __normal_iterator<_Iterator, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_Iterator, _Container>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<char>&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/ios_base.h:46,
                 from /usr/include/c++/11/ios:42,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/system_error:362:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_code&)'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:362:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:368:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_condition&)'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:368:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:376:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_condition&)'
  376 |   operator==(const error_condition& __lhs,
      |   ^~~~~~~~
/usr/include/c++/11/system_error:376:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  376 |   operator==(const error_condition& __lhs,
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:408:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_code&)'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:408:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::__cxx11::basic_string<char> >&, const std::allocator<std::__cxx11::basic_string<char> >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::__cxx11::basic_string<char> >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<char>&, const std::allocator<char>&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<char>&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:22: error: no match for 'operator==' (operand types are 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' and 'const std::vector<std::__cxx11::basic_string<char> >')
   39 |     REQUIRE(expected == actual);
      |             ~~~~~~~~ ^~ ~~~~~~
      |             |           |
      |             |           const std::vector<std::__cxx11::basic_string<char> >
      |             const std::map<int, std::vector<std::__cxx11::basic_string<char> > >
In file included from /usr/include/c++/11/bits/stl_algobase.h:64,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_pair.h:466:5: note: candidate: 'template<class _T1, class _T2> constexpr bool std::operator==(const std::pair<_T1, _T2>&, const std::pair<_T1, _T2>&)'
  466 |     operator==(const pair<_T1, _T2>& __x, const pair<_T1, _T2>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_pair.h:466:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::pair<_T1, _T2>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:420:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_Iterator>&)'
  420 |     operator==(const reverse_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:420:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:459:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_IteratorR>&)'
  459 |     operator==(const reverse_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:459:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorR>&)'
 1585 |     operator==(const move_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorL>&)'
 1648 |     operator==(const move_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:218:5: note: candidate: 'template<class _T1, class _T2> bool std::operator==(const std::allocator<_Tp1>&, const std::allocator<_T2>&)'
  218 |     operator==(const allocator<_T1>&, const allocator<_T2>&)
      |     ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:218:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::allocator<_Tp1>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:67,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_vector.h:1892:5: note: candidate: 'template<class _Tp, class _Alloc> bool std::operator==(const std::vector<_Tp, _Alloc>&, const std::vector<_Tp, _Alloc>&)'
 1892 |     operator==(const vector<_Tp, _Alloc>& __x, const vector<_Tp, _Alloc>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_vector.h:1892:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::vector<_Tp, _Alloc>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/char_traits.h:40,
                 from /usr/include/c++/11/string:40,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/postypes.h:222:5: note: candidate: 'template<class _StateT> bool std::operator==(const std::fpos<_StateT>&, const std::fpos<_StateT>&)'
  222 |     operator==(const fpos<_StateT>& __lhs, const fpos<_StateT>& __rhs)
      |     ^~~~~~~~
/usr/include/c++/11/bits/postypes.h:222:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::fpos<_StateT>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:535:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::basic_string_view<_CharT, _Traits>)'
  535 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:535:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:541:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >)'
  541 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:541:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:564:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >, std::basic_string_view<_CharT, _Traits>)'
  564 |     operator==(__type_identity_t<basic_string_view<_CharT, _Traits>> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:564:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'std::vector<std::__cxx11::basic_string<char> >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6226:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6226 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6234:5: note: candidate: 'template<class _CharT> typename __gnu_cxx::__enable_if<std::__is_char<_Tp>::__value, bool>::__type std::operator==(const std::__cxx11::basic_string<_CharT>&, const std::__cxx11::basic_string<_CharT>&)'
 6234 |     operator==(const basic_string<_CharT>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6234:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6248:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const _CharT*)'
 6248 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6248:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6289:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const _CharT*, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6289 |     operator==(const _CharT* __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6289:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   mismatched types 'const _CharT*' and 'std::map<int, std::vector<std::__cxx11::basic_string<char> > >'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/tuple:39,
                 from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/array:276:5: note: candidate: 'template<class _Tp, long unsigned int _Nm> bool std::operator==(const std::array<_Tp, _Nm>&, const std::array<_Tp, _Nm>&)'
  276 |     operator==(const array<_Tp, _Nm>& __one, const array<_Tp, _Nm>& __two)
      |     ^~~~~~~~
/usr/include/c++/11/array:276:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::array<_Tp, _Nm>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/tuple:1524:5: note: candidate: 'template<class ... _TElements, class ... _UElements> constexpr bool std::operator==(const std::tuple<_Tps ...>&, const std::tuple<_Args2 ...>&)'
 1524 |     operator==(const tuple<_TElements...>& __t,
      |     ^~~~~~~~
/usr/include/c++/11/tuple:1524:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::tuple<_Tps ...>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_map.h:1463:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::map<_Key, _Tp, _Compare, _Allocator>&, const std::map<_Key, _Tp, _Compare, _Allocator>&)'
 1463 |     operator==(const map<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_map.h:1463:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::map<_Key, _Tp, _Compare, _Allocator>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:62,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::multimap<_Key, _Tp, _Compare, _Allocator>&, const std::multimap<_Key, _Tp, _Compare, _Allocator>&)'
 1128 |     operator==(const multimap<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::multimap<_Key, _Tp, _Compare, _Allocator>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:718:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(const std::function<_Res(_ArgTypes ...)>&, std::nullptr_t)'
  718 |     operator==(const function<_Res(_Args...)>& __f, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:718:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:725:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(std::nullptr_t, const std::function<_Res(_ArgTypes ...)>&)'
  725 |     operator==(nullptr_t, const function<_Res(_Args...)>& __f) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:725:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2134:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2134 |     operator==(const unordered_map<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2134:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2148:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2148 |     operator==(const unordered_multimap<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2148:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/locale_facets.h:48,
                 from /usr/include/c++/11/bits/basic_ios.h:37,
                 from /usr/include/c++/11/ios:44,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note: candidate: 'template<class _CharT, class _Traits> bool std::operator==(const std::istreambuf_iterator<_CharT, _Traits>&, const std::istreambuf_iterator<_CharT, _Traits>&)'
  226 |     operator==(const istreambuf_iterator<_CharT, _Traits>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::istreambuf_iterator<_CharT, _Traits>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:753:5: note: candidate: 'template<class _Tp, class _Dp, class _Up, class _Ep> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, const std::unique_ptr<_Up, _Ep>&)'
  753 |     operator==(const unique_ptr<_Tp, _Dp>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:753:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:760:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, std::nullptr_t)'
  760 |     operator==(const unique_ptr<_Tp, _Dp>& __x, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:760:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:767:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(std::nullptr_t, const std::unique_ptr<_Tp, _Dp>&)'
  767 |     operator==(nullptr_t, const unique_ptr<_Tp, _Dp>& __x) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:767:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note: candidate: 'template<class _Tp1, class _Tp2, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp1, _Lp>&, const std::__shared_ptr<_Tp2, _Lp>&)'
 1410 |     operator==(const __shared_ptr<_Tp1, _Lp>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp1, _Lp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp, _Lp>&, std::nullptr_t)'
 1416 |     operator==(const __shared_ptr<_Tp, _Lp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(std::nullptr_t, const std::__shared_ptr<_Tp, _Lp>&)'
 1436 |     operator==(nullptr_t, const __shared_ptr<_Tp, _Lp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:437:5: note: candidate: 'template<class _Tp, class _Up> bool std::operator==(const std::shared_ptr<_Tp>&, const std::shared_ptr<_Tp>&)'
  437 |     operator==(const shared_ptr<_Tp>& __a, const shared_ptr<_Up>& __b) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:437:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:443:5: note: candidate: 'template<class _Tp> bool std::operator==(const std::shared_ptr<_Tp>&, std::nullptr_t)'
  443 |     operator==(const shared_ptr<_Tp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:443:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:464:5: note: candidate: 'template<class _Tp> bool std::operator==(std::nullptr_t, const std::shared_ptr<_Tp>&)'
  464 |     operator==(nullptr_t, const shared_ptr<_Tp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:464:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::shared_ptr<_Tp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/random:51,
                 from /testbed/test/catch.hpp:4590,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/random.tcc:1899:5: note: candidate: 'template<class _RealType1> bool std::operator==(const std::normal_distribution<_RealType>&, const std::normal_distribution<_RealType>&)'
 1899 |     operator==(const std::normal_distribution<_RealType>& __d1,
      |     ^~~~~~~~
/usr/include/c++/11/bits/random.tcc:1899:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::normal_distribution<_RealType>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::__cxx11::basic_string<char> >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note: candidate: 'template<class _IteratorL, class _IteratorR, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_IteratorL, _Container>&, const __gnu_cxx::__normal_iterator<_IteratorR, _Container>&)'
 1155 |     operator==(const __normal_iterator<_IteratorL, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_IteratorL, _Container>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note: candidate: 'template<class _Iterator, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_Iterator, _Container>&, const __gnu_cxx::__normal_iterator<_Iterator, _Container>&)'
 1163 |     operator==(const __normal_iterator<_Iterator, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_Iterator, _Container>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<char>&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:39:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   39 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/ios_base.h:46,
                 from /usr/include/c++/11/ios:42,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/system_error:362:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_code&)'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:362:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:368:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_condition&)'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:368:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:376:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_condition&)'
  376 |   operator==(const error_condition& __lhs,
      |   ^~~~~~~~
/usr/include/c++/11/system_error:376:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  376 |   operator==(const error_condition& __lhs,
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:408:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_code&)'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:408:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::__cxx11::basic_string<char> >&, const std::allocator<std::__cxx11::basic_string<char> >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::__cxx11::basic_string<char> >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<char>&, const std::allocator<char>&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<char>&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp: In function 'void ____C_A_T_C_H____T_E_S_T____6()':
/testbed/grade_school_test.cpp:51:22: error: no match for 'operator==' (operand types are 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' and 'const std::vector<std::__cxx11::basic_string<char> >')
   51 |     REQUIRE(expected == actual);
      |             ~~~~~~~~ ^~ ~~~~~~
      |             |           |
      |             |           const std::vector<std::__cxx11::basic_string<char> >
      |             const std::map<int, std::vector<std::__cxx11::basic_string<char> > >
In file included from /usr/include/c++/11/bits/stl_algobase.h:64,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_pair.h:466:5: note: candidate: 'template<class _T1, class _T2> constexpr bool std::operator==(const std::pair<_T1, _T2>&, const std::pair<_T1, _T2>&)'
  466 |     operator==(const pair<_T1, _T2>& __x, const pair<_T1, _T2>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_pair.h:466:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::pair<_T1, _T2>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:420:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_Iterator>&)'
  420 |     operator==(const reverse_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:420:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:459:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_IteratorR>&)'
  459 |     operator==(const reverse_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:459:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorR>&)'
 1585 |     operator==(const move_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorL>&)'
 1648 |     operator==(const move_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:218:5: note: candidate: 'template<class _T1, class _T2> bool std::operator==(const std::allocator<_Tp1>&, const std::allocator<_T2>&)'
  218 |     operator==(const allocator<_T1>&, const allocator<_T2>&)
      |     ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:218:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::allocator<_Tp1>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:67,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_vector.h:1892:5: note: candidate: 'template<class _Tp, class _Alloc> bool std::operator==(const std::vector<_Tp, _Alloc>&, const std::vector<_Tp, _Alloc>&)'
 1892 |     operator==(const vector<_Tp, _Alloc>& __x, const vector<_Tp, _Alloc>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_vector.h:1892:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::vector<_Tp, _Alloc>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/char_traits.h:40,
                 from /usr/include/c++/11/string:40,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/postypes.h:222:5: note: candidate: 'template<class _StateT> bool std::operator==(const std::fpos<_StateT>&, const std::fpos<_StateT>&)'
  222 |     operator==(const fpos<_StateT>& __lhs, const fpos<_StateT>& __rhs)
      |     ^~~~~~~~
/usr/include/c++/11/bits/postypes.h:222:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::fpos<_StateT>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:535:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::basic_string_view<_CharT, _Traits>)'
  535 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:535:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:541:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >)'
  541 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:541:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:564:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >, std::basic_string_view<_CharT, _Traits>)'
  564 |     operator==(__type_identity_t<basic_string_view<_CharT, _Traits>> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:564:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'std::vector<std::__cxx11::basic_string<char> >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6226:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6226 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6234:5: note: candidate: 'template<class _CharT> typename __gnu_cxx::__enable_if<std::__is_char<_Tp>::__value, bool>::__type std::operator==(const std::__cxx11::basic_string<_CharT>&, const std::__cxx11::basic_string<_CharT>&)'
 6234 |     operator==(const basic_string<_CharT>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6234:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6248:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const _CharT*)'
 6248 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6248:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6289:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const _CharT*, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6289 |     operator==(const _CharT* __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6289:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   mismatched types 'const _CharT*' and 'std::map<int, std::vector<std::__cxx11::basic_string<char> > >'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/tuple:39,
                 from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/array:276:5: note: candidate: 'template<class _Tp, long unsigned int _Nm> bool std::operator==(const std::array<_Tp, _Nm>&, const std::array<_Tp, _Nm>&)'
  276 |     operator==(const array<_Tp, _Nm>& __one, const array<_Tp, _Nm>& __two)
      |     ^~~~~~~~
/usr/include/c++/11/array:276:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::array<_Tp, _Nm>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/tuple:1524:5: note: candidate: 'template<class ... _TElements, class ... _UElements> constexpr bool std::operator==(const std::tuple<_Tps ...>&, const std::tuple<_Args2 ...>&)'
 1524 |     operator==(const tuple<_TElements...>& __t,
      |     ^~~~~~~~
/usr/include/c++/11/tuple:1524:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::tuple<_Tps ...>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_map.h:1463:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::map<_Key, _Tp, _Compare, _Allocator>&, const std::map<_Key, _Tp, _Compare, _Allocator>&)'
 1463 |     operator==(const map<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_map.h:1463:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::map<_Key, _Tp, _Compare, _Allocator>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:62,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::multimap<_Key, _Tp, _Compare, _Allocator>&, const std::multimap<_Key, _Tp, _Compare, _Allocator>&)'
 1128 |     operator==(const multimap<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::multimap<_Key, _Tp, _Compare, _Allocator>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:718:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(const std::function<_Res(_ArgTypes ...)>&, std::nullptr_t)'
  718 |     operator==(const function<_Res(_Args...)>& __f, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:718:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:725:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(std::nullptr_t, const std::function<_Res(_ArgTypes ...)>&)'
  725 |     operator==(nullptr_t, const function<_Res(_Args...)>& __f) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:725:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2134:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2134 |     operator==(const unordered_map<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2134:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2148:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2148 |     operator==(const unordered_multimap<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2148:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/locale_facets.h:48,
                 from /usr/include/c++/11/bits/basic_ios.h:37,
                 from /usr/include/c++/11/ios:44,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note: candidate: 'template<class _CharT, class _Traits> bool std::operator==(const std::istreambuf_iterator<_CharT, _Traits>&, const std::istreambuf_iterator<_CharT, _Traits>&)'
  226 |     operator==(const istreambuf_iterator<_CharT, _Traits>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::istreambuf_iterator<_CharT, _Traits>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:753:5: note: candidate: 'template<class _Tp, class _Dp, class _Up, class _Ep> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, const std::unique_ptr<_Up, _Ep>&)'
  753 |     operator==(const unique_ptr<_Tp, _Dp>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:753:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:760:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, std::nullptr_t)'
  760 |     operator==(const unique_ptr<_Tp, _Dp>& __x, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:760:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:767:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(std::nullptr_t, const std::unique_ptr<_Tp, _Dp>&)'
  767 |     operator==(nullptr_t, const unique_ptr<_Tp, _Dp>& __x) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:767:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note: candidate: 'template<class _Tp1, class _Tp2, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp1, _Lp>&, const std::__shared_ptr<_Tp2, _Lp>&)'
 1410 |     operator==(const __shared_ptr<_Tp1, _Lp>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp1, _Lp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp, _Lp>&, std::nullptr_t)'
 1416 |     operator==(const __shared_ptr<_Tp, _Lp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(std::nullptr_t, const std::__shared_ptr<_Tp, _Lp>&)'
 1436 |     operator==(nullptr_t, const __shared_ptr<_Tp, _Lp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:437:5: note: candidate: 'template<class _Tp, class _Up> bool std::operator==(const std::shared_ptr<_Tp>&, const std::shared_ptr<_Tp>&)'
  437 |     operator==(const shared_ptr<_Tp>& __a, const shared_ptr<_Up>& __b) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:437:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:443:5: note: candidate: 'template<class _Tp> bool std::operator==(const std::shared_ptr<_Tp>&, std::nullptr_t)'
  443 |     operator==(const shared_ptr<_Tp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:443:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:464:5: note: candidate: 'template<class _Tp> bool std::operator==(std::nullptr_t, const std::shared_ptr<_Tp>&)'
  464 |     operator==(nullptr_t, const shared_ptr<_Tp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:464:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::shared_ptr<_Tp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/random:51,
                 from /testbed/test/catch.hpp:4590,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/random.tcc:1899:5: note: candidate: 'template<class _RealType1> bool std::operator==(const std::normal_distribution<_RealType>&, const std::normal_distribution<_RealType>&)'
 1899 |     operator==(const std::normal_distribution<_RealType>& __d1,
      |     ^~~~~~~~
/usr/include/c++/11/bits/random.tcc:1899:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::normal_distribution<_RealType>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::__cxx11::basic_string<char> >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note: candidate: 'template<class _IteratorL, class _IteratorR, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_IteratorL, _Container>&, const __gnu_cxx::__normal_iterator<_IteratorR, _Container>&)'
 1155 |     operator==(const __normal_iterator<_IteratorL, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_IteratorL, _Container>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note: candidate: 'template<class _Iterator, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_Iterator, _Container>&, const __gnu_cxx::__normal_iterator<_Iterator, _Container>&)'
 1163 |     operator==(const __normal_iterator<_Iterator, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_Iterator, _Container>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<char>&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/ios_base.h:46,
                 from /usr/include/c++/11/ios:42,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/system_error:362:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_code&)'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:362:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:368:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_condition&)'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:368:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:376:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_condition&)'
  376 |   operator==(const error_condition& __lhs,
      |   ^~~~~~~~
/usr/include/c++/11/system_error:376:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  376 |   operator==(const error_condition& __lhs,
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:408:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_code&)'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:408:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::__cxx11::basic_string<char> >&, const std::allocator<std::__cxx11::basic_string<char> >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::__cxx11::basic_string<char> >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<char>&, const std::allocator<char>&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<char>&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:22: error: no match for 'operator==' (operand types are 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' and 'const std::vector<std::__cxx11::basic_string<char> >')
   51 |     REQUIRE(expected == actual);
      |             ~~~~~~~~ ^~ ~~~~~~
      |             |           |
      |             |           const std::vector<std::__cxx11::basic_string<char> >
      |             const std::map<int, std::vector<std::__cxx11::basic_string<char> > >
In file included from /usr/include/c++/11/bits/stl_algobase.h:64,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_pair.h:466:5: note: candidate: 'template<class _T1, class _T2> constexpr bool std::operator==(const std::pair<_T1, _T2>&, const std::pair<_T1, _T2>&)'
  466 |     operator==(const pair<_T1, _T2>& __x, const pair<_T1, _T2>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_pair.h:466:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::pair<_T1, _T2>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:420:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_Iterator>&)'
  420 |     operator==(const reverse_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:420:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:459:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_IteratorR>&)'
  459 |     operator==(const reverse_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:459:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorR>&)'
 1585 |     operator==(const move_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorL>&)'
 1648 |     operator==(const move_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:218:5: note: candidate: 'template<class _T1, class _T2> bool std::operator==(const std::allocator<_Tp1>&, const std::allocator<_T2>&)'
  218 |     operator==(const allocator<_T1>&, const allocator<_T2>&)
      |     ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:218:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::allocator<_Tp1>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:67,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_vector.h:1892:5: note: candidate: 'template<class _Tp, class _Alloc> bool std::operator==(const std::vector<_Tp, _Alloc>&, const std::vector<_Tp, _Alloc>&)'
 1892 |     operator==(const vector<_Tp, _Alloc>& __x, const vector<_Tp, _Alloc>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_vector.h:1892:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::vector<_Tp, _Alloc>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/char_traits.h:40,
                 from /usr/include/c++/11/string:40,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/postypes.h:222:5: note: candidate: 'template<class _StateT> bool std::operator==(const std::fpos<_StateT>&, const std::fpos<_StateT>&)'
  222 |     operator==(const fpos<_StateT>& __lhs, const fpos<_StateT>& __rhs)
      |     ^~~~~~~~
/usr/include/c++/11/bits/postypes.h:222:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::fpos<_StateT>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:535:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::basic_string_view<_CharT, _Traits>)'
  535 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:535:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:541:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >)'
  541 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:541:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:564:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >, std::basic_string_view<_CharT, _Traits>)'
  564 |     operator==(__type_identity_t<basic_string_view<_CharT, _Traits>> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:564:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'std::vector<std::__cxx11::basic_string<char> >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6226:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6226 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6234:5: note: candidate: 'template<class _CharT> typename __gnu_cxx::__enable_if<std::__is_char<_Tp>::__value, bool>::__type std::operator==(const std::__cxx11::basic_string<_CharT>&, const std::__cxx11::basic_string<_CharT>&)'
 6234 |     operator==(const basic_string<_CharT>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6234:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6248:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const _CharT*)'
 6248 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6248:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6289:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const _CharT*, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6289 |     operator==(const _CharT* __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6289:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   mismatched types 'const _CharT*' and 'std::map<int, std::vector<std::__cxx11::basic_string<char> > >'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/tuple:39,
                 from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/array:276:5: note: candidate: 'template<class _Tp, long unsigned int _Nm> bool std::operator==(const std::array<_Tp, _Nm>&, const std::array<_Tp, _Nm>&)'
  276 |     operator==(const array<_Tp, _Nm>& __one, const array<_Tp, _Nm>& __two)
      |     ^~~~~~~~
/usr/include/c++/11/array:276:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::array<_Tp, _Nm>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/tuple:1524:5: note: candidate: 'template<class ... _TElements, class ... _UElements> constexpr bool std::operator==(const std::tuple<_Tps ...>&, const std::tuple<_Args2 ...>&)'
 1524 |     operator==(const tuple<_TElements...>& __t,
      |     ^~~~~~~~
/usr/include/c++/11/tuple:1524:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::tuple<_Tps ...>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_map.h:1463:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::map<_Key, _Tp, _Compare, _Allocator>&, const std::map<_Key, _Tp, _Compare, _Allocator>&)'
 1463 |     operator==(const map<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_map.h:1463:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::map<_Key, _Tp, _Compare, _Allocator>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:62,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::multimap<_Key, _Tp, _Compare, _Allocator>&, const std::multimap<_Key, _Tp, _Compare, _Allocator>&)'
 1128 |     operator==(const multimap<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::multimap<_Key, _Tp, _Compare, _Allocator>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:718:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(const std::function<_Res(_ArgTypes ...)>&, std::nullptr_t)'
  718 |     operator==(const function<_Res(_Args...)>& __f, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:718:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:725:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(std::nullptr_t, const std::function<_Res(_ArgTypes ...)>&)'
  725 |     operator==(nullptr_t, const function<_Res(_Args...)>& __f) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:725:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2134:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2134 |     operator==(const unordered_map<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2134:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2148:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2148 |     operator==(const unordered_multimap<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2148:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/locale_facets.h:48,
                 from /usr/include/c++/11/bits/basic_ios.h:37,
                 from /usr/include/c++/11/ios:44,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note: candidate: 'template<class _CharT, class _Traits> bool std::operator==(const std::istreambuf_iterator<_CharT, _Traits>&, const std::istreambuf_iterator<_CharT, _Traits>&)'
  226 |     operator==(const istreambuf_iterator<_CharT, _Traits>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::istreambuf_iterator<_CharT, _Traits>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:753:5: note: candidate: 'template<class _Tp, class _Dp, class _Up, class _Ep> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, const std::unique_ptr<_Up, _Ep>&)'
  753 |     operator==(const unique_ptr<_Tp, _Dp>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:753:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:760:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, std::nullptr_t)'
  760 |     operator==(const unique_ptr<_Tp, _Dp>& __x, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:760:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:767:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(std::nullptr_t, const std::unique_ptr<_Tp, _Dp>&)'
  767 |     operator==(nullptr_t, const unique_ptr<_Tp, _Dp>& __x) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:767:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note: candidate: 'template<class _Tp1, class _Tp2, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp1, _Lp>&, const std::__shared_ptr<_Tp2, _Lp>&)'
 1410 |     operator==(const __shared_ptr<_Tp1, _Lp>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp1, _Lp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp, _Lp>&, std::nullptr_t)'
 1416 |     operator==(const __shared_ptr<_Tp, _Lp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(std::nullptr_t, const std::__shared_ptr<_Tp, _Lp>&)'
 1436 |     operator==(nullptr_t, const __shared_ptr<_Tp, _Lp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:437:5: note: candidate: 'template<class _Tp, class _Up> bool std::operator==(const std::shared_ptr<_Tp>&, const std::shared_ptr<_Tp>&)'
  437 |     operator==(const shared_ptr<_Tp>& __a, const shared_ptr<_Up>& __b) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:437:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:443:5: note: candidate: 'template<class _Tp> bool std::operator==(const std::shared_ptr<_Tp>&, std::nullptr_t)'
  443 |     operator==(const shared_ptr<_Tp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:443:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:464:5: note: candidate: 'template<class _Tp> bool std::operator==(std::nullptr_t, const std::shared_ptr<_Tp>&)'
  464 |     operator==(nullptr_t, const shared_ptr<_Tp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:464:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::shared_ptr<_Tp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/random:51,
                 from /testbed/test/catch.hpp:4590,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/random.tcc:1899:5: note: candidate: 'template<class _RealType1> bool std::operator==(const std::normal_distribution<_RealType>&, const std::normal_distribution<_RealType>&)'
 1899 |     operator==(const std::normal_distribution<_RealType>& __d1,
      |     ^~~~~~~~
/usr/include/c++/11/bits/random.tcc:1899:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::normal_distribution<_RealType>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::__cxx11::basic_string<char> >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note: candidate: 'template<class _IteratorL, class _IteratorR, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_IteratorL, _Container>&, const __gnu_cxx::__normal_iterator<_IteratorR, _Container>&)'
 1155 |     operator==(const __normal_iterator<_IteratorL, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_IteratorL, _Container>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note: candidate: 'template<class _Iterator, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_Iterator, _Container>&, const __gnu_cxx::__normal_iterator<_Iterator, _Container>&)'
 1163 |     operator==(const __normal_iterator<_Iterator, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_Iterator, _Container>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<char>&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:51:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   51 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/ios_base.h:46,
                 from /usr/include/c++/11/ios:42,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/system_error:362:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_code&)'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:362:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:368:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_condition&)'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:368:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:376:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_condition&)'
  376 |   operator==(const error_condition& __lhs,
      |   ^~~~~~~~
/usr/include/c++/11/system_error:376:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  376 |   operator==(const error_condition& __lhs,
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:408:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_code&)'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:408:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::__cxx11::basic_string<char> >&, const std::allocator<std::__cxx11::basic_string<char> >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::__cxx11::basic_string<char> >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<char>&, const std::allocator<char>&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<char>&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp: In function 'void ____C_A_T_C_H____T_E_S_T____12()':
/testbed/grade_school_test.cpp:90:22: error: no match for 'operator==' (operand types are 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' and 'const std::vector<std::__cxx11::basic_string<char> >')
   90 |     REQUIRE(expected == actual);
      |             ~~~~~~~~ ^~ ~~~~~~
      |             |           |
      |             |           const std::vector<std::__cxx11::basic_string<char> >
      |             const std::map<int, std::vector<std::__cxx11::basic_string<char> > >
In file included from /usr/include/c++/11/bits/stl_algobase.h:64,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_pair.h:466:5: note: candidate: 'template<class _T1, class _T2> constexpr bool std::operator==(const std::pair<_T1, _T2>&, const std::pair<_T1, _T2>&)'
  466 |     operator==(const pair<_T1, _T2>& __x, const pair<_T1, _T2>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_pair.h:466:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::pair<_T1, _T2>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:420:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_Iterator>&)'
  420 |     operator==(const reverse_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:420:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:459:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_IteratorR>&)'
  459 |     operator==(const reverse_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:459:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorR>&)'
 1585 |     operator==(const move_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorL>&)'
 1648 |     operator==(const move_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:218:5: note: candidate: 'template<class _T1, class _T2> bool std::operator==(const std::allocator<_Tp1>&, const std::allocator<_T2>&)'
  218 |     operator==(const allocator<_T1>&, const allocator<_T2>&)
      |     ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:218:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::allocator<_Tp1>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:67,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_vector.h:1892:5: note: candidate: 'template<class _Tp, class _Alloc> bool std::operator==(const std::vector<_Tp, _Alloc>&, const std::vector<_Tp, _Alloc>&)'
 1892 |     operator==(const vector<_Tp, _Alloc>& __x, const vector<_Tp, _Alloc>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_vector.h:1892:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::vector<_Tp, _Alloc>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/char_traits.h:40,
                 from /usr/include/c++/11/string:40,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/postypes.h:222:5: note: candidate: 'template<class _StateT> bool std::operator==(const std::fpos<_StateT>&, const std::fpos<_StateT>&)'
  222 |     operator==(const fpos<_StateT>& __lhs, const fpos<_StateT>& __rhs)
      |     ^~~~~~~~
/usr/include/c++/11/bits/postypes.h:222:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::fpos<_StateT>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:535:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::basic_string_view<_CharT, _Traits>)'
  535 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:535:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:541:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >)'
  541 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:541:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:564:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >, std::basic_string_view<_CharT, _Traits>)'
  564 |     operator==(__type_identity_t<basic_string_view<_CharT, _Traits>> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:564:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'std::vector<std::__cxx11::basic_string<char> >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6226:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6226 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6234:5: note: candidate: 'template<class _CharT> typename __gnu_cxx::__enable_if<std::__is_char<_Tp>::__value, bool>::__type std::operator==(const std::__cxx11::basic_string<_CharT>&, const std::__cxx11::basic_string<_CharT>&)'
 6234 |     operator==(const basic_string<_CharT>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6234:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6248:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const _CharT*)'
 6248 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6248:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6289:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const _CharT*, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6289 |     operator==(const _CharT* __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6289:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   mismatched types 'const _CharT*' and 'std::map<int, std::vector<std::__cxx11::basic_string<char> > >'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/tuple:39,
                 from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/array:276:5: note: candidate: 'template<class _Tp, long unsigned int _Nm> bool std::operator==(const std::array<_Tp, _Nm>&, const std::array<_Tp, _Nm>&)'
  276 |     operator==(const array<_Tp, _Nm>& __one, const array<_Tp, _Nm>& __two)
      |     ^~~~~~~~
/usr/include/c++/11/array:276:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::array<_Tp, _Nm>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/tuple:1524:5: note: candidate: 'template<class ... _TElements, class ... _UElements> constexpr bool std::operator==(const std::tuple<_Tps ...>&, const std::tuple<_Args2 ...>&)'
 1524 |     operator==(const tuple<_TElements...>& __t,
      |     ^~~~~~~~
/usr/include/c++/11/tuple:1524:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::tuple<_Tps ...>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_map.h:1463:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::map<_Key, _Tp, _Compare, _Allocator>&, const std::map<_Key, _Tp, _Compare, _Allocator>&)'
 1463 |     operator==(const map<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_map.h:1463:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::map<_Key, _Tp, _Compare, _Allocator>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:62,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::multimap<_Key, _Tp, _Compare, _Allocator>&, const std::multimap<_Key, _Tp, _Compare, _Allocator>&)'
 1128 |     operator==(const multimap<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::multimap<_Key, _Tp, _Compare, _Allocator>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:718:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(const std::function<_Res(_ArgTypes ...)>&, std::nullptr_t)'
  718 |     operator==(const function<_Res(_Args...)>& __f, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:718:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:725:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(std::nullptr_t, const std::function<_Res(_ArgTypes ...)>&)'
  725 |     operator==(nullptr_t, const function<_Res(_Args...)>& __f) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:725:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2134:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2134 |     operator==(const unordered_map<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2134:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2148:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2148 |     operator==(const unordered_multimap<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2148:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/locale_facets.h:48,
                 from /usr/include/c++/11/bits/basic_ios.h:37,
                 from /usr/include/c++/11/ios:44,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note: candidate: 'template<class _CharT, class _Traits> bool std::operator==(const std::istreambuf_iterator<_CharT, _Traits>&, const std::istreambuf_iterator<_CharT, _Traits>&)'
  226 |     operator==(const istreambuf_iterator<_CharT, _Traits>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::istreambuf_iterator<_CharT, _Traits>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:753:5: note: candidate: 'template<class _Tp, class _Dp, class _Up, class _Ep> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, const std::unique_ptr<_Up, _Ep>&)'
  753 |     operator==(const unique_ptr<_Tp, _Dp>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:753:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:760:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, std::nullptr_t)'
  760 |     operator==(const unique_ptr<_Tp, _Dp>& __x, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:760:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:767:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(std::nullptr_t, const std::unique_ptr<_Tp, _Dp>&)'
  767 |     operator==(nullptr_t, const unique_ptr<_Tp, _Dp>& __x) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:767:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note: candidate: 'template<class _Tp1, class _Tp2, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp1, _Lp>&, const std::__shared_ptr<_Tp2, _Lp>&)'
 1410 |     operator==(const __shared_ptr<_Tp1, _Lp>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp1, _Lp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp, _Lp>&, std::nullptr_t)'
 1416 |     operator==(const __shared_ptr<_Tp, _Lp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(std::nullptr_t, const std::__shared_ptr<_Tp, _Lp>&)'
 1436 |     operator==(nullptr_t, const __shared_ptr<_Tp, _Lp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:437:5: note: candidate: 'template<class _Tp, class _Up> bool std::operator==(const std::shared_ptr<_Tp>&, const std::shared_ptr<_Tp>&)'
  437 |     operator==(const shared_ptr<_Tp>& __a, const shared_ptr<_Up>& __b) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:437:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:443:5: note: candidate: 'template<class _Tp> bool std::operator==(const std::shared_ptr<_Tp>&, std::nullptr_t)'
  443 |     operator==(const shared_ptr<_Tp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:443:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:464:5: note: candidate: 'template<class _Tp> bool std::operator==(std::nullptr_t, const std::shared_ptr<_Tp>&)'
  464 |     operator==(nullptr_t, const shared_ptr<_Tp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:464:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::shared_ptr<_Tp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/random:51,
                 from /testbed/test/catch.hpp:4590,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/random.tcc:1899:5: note: candidate: 'template<class _RealType1> bool std::operator==(const std::normal_distribution<_RealType>&, const std::normal_distribution<_RealType>&)'
 1899 |     operator==(const std::normal_distribution<_RealType>& __d1,
      |     ^~~~~~~~
/usr/include/c++/11/bits/random.tcc:1899:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::normal_distribution<_RealType>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::__cxx11::basic_string<char> >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note: candidate: 'template<class _IteratorL, class _IteratorR, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_IteratorL, _Container>&, const __gnu_cxx::__normal_iterator<_IteratorR, _Container>&)'
 1155 |     operator==(const __normal_iterator<_IteratorL, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_IteratorL, _Container>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note: candidate: 'template<class _Iterator, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_Iterator, _Container>&, const __gnu_cxx::__normal_iterator<_Iterator, _Container>&)'
 1163 |     operator==(const __normal_iterator<_Iterator, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_Iterator, _Container>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<char>&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/ios_base.h:46,
                 from /usr/include/c++/11/ios:42,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/system_error:362:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_code&)'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:362:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:368:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_condition&)'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:368:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:376:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_condition&)'
  376 |   operator==(const error_condition& __lhs,
      |   ^~~~~~~~
/usr/include/c++/11/system_error:376:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  376 |   operator==(const error_condition& __lhs,
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:408:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_code&)'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:408:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::__cxx11::basic_string<char> >&, const std::allocator<std::__cxx11::basic_string<char> >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::__cxx11::basic_string<char> >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<char>&, const std::allocator<char>&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<char>&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:22: error: no match for 'operator==' (operand types are 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' and 'const std::vector<std::__cxx11::basic_string<char> >')
   90 |     REQUIRE(expected == actual);
      |             ~~~~~~~~ ^~ ~~~~~~
      |             |           |
      |             |           const std::vector<std::__cxx11::basic_string<char> >
      |             const std::map<int, std::vector<std::__cxx11::basic_string<char> > >
In file included from /usr/include/c++/11/bits/stl_algobase.h:64,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_pair.h:466:5: note: candidate: 'template<class _T1, class _T2> constexpr bool std::operator==(const std::pair<_T1, _T2>&, const std::pair<_T1, _T2>&)'
  466 |     operator==(const pair<_T1, _T2>& __x, const pair<_T1, _T2>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_pair.h:466:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::pair<_T1, _T2>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:420:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_Iterator>&)'
  420 |     operator==(const reverse_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:420:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:459:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_IteratorR>&)'
  459 |     operator==(const reverse_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:459:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorR>&)'
 1585 |     operator==(const move_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorL>&)'
 1648 |     operator==(const move_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:218:5: note: candidate: 'template<class _T1, class _T2> bool std::operator==(const std::allocator<_Tp1>&, const std::allocator<_T2>&)'
  218 |     operator==(const allocator<_T1>&, const allocator<_T2>&)
      |     ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:218:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::allocator<_Tp1>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/vector:67,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_vector.h:1892:5: note: candidate: 'template<class _Tp, class _Alloc> bool std::operator==(const std::vector<_Tp, _Alloc>&, const std::vector<_Tp, _Alloc>&)'
 1892 |     operator==(const vector<_Tp, _Alloc>& __x, const vector<_Tp, _Alloc>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_vector.h:1892:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::vector<_Tp, _Alloc>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/char_traits.h:40,
                 from /usr/include/c++/11/string:40,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/postypes.h:222:5: note: candidate: 'template<class _StateT> bool std::operator==(const std::fpos<_StateT>&, const std::fpos<_StateT>&)'
  222 |     operator==(const fpos<_StateT>& __lhs, const fpos<_StateT>& __rhs)
      |     ^~~~~~~~
/usr/include/c++/11/bits/postypes.h:222:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::fpos<_StateT>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:535:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::basic_string_view<_CharT, _Traits>)'
  535 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:535:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:541:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >)'
  541 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:541:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:564:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >, std::basic_string_view<_CharT, _Traits>)'
  564 |     operator==(__type_identity_t<basic_string_view<_CharT, _Traits>> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:564:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'std::vector<std::__cxx11::basic_string<char> >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6226:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6226 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6234:5: note: candidate: 'template<class _CharT> typename __gnu_cxx::__enable_if<std::__is_char<_Tp>::__value, bool>::__type std::operator==(const std::__cxx11::basic_string<_CharT>&, const std::__cxx11::basic_string<_CharT>&)'
 6234 |     operator==(const basic_string<_CharT>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6234:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6248:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const _CharT*)'
 6248 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6248:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6289:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const _CharT*, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6289 |     operator==(const _CharT* __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6289:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   mismatched types 'const _CharT*' and 'std::map<int, std::vector<std::__cxx11::basic_string<char> > >'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/tuple:39,
                 from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/array:276:5: note: candidate: 'template<class _Tp, long unsigned int _Nm> bool std::operator==(const std::array<_Tp, _Nm>&, const std::array<_Tp, _Nm>&)'
  276 |     operator==(const array<_Tp, _Nm>& __one, const array<_Tp, _Nm>& __two)
      |     ^~~~~~~~
/usr/include/c++/11/array:276:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::array<_Tp, _Nm>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/tuple:1524:5: note: candidate: 'template<class ... _TElements, class ... _UElements> constexpr bool std::operator==(const std::tuple<_Tps ...>&, const std::tuple<_Args2 ...>&)'
 1524 |     operator==(const tuple<_TElements...>& __t,
      |     ^~~~~~~~
/usr/include/c++/11/tuple:1524:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::tuple<_Tps ...>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_map.h:1463:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::map<_Key, _Tp, _Compare, _Allocator>&, const std::map<_Key, _Tp, _Compare, _Allocator>&)'
 1463 |     operator==(const map<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_map.h:1463:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::map<_Key, _Tp, _Compare, _Allocator>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/map:62,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::multimap<_Key, _Tp, _Compare, _Allocator>&, const std::multimap<_Key, _Tp, _Compare, _Allocator>&)'
 1128 |     operator==(const multimap<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::multimap<_Key, _Tp, _Compare, _Allocator>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:718:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(const std::function<_Res(_ArgTypes ...)>&, std::nullptr_t)'
  718 |     operator==(const function<_Res(_Args...)>& __f, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:718:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:725:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(std::nullptr_t, const std::function<_Res(_ArgTypes ...)>&)'
  725 |     operator==(nullptr_t, const function<_Res(_Args...)>& __f) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:725:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2134:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2134 |     operator==(const unordered_map<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2134:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2148:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2148 |     operator==(const unordered_multimap<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2148:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/locale_facets.h:48,
                 from /usr/include/c++/11/bits/basic_ios.h:37,
                 from /usr/include/c++/11/ios:44,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note: candidate: 'template<class _CharT, class _Traits> bool std::operator==(const std::istreambuf_iterator<_CharT, _Traits>&, const std::istreambuf_iterator<_CharT, _Traits>&)'
  226 |     operator==(const istreambuf_iterator<_CharT, _Traits>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::istreambuf_iterator<_CharT, _Traits>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:753:5: note: candidate: 'template<class _Tp, class _Dp, class _Up, class _Ep> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, const std::unique_ptr<_Up, _Ep>&)'
  753 |     operator==(const unique_ptr<_Tp, _Dp>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:753:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:760:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, std::nullptr_t)'
  760 |     operator==(const unique_ptr<_Tp, _Dp>& __x, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:760:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:767:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(std::nullptr_t, const std::unique_ptr<_Tp, _Dp>&)'
  767 |     operator==(nullptr_t, const unique_ptr<_Tp, _Dp>& __x) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:767:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note: candidate: 'template<class _Tp1, class _Tp2, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp1, _Lp>&, const std::__shared_ptr<_Tp2, _Lp>&)'
 1410 |     operator==(const __shared_ptr<_Tp1, _Lp>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp1, _Lp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp, _Lp>&, std::nullptr_t)'
 1416 |     operator==(const __shared_ptr<_Tp, _Lp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(std::nullptr_t, const std::__shared_ptr<_Tp, _Lp>&)'
 1436 |     operator==(nullptr_t, const __shared_ptr<_Tp, _Lp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:437:5: note: candidate: 'template<class _Tp, class _Up> bool std::operator==(const std::shared_ptr<_Tp>&, const std::shared_ptr<_Tp>&)'
  437 |     operator==(const shared_ptr<_Tp>& __a, const shared_ptr<_Up>& __b) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:437:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:443:5: note: candidate: 'template<class _Tp> bool std::operator==(const std::shared_ptr<_Tp>&, std::nullptr_t)'
  443 |     operator==(const shared_ptr<_Tp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:443:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:464:5: note: candidate: 'template<class _Tp> bool std::operator==(std::nullptr_t, const std::shared_ptr<_Tp>&)'
  464 |     operator==(nullptr_t, const shared_ptr<_Tp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:464:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::shared_ptr<_Tp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/random:51,
                 from /testbed/test/catch.hpp:4590,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/random.tcc:1899:5: note: candidate: 'template<class _RealType1> bool std::operator==(const std::normal_distribution<_RealType>&, const std::normal_distribution<_RealType>&)'
 1899 |     operator==(const std::normal_distribution<_RealType>& __d1,
      |     ^~~~~~~~
/usr/include/c++/11/bits/random.tcc:1899:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::normal_distribution<_RealType>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::__cxx11::basic_string<char> >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note: candidate: 'template<class _IteratorL, class _IteratorR, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_IteratorL, _Container>&, const __gnu_cxx::__normal_iterator<_IteratorR, _Container>&)'
 1155 |     operator==(const __normal_iterator<_IteratorL, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_IteratorL, _Container>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note: candidate: 'template<class _Iterator, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_Iterator, _Container>&, const __gnu_cxx::__normal_iterator<_Iterator, _Container>&)'
 1163 |     operator==(const __normal_iterator<_Iterator, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_Iterator, _Container>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<char>&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/grade_school_test.cpp:90:25: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
   90 |     REQUIRE(expected == actual);
      |                         ^~~~~~
In file included from /usr/include/c++/11/bits/ios_base.h:46,
                 from /usr/include/c++/11/ios:42,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/system_error:362:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_code&)'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:362:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:368:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_condition&)'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:368:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:376:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_condition&)'
  376 |   operator==(const error_condition& __lhs,
      |   ^~~~~~~~
/usr/include/c++/11/system_error:376:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  376 |   operator==(const error_condition& __lhs,
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:408:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_code&)'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:408:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::__cxx11::basic_string<char> >&, const std::allocator<std::__cxx11::basic_string<char> >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::__cxx11::basic_string<char> >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<char>&, const std::allocator<char>&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<char>&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp: In instantiation of 'bool Catch::compareEqual(const LhsT&, const RhsT&) [with LhsT = std::map<int, std::vector<std::__cxx11::basic_string<char> > >; RhsT = std::vector<std::__cxx11::basic_string<char> >]':
/testbed/test/catch.hpp:2343:34:   required from 'const Catch::BinaryExpr<LhsT, const RhsT&> Catch::ExprLhs<LhsT>::operator==(const RhsT&) [with RhsT = std::vector<std::__cxx11::basic_string<char> >; LhsT = const std::map<int, std::vector<std::__cxx11::basic_string<char> > >&]'
/testbed/grade_school_test.cpp:26:5:   required from here
/testbed/test/catch.hpp:2314:98: error: no match for 'operator==' (operand types are 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' and 'const std::vector<std::__cxx11::basic_string<char> >')
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:64,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_pair.h:466:5: note: candidate: 'template<class _T1, class _T2> constexpr bool std::operator==(const std::pair<_T1, _T2>&, const std::pair<_T1, _T2>&)'
  466 |     operator==(const pair<_T1, _T2>& __x, const pair<_T1, _T2>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_pair.h:466:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::pair<_T1, _T2>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:420:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_Iterator>&)'
  420 |     operator==(const reverse_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:420:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:459:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::reverse_iterator<_Iterator>&, const std::reverse_iterator<_IteratorR>&)'
  459 |     operator==(const reverse_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:459:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::reverse_iterator<_Iterator>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note: candidate: 'template<class _IteratorL, class _IteratorR> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorR>&)'
 1585 |     operator==(const move_iterator<_IteratorL>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1585:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note: candidate: 'template<class _Iterator> constexpr bool std::operator==(const std::move_iterator<_IteratorL>&, const std::move_iterator<_IteratorL>&)'
 1648 |     operator==(const move_iterator<_Iterator>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1648:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::move_iterator<_IteratorL>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:218:5: note: candidate: 'template<class _T1, class _T2> bool std::operator==(const std::allocator<_Tp1>&, const std::allocator<_T2>&)'
  218 |     operator==(const allocator<_T1>&, const allocator<_T2>&)
      |     ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:218:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::allocator<_Tp1>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/vector:67,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_vector.h:1892:5: note: candidate: 'template<class _Tp, class _Alloc> bool std::operator==(const std::vector<_Tp, _Alloc>&, const std::vector<_Tp, _Alloc>&)'
 1892 |     operator==(const vector<_Tp, _Alloc>& __x, const vector<_Tp, _Alloc>& __y)
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_vector.h:1892:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::vector<_Tp, _Alloc>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/char_traits.h:40,
                 from /usr/include/c++/11/string:40,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/postypes.h:222:5: note: candidate: 'template<class _StateT> bool std::operator==(const std::fpos<_StateT>&, const std::fpos<_StateT>&)'
  222 |     operator==(const fpos<_StateT>& __lhs, const fpos<_StateT>& __rhs)
      |     ^~~~~~~~
/usr/include/c++/11/bits/postypes.h:222:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::fpos<_StateT>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:535:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::basic_string_view<_CharT, _Traits>)'
  535 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:535:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:541:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::basic_string_view<_CharT, _Traits>, std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >)'
  541 |     operator==(basic_string_view<_CharT, _Traits> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:541:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/basic_string.h:48,
                 from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/string_view:564:5: note: candidate: 'template<class _CharT, class _Traits> constexpr bool std::operator==(std::__type_identity_t<std::basic_string_view<_CharT, _Traits> >, std::basic_string_view<_CharT, _Traits>)'
  564 |     operator==(__type_identity_t<basic_string_view<_CharT, _Traits>> __x,
      |     ^~~~~~~~
/usr/include/c++/11/string_view:564:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'std::vector<std::__cxx11::basic_string<char> >' is not derived from 'std::basic_string_view<_CharT, _Traits>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6226:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6226 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6234:5: note: candidate: 'template<class _CharT> typename __gnu_cxx::__enable_if<std::__is_char<_Tp>::__value, bool>::__type std::operator==(const std::__cxx11::basic_string<_CharT>&, const std::__cxx11::basic_string<_CharT>&)'
 6234 |     operator==(const basic_string<_CharT>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6234:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6248:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&, const _CharT*)'
 6248 |     operator==(const basic_string<_CharT, _Traits, _Alloc>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6248:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/string:55,
                 from /testbed/grade_school.h:5,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/basic_string.h:6289:5: note: candidate: 'template<class _CharT, class _Traits, class _Alloc> bool std::operator==(const _CharT*, const std::__cxx11::basic_string<_CharT, _Traits, _Allocator>&)'
 6289 |     operator==(const _CharT* __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/basic_string.h:6289:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   mismatched types 'const _CharT*' and 'std::map<int, std::vector<std::__cxx11::basic_string<char> > >'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/tuple:39,
                 from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/array:276:5: note: candidate: 'template<class _Tp, long unsigned int _Nm> bool std::operator==(const std::array<_Tp, _Nm>&, const std::array<_Tp, _Nm>&)'
  276 |     operator==(const array<_Tp, _Nm>& __one, const array<_Tp, _Nm>& __two)
      |     ^~~~~~~~
/usr/include/c++/11/array:276:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::array<_Tp, _Nm>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/stl_map.h:63,
                 from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/tuple:1524:5: note: candidate: 'template<class ... _TElements, class ... _UElements> constexpr bool std::operator==(const std::tuple<_Tps ...>&, const std::tuple<_Args2 ...>&)'
 1524 |     operator==(const tuple<_TElements...>& __t,
      |     ^~~~~~~~
/usr/include/c++/11/tuple:1524:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::tuple<_Tps ...>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/map:61,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_map.h:1463:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::map<_Key, _Tp, _Compare, _Allocator>&, const std::map<_Key, _Tp, _Compare, _Allocator>&)'
 1463 |     operator==(const map<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_map.h:1463:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::map<_Key, _Tp, _Compare, _Allocator>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/map:62,
                 from /testbed/grade_school.h:6,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note: candidate: 'template<class _Key, class _Tp, class _Compare, class _Alloc> bool std::operator==(const std::multimap<_Key, _Tp, _Compare, _Allocator>&, const std::multimap<_Key, _Tp, _Compare, _Allocator>&)'
 1128 |     operator==(const multimap<_Key, _Tp, _Compare, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_multimap.h:1128:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::multimap<_Key, _Tp, _Compare, _Allocator>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:718:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(const std::function<_Res(_ArgTypes ...)>&, std::nullptr_t)'
  718 |     operator==(const function<_Res(_Args...)>& __f, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:718:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/functional:59,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/std_function.h:725:5: note: candidate: 'template<class _Res, class ... _Args> bool std::operator==(std::nullptr_t, const std::function<_Res(_ArgTypes ...)>&)'
  725 |     operator==(nullptr_t, const function<_Res(_Args...)>& __f) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/std_function.h:725:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::function<_Res(_ArgTypes ...)>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2134:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2134 |     operator==(const unordered_map<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2134:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_map<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/unordered_map:47,
                 from /usr/include/c++/11/functional:61,
                 from /usr/include/c++/11/pstl/glue_algorithm_defs.h:13,
                 from /usr/include/c++/11/algorithm:74,
                 from /testbed/grade_school.h:8,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/unordered_map.h:2148:5: note: candidate: 'template<class _Key1, class _Tp1, class _Hash1, class _Pred1, class _Alloc1> bool std::operator==(const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&, const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>&)'
 2148 |     operator==(const unordered_multimap<_Key, _Tp, _Hash, _Pred, _Alloc>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unordered_map.h:2148:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unordered_multimap<_Key1, _Tp1, _Hash1, _Pred1, _Alloc1>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/locale_facets.h:48,
                 from /usr/include/c++/11/bits/basic_ios.h:37,
                 from /usr/include/c++/11/ios:44,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note: candidate: 'template<class _CharT, class _Traits> bool std::operator==(const std::istreambuf_iterator<_CharT, _Traits>&, const std::istreambuf_iterator<_CharT, _Traits>&)'
  226 |     operator==(const istreambuf_iterator<_CharT, _Traits>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/streambuf_iterator.h:226:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::istreambuf_iterator<_CharT, _Traits>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:753:5: note: candidate: 'template<class _Tp, class _Dp, class _Up, class _Ep> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, const std::unique_ptr<_Up, _Ep>&)'
  753 |     operator==(const unique_ptr<_Tp, _Dp>& __x,
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:753:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:760:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(const std::unique_ptr<_Tp, _Dp>&, std::nullptr_t)'
  760 |     operator==(const unique_ptr<_Tp, _Dp>& __x, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:760:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/memory:76,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/unique_ptr.h:767:5: note: candidate: 'template<class _Tp, class _Dp> bool std::operator==(std::nullptr_t, const std::unique_ptr<_Tp, _Dp>&)'
  767 |     operator==(nullptr_t, const unique_ptr<_Tp, _Dp>& __x) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/unique_ptr.h:767:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::unique_ptr<_Tp, _Dp>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note: candidate: 'template<class _Tp1, class _Tp2, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp1, _Lp>&, const std::__shared_ptr<_Tp2, _Lp>&)'
 1410 |     operator==(const __shared_ptr<_Tp1, _Lp>& __a,
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1410:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp1, _Lp>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(const std::__shared_ptr<_Tp, _Lp>&, std::nullptr_t)'
 1416 |     operator==(const __shared_ptr<_Tp, _Lp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1416:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/shared_ptr.h:53,
                 from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note: candidate: 'template<class _Tp, __gnu_cxx::_Lock_policy _Lp> bool std::operator==(std::nullptr_t, const std::__shared_ptr<_Tp, _Lp>&)'
 1436 |     operator==(nullptr_t, const __shared_ptr<_Tp, _Lp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr_base.h:1436:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::__shared_ptr<_Tp, _Lp>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:437:5: note: candidate: 'template<class _Tp, class _Up> bool std::operator==(const std::shared_ptr<_Tp>&, const std::shared_ptr<_Tp>&)'
  437 |     operator==(const shared_ptr<_Tp>& __a, const shared_ptr<_Up>& __b) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:437:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:443:5: note: candidate: 'template<class _Tp> bool std::operator==(const std::shared_ptr<_Tp>&, std::nullptr_t)'
  443 |     operator==(const shared_ptr<_Tp>& __a, nullptr_t) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:443:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::shared_ptr<_Tp>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/memory:77,
                 from /testbed/test/catch.hpp:2946,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/shared_ptr.h:464:5: note: candidate: 'template<class _Tp> bool std::operator==(std::nullptr_t, const std::shared_ptr<_Tp>&)'
  464 |     operator==(nullptr_t, const shared_ptr<_Tp>& __a) noexcept
      |     ^~~~~~~~
/usr/include/c++/11/bits/shared_ptr.h:464:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const std::shared_ptr<_Tp>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/random:51,
                 from /testbed/test/catch.hpp:4590,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/bits/random.tcc:1899:5: note: candidate: 'template<class _RealType1> bool std::operator==(const std::normal_distribution<_RealType>&, const std::normal_distribution<_RealType>&)'
 1899 |     operator==(const std::normal_distribution<_RealType>& __d1,
      |     ^~~~~~~~
/usr/include/c++/11/bits/random.tcc:1899:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const std::normal_distribution<_RealType>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<std::__cxx11::basic_string<char> >&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note: candidate: 'template<class _IteratorL, class _IteratorR, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_IteratorL, _Container>&, const __gnu_cxx::__normal_iterator<_IteratorR, _Container>&)'
 1155 |     operator==(const __normal_iterator<_IteratorL, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1155:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_IteratorL, _Container>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/stl_algobase.h:67,
                 from /usr/include/c++/11/vector:60,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note: candidate: 'template<class _Iterator, class _Container> bool __gnu_cxx::operator==(const __gnu_cxx::__normal_iterator<_Iterator, _Container>&, const __gnu_cxx::__normal_iterator<_Iterator, _Container>&)'
 1163 |     operator==(const __normal_iterator<_Iterator, _Container>& __lhs,
      |     ^~~~~~~~
/usr/include/c++/11/bits/stl_iterator.h:1163:5: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' is not derived from 'const __gnu_cxx::__normal_iterator<_Iterator, _Container>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/x86_64-linux-gnu/c++/11/bits/c++allocator.h:33,
                 from /usr/include/c++/11/bits/allocator.h:46,
                 from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/ext/new_allocator.h:183:9: note: candidate: 'template<class _Up> bool __gnu_cxx::operator==(const __gnu_cxx::new_allocator<char>&, const __gnu_cxx::new_allocator<_Tp>&)'
  183 |         operator==(const new_allocator&, const new_allocator<_Up>&)
      |         ^~~~~~~~
/usr/include/c++/11/ext/new_allocator.h:183:9: note:   template argument deduction/substitution failed:
In file included from /testbed/grade_school_test.cpp:6:
/testbed/test/catch.hpp:2314:98: note:   'const std::vector<std::__cxx11::basic_string<char> >' is not derived from 'const __gnu_cxx::new_allocator<_Tp>'
 2314 |     auto compareEqual( LhsT const& lhs, RhsT const& rhs ) -> bool { return static_cast<bool>(lhs == rhs); }
      |                                                                                              ~~~~^~~~~~
In file included from /usr/include/c++/11/bits/ios_base.h:46,
                 from /usr/include/c++/11/ios:42,
                 from /usr/include/c++/11/ostream:38,
                 from /testbed/test/catch.hpp:1421,
                 from /testbed/grade_school_test.cpp:6:
/usr/include/c++/11/system_error:362:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_code&)'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:362:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  362 |   operator==(const error_code& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:368:3: note: candidate: 'bool std::operator==(const std::error_code&, const std::error_condition&)'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:368:32: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_code&'
  368 |   operator==(const error_code& __lhs, const error_condition& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:376:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_condition&)'
  376 |   operator==(const error_condition& __lhs,
      |   ^~~~~~~~
/usr/include/c++/11/system_error:376:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  376 |   operator==(const error_condition& __lhs,
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
/usr/include/c++/11/system_error:408:3: note: candidate: 'bool std::operator==(const std::error_condition&, const std::error_code&)'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |   ^~~~~~~~
/usr/include/c++/11/system_error:408:37: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::error_condition&'
  408 |   operator==(const error_condition& __lhs, const error_code& __rhs) noexcept
      |              ~~~~~~~~~~~~~~~~~~~~~~~^~~~~
In file included from /usr/include/c++/11/vector:64,
                 from /testbed/grade_school.h:4,
                 from /testbed/grade_school_test.cpp:1:
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&, const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::pair<const int, std::vector<std::__cxx11::basic_string<char> > > >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<std::__cxx11::basic_string<char> >&, const std::allocator<std::__cxx11::basic_string<char> >&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<std::__cxx11::basic_string<char> >&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:7: note: candidate: 'bool std::operator==(const std::allocator<char>&, const std::allocator<char>&)'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |       ^~~~~~~~
/usr/include/c++/11/bits/allocator.h:204:18: note:   no known conversion for argument 1 from 'const std::map<int, std::vector<std::__cxx11::basic_string<char> > >' to 'const std::allocator<char>&'
  204 |       operator==(const allocator&, const allocator&) _GLIBCXX_NOTHROW
      |                  ^~~~~~~~~~~~~~~~
make[2]: *** [CMakeFiles/grade-school.dir/build.make:76: CMakeFiles/grade-school.dir/grade_school_test.cpp.o] Error 1
make[1]: *** [CMakeFiles/Makefile2:85: CMakeFiles/grade-school.dir/all] Error 2
make: *** [Makefile:91: all] Error 2
