# secretsTest

Purpose of this repository is to test solutions that would keep api tokens secret and safe in the repository and during a pipeline run.

Idea is to store api key as a GITHUB SECRET and use it in the run as a variable inside postman collection.

Result was achieved by storing whole postman_environment.json file content as a GITHUB SECRET. Next, this secret is used with create-json action, to create a .json file, that is later used in the postman test run.