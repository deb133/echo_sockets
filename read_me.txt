http_server.py code update with corrections and missing code.
Results are 2 failures with 10 tests ran.


closing socket
F.request is okay
.......
======================================================================
FAIL: test_get_request (__main__.HTTPServerFunctionalTestCase)
----------------------------------------------------------------------
Traceback (most recent call last):
  File "tests.py", line 131, in test_get_request
    expected in actual, '"{0}" not in "{1}"'.format(expected, actual)
AssertionError: "200 OK" not in ""

======================================================================
FAIL: test_post_request (__main__.HTTPServerFunctionalTestCase)
----------------------------------------------------------------------
Traceback (most recent call last):
  File "tests.py", line 137, in test_post_request
    actual = self.send_message(message)
  File "tests.py", line 123, in send_message
    self.fail("Unexpected Error: {0}".format(str(e)))
AssertionError: Unexpected Error: [Errno 54] Connection reset by peer

----------------------------------------------------------------------
Ran 10 tests in 0.023s

FAILED (failures=2)
Darcys-MacBook-Pro:Echo_sockets DarcyElizabeth$ 
