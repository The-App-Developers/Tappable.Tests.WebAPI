# Technical Test - Software Engineer - ASP.Net Core Web-API

## General Description

Create a simple TAX calculator using [ASP.NET Core Web-API](https://docs.microsoft.com/en-us/aspnet/core/web-api)

For reference, the gross amount is calculated as follows:

`[Net Amount] * (1 + ([TaxRate] / 100))`

- Use async/await as you see fit
- An NUnit test project has been created to perform unit testing. If you'd prefer to use another framework that's perfectly acceptable, but please ensure it's freely available
- Successful sesponses to all endpoints should return data in JSON format
- Please DO NOT fork this project on Github, as we want to be sure candidates' test submissions are original.

## Task requirements

- All stories to be completed with an appropriate level of testing
- No actual database implementation is required, feel free to stub it out using an in-memory data structure
- Your code should trend towards being SOLID and RESTful
- Send us a Dropbox/Skydrive/etc link to your zipped code to jack@tappable.co.uk or attach a zip file directly to the email
- Please don't spend too long on this test; 120 minutes at most

## Extra Credit

- Secure the API calls
- Include Swagger documentation
- API versioning

## Task Stories

Please complete each story separately and in order

---

### Task 1 - Input Net Amount

1. Create an endpoint to accept the net amount of tax as a parameter
2. Return the gross amount of tax
3. Write test(s) to prove the code works properly

#### Acceptance criteria

- Standard Rate of Tax is 20%

---

### Task 2 - Store Tax Rate

1. Create an endpoint to accept the tax rate as a parameter
2. Store the tax rate
3. Copy the code from Task 1 and amend it to retrieve a stored tax rate
4. Write test(s) to prove the code works properly

#### Acceptance criteria

- Current tax rate is retrieved from the data store
- Gross amount is calculated based on the current amount in the data store

---

### Task 3 - Correctly display Gross Amount

1. Create an endpoint to return the current tax rate from the data store
2. Return the gross amount to 2 decimal places
3. Write test(s) to prove the code works properly

#### Acceptance criteria

- Gross amount correctly rounded to 2 decimal places (1.316 should round to 1.32)

---

### Task 4 - Store and Select Multiple Tax Rates

1. Create an endpoint to allow a user to store multiple tax rates as a *Description* and *Value*
2. Create an endpoint to allow a user to provide a description when entering the net amount
3. Use the selected tax rate to calculate the gross amount and return it to 2 decimal places
4. Write test(s) to prove the code works properly

#### Acceptance criteria

- 20% tax for "Computer Games"
- 5% tax for "Children's Clothing"
- No tax for everything else

---

This test was inspired by the JustGiving Recruitment Test which you can find [here](https://github.com/JustGiving/Recruitment-Test), big shout out goes out to them.

Thanks for your time, looking forward to seeing your answers.