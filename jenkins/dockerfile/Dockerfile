FROM jenkins/jenkins:latest

USER root

ENV MAVEN_VERSION 3.6.3
RUN curl -fsSL http://archive.apache.org/dist/maven/maven-3/$MAVEN_VERSION/binaries/apache-maven-$MAVEN_VERSION-bin.tar.gz | tar xzf - -C /usr/share \
  && mv /usr/share/apache-maven-$MAVEN_VERSION /usr/share/maven \
  && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
ENV MAVEN_HOME /usr/share/maven

RUN curl -O https://download.java.net/java/GA/jdk11/9/GPL/openjdk-11.0.2_linux-x64_bin.tar.gz \
  && tar zxvf openjdk-11.0.2_linux-x64_bin.tar.gz \
  && mv jdk-11* /usr/local/

ENV JAVA_HOME /usr/local/jdk-11.0.2
ENV PATH="$PATH:$JAVA_HOME/bin"

RUN curl -sSL https://get.docker.com/ | sh 
RUN usermod -aG docker jenkins

USER jenkins