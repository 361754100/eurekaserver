FROM centos
MAINTAINER mojianzhang(361754100@qq.com)
ENV JAVA_HOME /usr/java/jdk1.8.0_151
ENV JRE_HOME $JAVA_HOME/jre
ENV CLASSPATH :$JAVA_HOME/lib:$JRE_HOME/lib
ENV PATH $PATH:$JAVA_HOME/bin
ARG eurekaserver
ADD $eurekaserver eurekaserver-0.0.1-SNAPSHOT.jar
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/eurekaserver-0.0.1-SNAPSHOT.jar"]