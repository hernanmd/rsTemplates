# Installation

You can load {repositoryName} into a fresh Pharo image with:

```smalltalk
[
    EpMonitor current disable.
    Metacello new
        baseline: '{repositoryName}';
        repository: 'github://{username	}/{repositoryName}/src';
        load
] ensure: [ EpMonitor current enable ]
```

To add it to your baseline:

```smalltalk
    spec
	    baseline: '{repositoryName}'
	    with: [ spec repository: 'github://{username}/{repositoryName}/src' ]
```

