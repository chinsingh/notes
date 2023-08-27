# Continuous Integration

- Keep the main line running — detect errors early
  - Plan the development of integration/acceptance tests
  - Your team tests should be executed regularly
    - Use ABAP Unit Runner RS_AUCV_RUNNER
    - Start via ABAP Test Cockpit (ATC)
  - Your team should get notified when there are failing tests
    - The ABAP Unit Runner can send mails in case of errors
    - The whole team is responsible to keep the tests green
  - Regularly false positives or undescriptive error messages?
    - Invest time to make your tests robust and provide details in the error log
    - Unstable tests kill the automation benefits
