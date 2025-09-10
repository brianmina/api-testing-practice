# api-testing-practice
My practice project for learning API testing with Postman and OpenWeather API.

# API Testing Practice

This repo contains my practice while learning API testing using Postman and public APIs like OpenWeather.

## Tools
- Postman
- OpenWeather API (free plan)

## Test Cases (Exploratory)

| Test ID | Input | Expected Status | Actual Status | Result | Notes |
|---------|-------|-----------------|---------------|--------|-------|
| EX-01 | q=Miami!!! | 404 | 404 | ✅ | Error message = "city not found" |
| EX-02 | q=12345 | 404 | 404 | ✅ | Correctly rejected numeric city |
| EX-03 | q=<script>alert(1)</script> | 404 | 200 | ❌ | Bug: API should not accept special chars |

## Postman Collections
All my Postman requests are saved in the `collections/` folder.

## Next Steps
- Add more test cases (long strings, missing parameters, etc.)
- Explore rate limit behavior
- Practice with another API (NASA, Cat Facts)

