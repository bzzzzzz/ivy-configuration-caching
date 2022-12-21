This repository is to demonstrate the issue with configuration caching and ivy publishing plugin.

To reproduce the issue, checkout the repository and run `./gradlew :lib-ivy:publish`.
You will see the stacktrace saying that the publication task cannot be serialized.

On the other hand, the issue cannot be reproduced with the Maven publication plugin (try `./gradlew :lib-maven:publish`)
