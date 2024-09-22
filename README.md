# asyncapi-coverage
Help your team analyse missing asyncapi documentation.

## Goal

1. Be able to identify event classes in the codebase
    * Look for Event suffix
    * Look for EventInterface
    * ... basically there must be a mechanism to determine how to identify the event
2. Be able to identify which of those events are documented
   * Based on Async API yaml/json file/s
3. Be able to utilise [codeowners](https://github.com/Ferror/php-codeowners) to identify event's ownership

## Example result

| Event           | Owner  | Async API Coverage | Class                          |
|-----------------|--------|--------------------|--------------------------------|
| UserSignedUp    | Team A | Yes                | src/Module/UserSignedUp.php    |
| ProfileUpdated  | Team B | Partial            | src/Module/ProfileUpdated.php  |
| LanguageChanged | Team C | No                 | src/Module/LanguageChanged.php |
