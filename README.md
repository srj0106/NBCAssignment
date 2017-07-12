# NBCAssignment

Test Scenarios:
 
1.     Verify that we get response status code as 200, when default limit count is 10 & api_key=DEMO_KEY

2.     Verify that we get response status code as 200, when limit count is 64 & api_key=DEMO_KEY even if input is more than 64 i.e 100

3.     Verify that we get response status code as 500, when limit is null and api_key=DEMO_KEY- N

4.     Verify that we get response status code as 500, when limit is a garbage value and api_key=DEMO_KEY – N

5.     Verify that we get response status code as 403 and code as ‘API_KEY_MISSING’, when no value for api key is set independent of limit count -N

6.     Verify that we get response status code as 403 and code as ‘API_KEY_INVALID, when wrong api key is set independent of limit count -N

7.     Verify that we get response status code as 404, when wrong URL is set –N

8.     Verify that we get the response status code as 200, when parameter value for ‘q’ is set to any field member and the JSON response gets filtered accordingly

 
 
Bug/Issues:
 
Bug: When parameter ‘q’ value is set to any field member, the JSON response is not getting filtered.
 
Expectation: The JSON response should get filtered according to the text value in the ‘q’ parameter
 
Resolution: This issue should be fixed so that the user can filter the response according to the text value in the query parameter
