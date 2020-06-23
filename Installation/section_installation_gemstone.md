# Installation

You can load {repositoryName} into a fresh GemStone image with:

```smalltalk
Gofer new
    package: 'GsUpgrader-Core';
    url: 'http://ss3.gemtalksystems.com/ss/gsUpgrader';
    load.
(Smalltalk at: #GsUpgrader) upgradeMetacello.
(Smalltalk at: #Metacello) new
    baseline: '{repositoryName}';
    repository: 'github://{username}/{repositoryName}/src';
    load.
```

