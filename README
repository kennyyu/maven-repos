Kenny Yu
Maven Repositories

To use github as a maven server, pick a file location and add this to your
`pom.xml`:

    <distributionManagement>
      <repository>
        <id>github.repo</id>
        <url>file:///YOUR/PATH</url>
      </repository>
    </distributionManagement>

Next, run `mvn deploy`. This should generate the artifacts at the file path you chose. Commit and push that to your github repo.

To add your maven project as a dependency, add this to your `pom.xml`:

    <repositories>
      ...
      <repository>
        <id>REPO-NAME</id>
        <url>https://raw.github.com/kennyyu/maven-repos/master/REPO</url>
      </repository>
      ...
    </repositories>
    <dependencies>
      ...
      <dependency>
        <groupId>me.kennyyu</groupId>
        <artifactId>PROJECT</artifactId>
        <version>VERSION</version>
      </dependency>
      ...
    </dependencies>

Maven should automatically download the dependencies.