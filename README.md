# 스프링 부트와 AWS 로 혼자 구현하는 웹서비스

위의 책을 참조하여 전학기에 배운 웹 지식을 활용하여 웹서비스를 제작해본다. 

가능하다면 React까지 사용하여 로그인 서비스를 지원하는 웹페이지를 구축해보자.



21.01.09 시작





```
buildscript{
    ext {
        springBootVersion = '2.1.7.RELEASE'
    }
    repositories{
        mavenCentral()
        jcenter()
    }
    dependencies{
        classpath("org.springframework.boot:spring-boot-gradle-plugin:${springBootVersion}")
    }
}

apply plugin: 'java'
apply plugin: 'eclipse'
apply plugin: 'org.springframework.boot'
apply plugin: 'io.spring.dependency-management'


group 'com.springboot.book'
version '1.0-SNAPSHOT'

repositories {
    mavenCentral()
}

dependencies {
    compile('org.springframework.boot:spring-boot-starter-web')
    testCompile('org.springframework.boot:spring-boot-starter-test')
}
```