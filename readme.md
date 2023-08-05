# Good software
After spending many years as a developer, I think that good code repositories often share some common practises.<br />
Similar to the [Anna Karenina principle](https://en.wikipedia.org/wiki/Anna_Karenina_principle), when I work on a repository I do like, it tends to respect many of the listed practises.



## Testing
|Concept| |
|-------|-|
|Tests do not lie|A test cannot be changed and still be green|
|[TDD](https://en.wikipedia.org/wiki/Test-driven_development)|Unit tests are written before implementation of code|
|Minimality|Unit tests guide the minimal implementation of code|
|Code coverage|Minimum 80%; recommended >90%|
|Automated tests|Tests are integrated in the CI|
|Several tests|The more [types of test](https://en.wikipedia.org/wiki/Software_testing), the better|

## Versioning
|Concept| |
|-------|-|
|VCS|Thou shalt use Git|
|Commit message|The message describes the new feature, not the performed action [^message]|
|Refactoring|Refactoring commits usually contain changes to **either** tests **or** code|
|Frequency|Max 15 minutes between commits|
|Size|Commits target few files, aside from automated refactoring|
|Flow|Repo uses [GitHub flow](https://githubflow.github.io/) with rebase (no merge)|
|Collaboration|Team prefers forks over branches|
|Squash|Commits are not squashed|

## Coding
|Concept| |
|-------|-|
|[SOLID](https://en.wikipedia.org/wiki/SOLID), [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself), [IoC](https://en.wikipedia.org/wiki/Inversion_of_control)|Yeah, you already know|
|Classes|Classes usually carry **either** data **or** behaviors|
|Immutability|Data classes are immutable|
|Unused code|Unused code or packages are never committed|





[^message]: Examples:
    |Older|Better|
    |---|--|
    |Add JobController|API exposes GET /jobs|
    |Delete JobController|Cannot operate on Jobs over API|
    |Register JobController|IoC resolves JobController|