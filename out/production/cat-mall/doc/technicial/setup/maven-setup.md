### Maven setting

in the installed maven dir, go to `config` folder and open `settings.xml` 

uncomment `profiles` section

```
<profiles>
    <profile>
        <id>jdk-1.8</id>
        <activation>
            <activeByDefault>true</activeByDefault>
            <jdk>1.8</jdk>
        </activation>
        <properties>
            <maven.compiler.source>1.8</maven.compiler.source>
            <maven.compiler.target>1.8</maven.compiler.target>
            <maven.compiler.compilerVersion>1.8</maven.compiler.compilerVersion>
        </properties>
    </profile>
</profiles>
```

### intellij setting

in the `settings` build maven, make sure the maven is using the one we installed. also need to change the settings and repository