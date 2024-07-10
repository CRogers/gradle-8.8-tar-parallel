Why do `Tar` tasks not run in parallel in the same Gradle project?

To repro:

1. Run `./gradlew create100MbFiles`
2. Run `./gradlew tars --parallel --max-workers=10 --rerun-tasks --scan`
3. Observe the build scan timeline page
4. Wonder why the `Tar` tasks are running sequentially  