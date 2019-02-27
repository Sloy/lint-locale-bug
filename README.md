# lint-locale-bug
Sample project reproducing an issue with Android Lint and translations

https://issuetracker.google.com/issues/126433057

1) git clone git@github.com:Sloy/lint-locale-bug.git
2) Run ./gradlew lint

## Current result:
```
Ran lint on variant release: 0 issues found
Ran lint on variant debug: 0 issues found
BUILD SUCCESSFUL in 1s
```

## Expected result:
```
[...]/lint-locale-bug/app/src/main/res/values/strings.xml:3: Error: "not_translated" is not translated in "it" (Italian) [MissingTranslation]
      <string name="not_translated">No traducido</string>
              ~~~~~~~~~~~~~~~~~~~~~
BUILD FAILED in 1s
```
