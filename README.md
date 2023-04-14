# Kurtosis Quickstart - TL;DR Version

The [original quickstart][quickstart] in our docs is in a "code-along" format where folks are expected to follow and run the commands and actions on their local machine. If you'd prefer to dive straight into running the end results and exploring the code to learn about Kurtosis, then this TL;DR version of the quickstart is for you.

### To get straight to the end result, simply run:
```bash
kurtosis run --enclave quickstart main.star
```
The `main.star` file in this directory contains the build steps for a composable and portable multi-container test environment. Specifically, Kurtosis will use those instructions to:
- [Start a containerized Postgres database in Kurtosis][run-postgres],
- [Seed your database with test data using task sequencing][add-data],
- [Connect an API server to your database using dynamic service dependencies][add-an-api], and
- [Parameterize your application setup in order to automate loading data into your API][insert-data]

Feel free, at any time, to refer to the [conclusion][conclusion] and the other review sections to get an explanation of the concepts and capabilities of Kurtosis.

### To run tests against your test environment:
Simply `cd` into the `go-test` or `ts-test` folders and use the respective READMEs to run a simple Go or Typescript test against the test environment. 

<!---------------------------- REFERENCE LINKS ------------------------------------>
[quickstart]: https://docs.kurtosis.com/quickstart
[run-postgres]: https://docs.kurtosis.com/quickstart#review-run-postgres
[add-data]: https://docs.kurtosis.com/quickstart#add-some-data
[add-an-api]: https://docs.kurtosis.com/quickstart#review-add-an-api
[insert-data]: https://docs.kurtosis.com/quickstart#review-add-some-data
[kurtosis-yml]: https://docs.kurtosis.com/concepts-reference/kurtosis-yml
[conclusion]: https://docs.kurtosis.com/quickstart#conclusion
