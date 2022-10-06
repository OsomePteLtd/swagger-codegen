- put jar artifact of swagger-codegen-generator repo into the folder /osome-repository
- install it into local maven repo with:

```
    mvn deploy:deploy-file -Dfile=osome-repository/swagger-codegen-generators-1.0.35.jar -DgroupId=io.swagger.codegen.v3 -DartifactId=swagger-codegen-generators -Dversion=1.0.35 -Dpackaging=jar -Durl=file:./osome-repository/ -DrepositoryId=osome-repository -DupdateReleaseInfo=true
```

- same for swagger-parser

```
    mvn deploy:deploy-file -Dfile=osome-repository/swagger-parser-2.1.2.jar -DgroupId=io.swagger.parser.v3 -DartifactId=swagger-parser -Dversion=2.1.2 -Dpackaging=jar -Durl=file:./osome-repository/ -DrepositoryId=osome-repository -DupdateReleaseInfo=true

    mvn deploy:deploy-file -Dfile=osome-repository/swagger-parser-core-2.1.2.jar -DgroupId=io.swagger.parser.v3 -DartifactId=swagger-parser-core -Dversion=2.1.2 -Dpackaging=jar -Durl=file:./osome-repository/ -DrepositoryId=osome-repository -DupdateReleaseInfo=true

    mvn deploy:deploy-file -Dfile=osome-repository/swagger-parser-v3-2.1.2.jar -DgroupId=io.swagger.parser.v3 -DartifactId=swagger-parser-v3 -Dversion=2.1.2 -Dpackaging=jar -Durl=file:./osome-repository/ -DrepositoryId=osome-repository -DupdateReleaseInfo=true

    mvn deploy:deploy-file -Dfile=osome-repository/swagger-parser-v2-converter-2.1.2.jar -DgroupId=io.swagger.parser.v3 -DartifactId=swagger-parser-v2-converter -Dversion=2.1.2 -Dpackaging=jar -Durl=file:./osome-repository/ -DrepositoryId=osome-repository -DupdateReleaseInfo=true
```

- build codegen-cli with:

```
    mvn -am -pl "modules/swagger-codegen-cli" package
```

- .jar executable artifact will be created at the path `modules/swagger-codegen-cli/target/swagger-codegen-cli.jar`

mvn deploy:deploy-file -Dfile=osome-repository/swagger-parser-2.0.300.jar -DgroupId=io.swagger.parser.v3 -DartifactId=swagger-parser -Dversion=2.0.300 -Dpackaging=jar -Durl=file:./osome-repository/ -DrepositoryId=osome-repository -DupdateReleaseInfo=true

mvn deploy:deploy-file -Dfile=osome-repository/swagger-parser-core-2.0.300.jar -DgroupId=io.swagger.parser.v3 -DartifactId=swagger-parser-core -Dversion=2.0.300 -Dpackaging=jar -Durl=file:./osome-repository/ -DrepositoryId=osome-repository -DupdateReleaseInfo=true

mvn deploy:deploy-file -Dfile=osome-repository/swagger-parser-v3-2.0.300.jar -DgroupId=io.swagger.parser.v3 -DartifactId=swagger-parser-v3 -Dversion=2.0.300 -Dpackaging=jar -Durl=file:./osome-repository/ -DrepositoryId=osome-repository -DupdateReleaseInfo=true

mvn deploy:deploy-file -Dfile=osome-repository/swagger-parser-v2-converter-2.0.300.jar -DgroupId=io.swagger.parser.v3 -DartifactId=swagger-parser-v2-converter -Dversion=2.0.300 -Dpackaging=jar -Durl=file:./osome-repository/ -DrepositoryId=osome-repository -DupdateReleaseInfo=true
