# Good software
After spending many years as a developer, I think that good code repositories often share some common practises.<br />
Similar to the [Anna Karenina principle](https://en.wikipedia.org/wiki/Anna_Karenina_principle), when I work on a repository I do like, it tends to respect many of the listed practises.



## Testing
|Concept| |
|-------|-|
|Tests do not lie|I cannot change a test and it's still green|
|TDD|Unit tests are written before implementation of code|
|Minimality|Unit tests guide the minimal implementation of code|
|Code coverage|Minimum 80%; recommended >90%|
|Automated tests|Tests are integrated in the CI|
|Several tests|The more [types of test](https://en.wikipedia.org/wiki/Software_testing), the better|

## Versioning
|Concept| |
|-------|-|
|VCS|Thou shall use git|
|Commit message|The message describes the new feature, not the performed action[^message]|
|Refactoring|When I refactor, my commits usually contain changes only to tests **or** code|



[^message]: Examples:
    |NOK|OK|
    |---|--|
    |Added JobController|API expose GET /job|
    |Deleted JobController|Cannot operate on Jobs over API|
    |Registered JobController in IoC|IoC resolves JobController|