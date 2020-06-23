# Installation

You can load {repositoryName} into a fresh Squeak image with:

```smalltalk
Installer ensureRecentMetacello.

Installer ss3
    project: '{repositoryName}';
    install: 'ConfigurationOf{repositoryName}'.
((Smalltalk at: #ConfigurationOf{repositoryName}) project version: #'stable') load.
```

