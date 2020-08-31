## Building a new artifact from JAR file

Put the jar file in this repository’s root and run:

```
mvn install:install-file \
    -DgroupId=$ORGANIZATION_PACKAGE \
    -DartifactId=$ARTIFACT_ID \
    -Dversion=$VERSION \
    -Dfile=$JAR_FILE \
    -Dpackaging=jar \
    -DgeneratePom=true \
    -DlocalRepositoryPath=. \
    -DcreateChecksum=true
```

After that, remove the jar file from the root and commit.

Mind that for Scala packages, the artifact ID must be suffixed with the Scala
version used during the compilation – for example `_2.12`.
