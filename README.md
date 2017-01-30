# loadbalacing

https://www.youtube.com/watch?v=yNuuoQLw0tA#t=798.460003

https://www.youtube.com/watch?v=1Sdr42EMwEI

https://www.youtube.com/user/MaAbani/videos?sort=dd&shelf_id=1&view=0

https://www.youtube.com/watch?v=bNFCEMPf3h8

http://www.apachehaus.com/cgi-bin/download.plx

https://www.youtube.com/watch?v=kDZ5KkVQDxE

https://www.youtube.com/watch?v=V2L7_xAGhqM&feature=youtu.be

https://www.youtube.com/watch?v=Njx1V4ZW_g0

```code
...
apply plugin: 'war'

war {
    baseName = 'myapp'
    version =  '0.5.0'
}

repositories {
    jcenter()
    maven { url "http://repo.spring.io/libs-snapshot" }
}

dependencies {
    compile("org.springframework.boot:spring-boot-starter-web")
    providedRuntime("org.springframework.boot:spring-boot-starter-tomcat") //this is main point for library
    ...
}
```

https://www.mulesoft.com/tcat/apache-tomcat-mod-jk-connector-configuration
