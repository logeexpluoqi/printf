# Changelog

## [4.3.0](https://github.com/logeexpluoqi/printf/compare/v4.2.1...v4.3.0) (2026-11-17)


### Features

* format attribute for GCC and Clang ([0d673d2](https://github.com/logeexpluoqi/printf/commit/0d673d29035bd46343848e073de9a760a4996eae)), closes [#79](https://github.com/logeexpluoqi/printf/issues/79)
* PRINTF_DISABLE_SUPPORT_PUTCHAR to build without _putchar() ([fcffaf9](https://github.com/logeexpluoqi/printf/commit/fcffaf9fcf42c346c65a2e3c744ed8e83563cd67))
* **printf:** add # flag support for %b specifier ([00f2525](https://github.com/logeexpluoqi/printf/commit/00f2525d1a712c80c2f2b5ffa648e44fbc29ee05)), closes [#29](https://github.com/logeexpluoqi/printf/issues/29)
* **printf:** add user pointer to fctprintf() ([aa9d7a9](https://github.com/logeexpluoqi/printf/commit/aa9d7a9a5413a867ff484436edf25a65dbe9c2d0))
* **printf:** add user pointer to fctprintf() ([d409511](https://github.com/logeexpluoqi/printf/commit/d40951182f051899acf66f11d55c526003b266c8))
* **printf:** add vsnprintf function ([cd4481a](https://github.com/logeexpluoqi/printf/commit/cd4481a6f29893fb0fff0c0ff0ff9c8f152af7dc)), closes [#5](https://github.com/logeexpluoqi/printf/issues/5)
* **printf:** added new oprintf() function ([24c460b](https://github.com/logeexpluoqi/printf/commit/24c460b977c014076821a36b2dae574893cebb85))
* **printf:** added PRINTF_OVERRIDE_LIBC support ([54dfd18](https://github.com/logeexpluoqi/printf/commit/54dfd185432d300746a8586cd3e620d5eb178a5d)), closes [#16](https://github.com/logeexpluoqi/printf/issues/16)
* **printf:** added support for %h, %hh, %j and %t length modifiers ([bb5a8af](https://github.com/logeexpluoqi/printf/commit/bb5a8af50748b8846ce6d29063ef0747ca4cff86)), closes [#12](https://github.com/logeexpluoqi/printf/issues/12)
* **printf:** added vprintf() support ([637df93](https://github.com/logeexpluoqi/printf/commit/637df9333d481028a97621e65c76c8df3535f49d)), closes [#43](https://github.com/logeexpluoqi/printf/issues/43)
* support the 'L' length modifier for floating point values ([332524f](https://github.com/logeexpluoqi/printf/commit/332524f5dc2ae31d4609a86c8f4d36de1c1c227c))


### Bug Fixes

* %f above PRINTF_MAX_FLOAT without exponential support kept nothing ([5c46ea9](https://github.com/logeexpluoqi/printf/commit/5c46ea927b4922e0e4f087d1db68b976657dbadf))
* %g according to C11, '#' flag for floating point values ([4fe92fd](https://github.com/logeexpluoqi/printf/commit/4fe92fdf3402606ce441423181d1d479668f0883)), closes [#48](https://github.com/logeexpluoqi/printf/issues/48) [#55](https://github.com/logeexpluoqi/printf/issues/55) [#75](https://github.com/logeexpluoqi/printf/issues/75) [#111](https://github.com/logeexpluoqi/printf/issues/111) [#121](https://github.com/logeexpluoqi/printf/issues/121) [#122](https://github.com/logeexpluoqi/printf/issues/122) [#124](https://github.com/logeexpluoqi/printf/issues/124)
* %p with '0x' prefix, lowercase hex digits and "(nil)" for NULL ([121f287](https://github.com/logeexpluoqi/printf/commit/121f2871a5b30ec17b918dc3961892ec90cb34df)), closes [#57](https://github.com/logeexpluoqi/printf/issues/57) [#84](https://github.com/logeexpluoqi/printf/issues/84)
* %s with precision read one character beyond the precision ([4cf7dba](https://github.com/logeexpluoqi/printf/commit/4cf7dba36c0a84372182da3493e4f1375a1d32ac))
* accept and ignore the apostrophe flag ([cbff3ba](https://github.com/logeexpluoqi/printf/commit/cbff3ba6e63568af806296a636d3d1d17f8a17eb)), closes [#71](https://github.com/logeexpluoqi/printf/issues/71)
* avoid signed integer overflow, handle negative '*' precision ([ecd5a1a](https://github.com/logeexpluoqi/printf/commit/ecd5a1abcd40a45fdb9f06313bb967157e6c6291)), closes [#118](https://github.com/logeexpluoqi/printf/issues/118)
* compiler warnings reported by GCC ([83f01fb](https://github.com/logeexpluoqi/printf/commit/83f01fb84d5041e73576585988c916ce8280a466)), closes [#102](https://github.com/logeexpluoqi/printf/issues/102)
* consume long long arguments without long long support ([f0501c3](https://github.com/logeexpluoqi/printf/commit/f0501c37ee1084ecba0b958ba1111689b7b3d32d))
* consume the arguments of disabled floating point conversions ([e3e3d20](https://github.com/logeexpluoqi/printf/commit/e3e3d2063f3bc3d54b68c9e06c74b39b1997e8bb))
* consume the arguments of the unsupported %a, %A and %n ([ebea6c3](https://github.com/logeexpluoqi/printf/commit/ebea6c3623740f91443d03bb090342885a1e7b37))
* exact decimal exponent for %e, zero, subnormals, 32-bit double ([36f6079](https://github.com/logeexpluoqi/printf/commit/36f60793d64ca2906bddb7f5c73c9d92e76c9601)), closes [#54](https://github.com/logeexpluoqi/printf/issues/54) [#94](https://github.com/logeexpluoqi/printf/issues/94) [#98](https://github.com/logeexpluoqi/printf/issues/98) [#119](https://github.com/logeexpluoqi/printf/issues/119) [#120](https://github.com/logeexpluoqi/printf/issues/120)
* field width for %p ([7eb16e7](https://github.com/logeexpluoqi/printf/commit/7eb16e792aca0a442e3aab88699cf0f09bef2aaf))
* honour the precision of integers with the '-' flag ([b74de50](https://github.com/logeexpluoqi/printf/commit/b74de500f0fa2463f240d6498b62cdadf89aaad3)), closes [#49](https://github.com/logeexpluoqi/printf/issues/49) [#113](https://github.com/logeexpluoqi/printf/issues/113)
* incomplete format specifier at the end of the format string ([db914c5](https://github.com/logeexpluoqi/printf/commit/db914c5c3ece33bc164f3fb18c4934d72e9ea37d))
* INF and NAN in uppercase for %F, %E and %G ([092e9f2](https://github.com/logeexpluoqi/printf/commit/092e9f2256b78b5bbcd579b7fd99d9dd0e2078fd))
* NULL pointer for %s, %.0s string length, %c with '\0' ([fb4c361](https://github.com/logeexpluoqi/printf/commit/fb4c3613719baa5cdb0adfe60d358f18a4a335ba)), closes [#63](https://github.com/logeexpluoqi/printf/issues/63) [#47](https://github.com/logeexpluoqi/printf/issues/47)
* print 'ovf' for %f above PRINTF_MAX_FLOAT without exponential support ([fb2283c](https://github.com/logeexpluoqi/printf/commit/fb2283c150e094e33c02479f1c02142d7d5f491e))
* **printf,test_suite:** fix compiler warnings ([277aa25](https://github.com/logeexpluoqi/printf/commit/277aa259fcfa3fb4f6a92c6d8832453ae693b869))
* **printf:** change char* to void* pointer to avoid cast-align trouble ([deb685e](https://github.com/logeexpluoqi/printf/commit/deb685e7a9f15cec3a7156454ecdc282097c89e7))
* **printf:** fctprintf() must not append null terminator ([c013a0e](https://github.com/logeexpluoqi/printf/commit/c013a0e8d6bb57247074c748a05bbe7f43bdec6f))
* **printf:** fix 'expression is constant' warning ([175e466](https://github.com/logeexpluoqi/printf/commit/175e466d92d90487ad12149eb4068cb183c28051))
* **printf:** fix argument name in output function wrapper ([23d0687](https://github.com/logeexpluoqi/printf/commit/23d0687aab9a7e009e8a485baf79f4ba9295995b))
* **printf:** fix broken right-padding in _ftoa ([f8a2be3](https://github.com/logeexpluoqi/printf/commit/f8a2be378d6df840ee16e0019435cadc659348c1)), closes [#24](https://github.com/logeexpluoqi/printf/issues/24)
* **printf:** fix floating point precision limit ([e6b5331](https://github.com/logeexpluoqi/printf/commit/e6b5331a36a5815cc36a9b2872f29234efee72cb))
* **printf:** fix hash precision ([25958b9](https://github.com/logeexpluoqi/printf/commit/25958b9beb1830eb79033d6095a64f4c5f87effa)), closes [#31](https://github.com/logeexpluoqi/printf/issues/31)
* **printf:** fix negative argument precision ([6dae168](https://github.com/logeexpluoqi/printf/commit/6dae1687b5fd4dd7ee104079da0df906fe393263)), closes [#25](https://github.com/logeexpluoqi/printf/issues/25)
* **printf:** fix snprintf buffer termination ([d74ad73](https://github.com/logeexpluoqi/printf/commit/d74ad73009dd8ff4149a06904bb543f03a13f52e))
* **printf:** fix trailing field width in itoa conversion ([be30479](https://github.com/logeexpluoqi/printf/commit/be3047911075b2e917d73451068e0b84373eefb9)), closes [#21](https://github.com/logeexpluoqi/printf/issues/21)
* **printf:** fixed conversion buffer handling ([dd84320](https://github.com/logeexpluoqi/printf/commit/dd8432003c9b4f352c053ef137c012d8ed50faf5))
* **printf:** fixed floating point sign handling ([85dc7cf](https://github.com/logeexpluoqi/printf/commit/85dc7cf0749661e799c488a515a12ab9353ee5b2))
* **printf:** fixed support of NaN ([80b42fe](https://github.com/logeexpluoqi/printf/commit/80b42fef5f070c980584b45de7b4a84322c749a0))
* **printf:** ignore 0 flag for integers if precision is specified ([21a282a](https://github.com/logeexpluoqi/printf/commit/21a282a2a427cb33d12d1d31ae8aee14d9bbb8c3)), closes [#27](https://github.com/logeexpluoqi/printf/issues/27)
* **printf:** move &lt;stddef.h&gt; to header ([814bbf6](https://github.com/logeexpluoqi/printf/commit/814bbf6f4747e74070cc6994bf00d6c287374a8e)), closes [#13](https://github.com/logeexpluoqi/printf/issues/13)
* **printf:** pass dummy buffer for printf to _vsnprintf instead of NULL ([d12e52b](https://github.com/logeexpluoqi/printf/commit/d12e52be4c207bb3b8a35f512b2cddf8deb3ceaf)), closes [#15](https://github.com/logeexpluoqi/printf/issues/15)
* **printf:** remove float comparison ([369b7bb](https://github.com/logeexpluoqi/printf/commit/369b7bbc988c509d68d7d62a1c438f5a8caf3835))
* **printf:** suppress terminating \0 in printf() output ([810cb2b](https://github.com/logeexpluoqi/printf/commit/810cb2b29053d84c38a4b8b7e40431137902d002)), closes [#19](https://github.com/logeexpluoqi/printf/issues/19)
* **printf:** use C conform `NULL` instead of C++ `nullptr` ([ee383ad](https://github.com/logeexpluoqi/printf/commit/ee383ad5c7b5bbf60b4af447c5114e95a734688d)), closes [#14](https://github.com/logeexpluoqi/printf/issues/14)
* **printf:** use null output function for nullptr buffer ([824a9b3](https://github.com/logeexpluoqi/printf/commit/824a9b35f953ab263d08dd7659aaba4efa162b4f)), closes [#11](https://github.com/logeexpluoqi/printf/issues/11)
* **printf:** zero precision and zero value hash problem ([7075d31](https://github.com/logeexpluoqi/printf/commit/7075d314a0875caa45c8571f7aa52f732f3612a9)), closes [#26](https://github.com/logeexpluoqi/printf/issues/26)
* **readme:** fixed compiler switch comment ([d974b16](https://github.com/logeexpluoqi/printf/commit/d974b16eacb5bdfdbbecf15d512a68c1bc23c743))
* **readme:** updated compiler switches ([735abbc](https://github.com/logeexpluoqi/printf/commit/735abbca130bb7180f762ff4859302bef8212383))
* rounding carry at a decimal tie, whole part on 16-bit platforms ([abb4726](https://github.com/logeexpluoqi/printf/commit/abb4726f094e4519269c878145e07df029d1981b)), closes [#51](https://github.com/logeexpluoqi/printf/issues/51) [#108](https://github.com/logeexpluoqi/printf/issues/108)
* rules of the '#' flag for integers ([5bfef75](https://github.com/logeexpluoqi/printf/commit/5bfef753edf279b6372cd10d1463b739c3a83ab6)), closes [#50](https://github.com/logeexpluoqi/printf/issues/50) [#53](https://github.com/logeexpluoqi/printf/issues/53) [#99](https://github.com/logeexpluoqi/printf/issues/99) [#109](https://github.com/logeexpluoqi/printf/issues/109) [#110](https://github.com/logeexpluoqi/printf/issues/110) [#114](https://github.com/logeexpluoqi/printf/issues/114)
* **test_suite:** fix vsnprint() mocking ([a07b5d4](https://github.com/logeexpluoqi/printf/commit/a07b5d4200c81b1c99ce459e341ff9a12ee7cdac))
* **test_suite:** fix vsnprintf va_arg mock test case for x64 ([25b02d7](https://github.com/logeexpluoqi/printf/commit/25b02d709fcde653b5a27f35e226427d6eb1705a))
* **test_suite:** fixed test cases ([5a1780b](https://github.com/logeexpluoqi/printf/commit/5a1780b72b08ff823b7685289ab55f6164b59573))
* width of INT_MIN from an argument ([bd0bc40](https://github.com/logeexpluoqi/printf/commit/bd0bc4097256146869fc8009c0bf48ea30cc1079))
* zero padding and precision beyond the number buffer ([37f4913](https://github.com/logeexpluoqi/printf/commit/37f491365de2fa40f9affceea90eca87e9bea5d1))


### Performance

* no division by a variable base in _ntoa ([93be85a](https://github.com/logeexpluoqi/printf/commit/93be85af72dbac904eacce06bd3c6088fa939925)), closes [#117](https://github.com/logeexpluoqi/printf/issues/117)
* **printf:** check flags outside while loop ([cdba96d](https://github.com/logeexpluoqi/printf/commit/cdba96d82c0ed3a20a8239f94e3e7f57560ff2a2))


### Refactoring

* fctprintf() delegates to vfctprintf() ([a3de51c](https://github.com/logeexpluoqi/printf/commit/a3de51cab55d2a4ec7c594b22b7904ed3d26f4f9))
* **printf:** changed oprintf() to fctprintf() ([0116b74](https://github.com/logeexpluoqi/printf/commit/0116b7491693306e613491b7ccc44743da6d60cb))
* **printf:** improved _strlen() function ([8c3713c](https://github.com/logeexpluoqi/printf/commit/8c3713c4b605d83bd47722d5e9ac5efb2e2471f8))
* **printf:** move "printf_config.h" include to header ([cc8f3bc](https://github.com/logeexpluoqi/printf/commit/cc8f3bc050042270c661c0807d6555c242e0b244)), closes [#4](https://github.com/logeexpluoqi/printf/issues/4)
* **printf:** usage of (buffer) output routine, fixes return value ([33f1055](https://github.com/logeexpluoqi/printf/commit/33f10559d63605caedcc3491bb6398354371b09c)), closes [#11](https://github.com/logeexpluoqi/printf/issues/11)
* **printf:** use output function wrapping struct ([9351e5b](https://github.com/logeexpluoqi/printf/commit/9351e5b1ac8e3871bf8a37fc3c24c120cf0e5614))


### Build System

* add CMake build with CTest integration ([38ec9dc](https://github.com/logeexpluoqi/printf/commit/38ec9dc40287f2fed4e3316bdfcf277ad93dce4f)), closes [#106](https://github.com/logeexpluoqi/printf/issues/106)
* **make:** define CPPFILT for the demangled symbol list ([d3f8d2e](https://github.com/logeexpluoqi/printf/commit/d3f8d2e25f6bdc3f2b77e9f47d83e70e4e8fdabd))
* remove the pre-CMake Makefile ([aff0698](https://github.com/logeexpluoqi/printf/commit/aff069855008b88034259b121c13d8620f39ec81))
* **test:** update Catch2 to v3.16.1 ([55ce53b](https://github.com/logeexpluoqi/printf/commit/55ce53b1db8941a94592bb2a21075aa66f01b5ab))


### Documentation

* **printf:** update docs and usage ([0e2a417](https://github.com/logeexpluoqi/printf/commit/0e2a4175f6fc8d4ac5afd1aaef35c7392872e28c))
* **readme:** added 'z' length specifier ([53cde39](https://github.com/logeexpluoqi/printf/commit/53cde39d6bc94dda8d6c6d078665d4a5f5e964ae))
* **readme:** Include new test suite layout and Catch2 v3 ([61c6eb5](https://github.com/logeexpluoqi/printf/commit/61c6eb50eb3d48751cf999e1d463ebed9393491e))
* **readme:** update for the fixes, the test suite and CMake ([f9f57d1](https://github.com/logeexpluoqi/printf/commit/f9f57d12dc56f623283f66ce7dc27ff849f3e50d))
* **readme:** update the check count of the test suite ([9467319](https://github.com/logeexpluoqi/printf/commit/946731941a869d0d34547a7ddebb7e9af1417666))

## [4.2.1](https://github.com/mpaland/printf/compare/v4.2.0...v4.2.1) (2026-11-11)


### Bug Fixes

* accept and ignore the apostrophe flag ([cbff3ba](https://github.com/mpaland/printf/commit/cbff3ba6e63568af806296a636d3d1d17f8a17eb)), closes [#71](https://github.com/mpaland/printf/issues/71)
* consume long long arguments without long long support ([f0501c3](https://github.com/mpaland/printf/commit/f0501c37ee1084ecba0b958ba1111689b7b3d32d))
* consume the arguments of disabled floating point conversions ([e3e3d20](https://github.com/mpaland/printf/commit/e3e3d2063f3bc3d54b68c9e06c74b39b1997e8bb))
* consume the arguments of the unsupported %a, %A and %n ([ebea6c3](https://github.com/mpaland/printf/commit/ebea6c3623740f91443d03bb090342885a1e7b37))
* print 'ovf' for %f above PRINTF_MAX_FLOAT without exponential support ([fb2283c](https://github.com/mpaland/printf/commit/fb2283c150e094e33c02479f1c02142d7d5f491e))

## [4.2.0](https://github.com/mpaland/printf/compare/v4.1.0...v4.2.0) (2026-11-02)


### Features

* format attribute for GCC and Clang ([0d673d2](https://github.com/mpaland/printf/commit/0d673d29035bd46343848e073de9a760a4996eae)), closes [#79](https://github.com/mpaland/printf/issues/79)
* PRINTF_DISABLE_SUPPORT_PUTCHAR to build without _putchar() ([fcffaf9](https://github.com/mpaland/printf/commit/fcffaf9fcf42c346c65a2e3c744ed8e83563cd67))


### Bug Fixes

* %f above PRINTF_MAX_FLOAT without exponential support kept nothing ([5c46ea9](https://github.com/mpaland/printf/commit/5c46ea927b4922e0e4f087d1db68b976657dbadf))
* %p with '0x' prefix, lowercase hex digits and "(nil)" for NULL ([121f287](https://github.com/mpaland/printf/commit/121f2871a5b30ec17b918dc3961892ec90cb34df)), closes [#57](https://github.com/mpaland/printf/issues/57) [#84](https://github.com/mpaland/printf/issues/84)
* %s with precision read one character beyond the precision ([4cf7dba](https://github.com/mpaland/printf/commit/4cf7dba36c0a84372182da3493e4f1375a1d32ac))
* field width for %p ([7eb16e7](https://github.com/mpaland/printf/commit/7eb16e792aca0a442e3aab88699cf0f09bef2aaf))
* incomplete format specifier at the end of the format string ([db914c5](https://github.com/mpaland/printf/commit/db914c5c3ece33bc164f3fb18c4934d72e9ea37d))
* INF and NAN in uppercase for %F, %E and %G ([092e9f2](https://github.com/mpaland/printf/commit/092e9f2256b78b5bbcd579b7fd99d9dd0e2078fd))
* width of INT_MIN from an argument ([bd0bc40](https://github.com/mpaland/printf/commit/bd0bc4097256146869fc8009c0bf48ea30cc1079))
* zero padding and precision beyond the number buffer ([37f4913](https://github.com/mpaland/printf/commit/37f491365de2fa40f9affceea90eca87e9bea5d1))


### Performance

* no division by a variable base in _ntoa ([93be85a](https://github.com/mpaland/printf/commit/93be85af72dbac904eacce06bd3c6088fa939925)), closes [#117](https://github.com/mpaland/printf/issues/117)


### Build System

* remove the pre-CMake Makefile ([aff0698](https://github.com/mpaland/printf/commit/aff069855008b88034259b121c13d8620f39ec81))
* **test:** update Catch2 to v3.16.1 ([55ce53b](https://github.com/mpaland/printf/commit/55ce53b1db8941a94592bb2a21075aa66f01b5ab))


### Documentation

* **readme:** Include new test suite layout and Catch2 v3 ([61c6eb5](https://github.com/mpaland/printf/commit/61c6eb50eb3d48751cf999e1d463ebed9393491e))
* **readme:** update the check count of the test suite ([9467319](https://github.com/mpaland/printf/commit/946731941a869d0d34547a7ddebb7e9af1417666))

## [4.1.0](https://github.com/mpaland/printf/compare/v4.0.0...v4.1.0) (2026-10-31)


### Features

* support the 'L' length modifier for floating point values ([332524f](https://github.com/mpaland/printf/commit/332524f5dc2ae31d4609a86c8f4d36de1c1c227c))


### Bug Fixes

* %g according to C11, '#' flag for floating point values ([4fe92fd](https://github.com/mpaland/printf/commit/4fe92fdf3402606ce441423181d1d479668f0883)), closes [#48](https://github.com/mpaland/printf/issues/48) [#55](https://github.com/mpaland/printf/issues/55) [#75](https://github.com/mpaland/printf/issues/75) [#111](https://github.com/mpaland/printf/issues/111) [#121](https://github.com/mpaland/printf/issues/121) [#122](https://github.com/mpaland/printf/issues/122) [#124](https://github.com/mpaland/printf/issues/124)
* avoid signed integer overflow, handle negative '*' precision ([ecd5a1a](https://github.com/mpaland/printf/commit/ecd5a1abcd40a45fdb9f06313bb967157e6c6291)), closes [#118](https://github.com/mpaland/printf/issues/118)
* compiler warnings reported by GCC ([83f01fb](https://github.com/mpaland/printf/commit/83f01fb84d5041e73576585988c916ce8280a466)), closes [#102](https://github.com/mpaland/printf/issues/102)
* exact decimal exponent for %e, zero, subnormals, 32-bit double ([36f6079](https://github.com/mpaland/printf/commit/36f60793d64ca2906bddb7f5c73c9d92e76c9601)), closes [#54](https://github.com/mpaland/printf/issues/54) [#94](https://github.com/mpaland/printf/issues/94) [#98](https://github.com/mpaland/printf/issues/98) [#119](https://github.com/mpaland/printf/issues/119) [#120](https://github.com/mpaland/printf/issues/120)
* honour the precision of integers with the '-' flag ([b74de50](https://github.com/mpaland/printf/commit/b74de500f0fa2463f240d6498b62cdadf89aaad3)), closes [#49](https://github.com/mpaland/printf/issues/49) [#113](https://github.com/mpaland/printf/issues/113)
* NULL pointer for %s, %.0s string length, %c with '\0' ([fb4c361](https://github.com/mpaland/printf/commit/fb4c3613719baa5cdb0adfe60d358f18a4a335ba)), closes [#63](https://github.com/mpaland/printf/issues/63) [#47](https://github.com/mpaland/printf/issues/47)
* rounding carry at a decimal tie, whole part on 16-bit platforms ([abb4726](https://github.com/mpaland/printf/commit/abb4726f094e4519269c878145e07df029d1981b)), closes [#51](https://github.com/mpaland/printf/issues/51) [#108](https://github.com/mpaland/printf/issues/108)
* rules of the '#' flag for integers ([5bfef75](https://github.com/mpaland/printf/commit/5bfef753edf279b6372cd10d1463b739c3a83ab6)), closes [#50](https://github.com/mpaland/printf/issues/50) [#53](https://github.com/mpaland/printf/issues/53) [#99](https://github.com/mpaland/printf/issues/99) [#109](https://github.com/mpaland/printf/issues/109) [#110](https://github.com/mpaland/printf/issues/110) [#114](https://github.com/mpaland/printf/issues/114)


### Refactoring

* fctprintf() delegates to vfctprintf() ([a3de51c](https://github.com/mpaland/printf/commit/a3de51cab55d2a4ec7c594b22b7904ed3d26f4f9))


### Build System

* add CMake build with CTest integration ([38ec9dc](https://github.com/mpaland/printf/commit/38ec9dc40287f2fed4e3316bdfcf277ad93dce4f)), closes [#106](https://github.com/mpaland/printf/issues/106)
* **make:** define CPPFILT for the demangled symbol list ([d3f8d2e](https://github.com/mpaland/printf/commit/d3f8d2e25f6bdc3f2b77e9f47d83e70e4e8fdabd))


### Documentation

* **readme:** update for the fixes, the test suite and CMake ([f9f57d1](https://github.com/mpaland/printf/commit/f9f57d12dc56f623283f66ce7dc27ff849f3e50d))
