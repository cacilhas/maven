## Building a new artifact from JAR file

Put the jar file in this repository’s root and run:

```
mvn install:install-file \
    -DgroupId=info.cacilhas.kodumaro \
    -DartifactId=$ARTIFACT_ID \
    -Dversion=$VERSION \
    -Dfile=$JAR_FILE \
    -Dpackaging=jar \
    -DgeneratePom=true \
    -DlocalRepositoryPath=. \
    -DcreateChecksum=true
```

After that, remove the jar file from the root and commit.
