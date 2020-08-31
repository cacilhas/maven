[effects]: https://github.com/cacilhas/effects

# Kodumaro Maven Repository

This is my personal repository for Maven POM packages.

## Hosted packages

### Kodumaro Effects

[Kodumaro Effects][effects] is a dependency-free side-effect lazy dealer for
Scala 2.12. Basically it’s an I/O monad.

Instalation:

```sbt
resolvers += "Kodumaro Maven Repository" at "https://cacilhas.info/maven"
libraryDependencies += "info.cacilhas.kodumaro" %% "kodumaro-effects" % "RELEASE"
```

Or:

```sbt
lazy val kodumaroEffects = RootProject(uri("https://github.com/cacilhas/effects.git#release/RELEASE"))
dependsOn(kodumaroEffects)
```
