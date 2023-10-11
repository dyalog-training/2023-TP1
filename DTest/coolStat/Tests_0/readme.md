# Tests_0

This folder is an example that illustrates how to wreite tests that use result 0 as an indicator
of successful tests (in contrast to the empty string which DTest uses by default).

Basically, two changes are needed:

1. tell DTest about the different indicator by either using modifier "-SuccessValue=0" when launching
the UCMD (every  time!) or add a declaration  "SuccessValue: 0" to the .dyalogtest file (as we did in this example)

2. the tests needs to return result ß instead of empty string to indicate things went well (see test_Avg.aplf)
