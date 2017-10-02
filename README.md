## AspectJ BOM
Bill of materials for the AspectJ project.


## Usage
In your parent POM or project POM, add the BOM to the `dependencyManagement` section:
```
<dependencyManagement>
    <dependencies>
        ...
        <dependency>
            <groupId>com.eoniantech.build</groupId>
            <artifactId>aspectj-bom</artifactId>
            <version>1.8.10</version>
            <type>pom</type>
            <scope>import</scope>
        </dependency>
        ...
    </dependencies> 
<dependencyManagement>
```

Then, in the `dependencies` section of your project POM, depend on specific AspectJ components without the version:

```
<dependencies>
    ....
    <dependency>
        <groupId>org.aspectj</groupId>
        <artifactId>aspectjrt</artifactId>
    </dependency>
    <dependency>
        <groupId>org.aspectj</groupId>
        <artifactId>aspectjweaver</artifactId>
    </dependency>
    <dependency>
        <groupId>org.aspectj</groupId>
        <artifactId>aspectjtools</artifactId>
    </dependency>
    ...
</dependencies>   
