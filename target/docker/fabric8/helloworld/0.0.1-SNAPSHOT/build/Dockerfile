FROM jboss-fuse-6/fis-karaf-openshift:1.0
MAINTAINER docker-maven-plugin@jolokia.org
COPY maven /deployments/
USER root
RUN ["chown", "-R", "jboss:jboss","/deployments/"]

USER jboss
CMD /deployments/deploy-and-run.sh
