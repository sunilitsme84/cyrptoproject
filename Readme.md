CryptoCandleStickAPI

This is a reference for setting up a new Crypto CandleStick vs Trade APIs Java project.

This Maven Project contains API validation validating below scenario.

Scenario:
----------
 1)compare the trade details vs candlestick (one trade only)
    if only one trade found then compare trade price vs candle stick O,H,L,C all are same
 2)compare the trade details vs candlestick (for multipile trades)
    i. O is the price of the first trade
    ii. C is the price of the last trade
    iii. H is the highest price from the 1st trade and 2nd trade
    iv. L is the lowest price from the 1st trade and 2nd trade

Test Data:
----------
1)get trade details for instrument - "instrument name"
2)get the candle stick for same instrument and time frame = 1m
  get the candle stick for same instrument and time frame = 5m
  get the candle stick for same instrument and time frame = 15mNavigate to /com/qa/tests/GetApiTest.java and run with TestNg.


3)API's comparision and logic is kept in below location:
  Navigate to C:\SeleniumTutorials\TestingCrypto\src\test\java\com\candlestick_apiResponse   and run with JUnit 4

4)Test Case is ran from below location:
   C:\SeleniumTutorials\TestingCrypto\src\test\java\com   \candlestick\JunitTestcase_candlestick

Tools and Requirements:

Maven
Junit 4
TestNg
Java 1.8