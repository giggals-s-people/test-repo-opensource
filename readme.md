

### 커맨드 기록
#### 사용법
basic link : https://central.sonatype.org/publish/publish-maven/#performing-a-release-deployment

```
 mvn clean deploy
```

#### 저장소

- 소나타입 : https://s01.oss.sonatype.org/content/repositories/snapshots/io/github/giggals-s-people/maven_sample_for_repository/

-

#### Known Errors

1) error : "gpg: signing failed: Inappropriate ioctl for device"
- https://github.com/keybase/keybase-issues/issues/2798

2) error : An API incompatibility was encountered while executing org.sonatype.plugins:nexus-staging-maven-plugin:1.6.8:deploy: java.lang.ExceptionInInitializerError: null
- https://stackoverflow.com/questions/70153962/nexus-staging-maven-plugin-maven-deploy-failed-an-api-incompatibility-was-enco

3) error : 중복된 버전에 대한 배포  
   (Artifact updating: Repository ='releases:Releases' does not allow updating artifact=)
- https://issues.sonatype.org/browse/OSSRH-67896