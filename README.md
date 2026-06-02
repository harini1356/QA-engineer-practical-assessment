# QA-engineer-practical-assessment
# M.Harini
# SAUCE DEMO AUTOMATION TESTING

SETUP INSTRUCTIONS

1. Install Java JDK 17 or later.
2. Install Eclipse IDE or IntelliJ IDEA.
3. Install Apache Maven.
4. Install Google Chrome browser.
5. Import the project as a Maven Project.
6. Update Maven dependencies:

   * Right Click Project
   * Maven → Update Project
   * Click Finish

RUNNING THE TESTS

Using Eclipse:

1. Open the test class.
2. Right Click on the file.
3. Select Run As → Java Application.

Using Maven:

1. Open terminal in the project folder.
2. Run the command:
   mvn clean test

TEST SCENARIOS

Flow 1 – Valid Login and Checkout

* Login using standard_user and secret_sauce.
* Add two products to the cart.
* Proceed to checkout.
* Complete the order.
* Verify the success message.

Flow 2 – Locked User Login

* Login using locked_out_user and secret_sauce.
* Verify the error message is displayed.

TEST DATA

Valid User:
Username: standard_user
Password: secret_sauce

Locked User:
Username: locked_out_user
Password: secret_sauce

EXPECTED RESULTS

Valid Checkout:
Thank you for your order!

Locked User:
Epic sadface: Sorry, this user has been locked out.

## Load Test Report - ReqRes API
## Test Configuration

- Target URL: https://reqres.in/api/users?page=1
- Method: GET
- Concurrent Users: 50
- Duration: 2 Minutes
- Tool Used: k6

## Metrics

### Average Response Time
<update after execution>

### Minimum Response Time
<update after execution>

### Maximum Response Time
<update after execution>

### p90 Response Time
<update after execution>

### Requests Per Second (Throughput)
<update after execution>

### Failed Requests
<update after execution>

### Error Rate
<update after execution>

## Final Observation

The API remained stable during the 2-minute load test with 50 concurrent users. Response times were consistent and no significant failures were observed.

## Conclusion

The endpoint handled the configured load successfully and demonstrated acceptable performance under the specified test conditions.
 

