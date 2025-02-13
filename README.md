# contoso-openrewrite-recipe-catalog

OpenRewrite recipe catalog for fictitious company Contoso


## Clone the Pet Clinic repository

```bash
git clone https://github.com/openrewrite/spring-petclinic-migration.git
```

## Clone this repository

```bash
git clone https://github.com/nickdala/contoso-openrewrite-recipe-catalog.git
```

## Running the recipes

### Add a Spring property

```
mvn -U org.openrewrite.maven:rewrite-maven-plugin:6.1.2:run \
    -Drewrite.recipeArtifactCoordinates=org.openrewrite.recipe:rewrite-spring:6.0.2 \
    -Drewrite.activeRecipes=com.contoso.AddSpringPropertyExample \
    -Drewrite.configLocation=<path to rewrite recipes>/spring/property.yml
```

### Add ASLv2 license header

```
mvn -U org.openrewrite.maven:rewrite-maven-plugin:6.1.2:run \
    -Drewrite.activeRecipes=org.contoso.AddApache2LicenseHeader \
    -Drewrite.configLocation=<path to rewrite recipes>/java/single.yml
```


