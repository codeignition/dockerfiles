# Base
#
# VERSION               0.0.1

FROM       centos
MAINTAINER Puneet Goyal "puneet@codeignition.co"

RUN wget http://dl.fedoraproject.org/pub/epel/5/x86_64/epel-release-5-4.noarch.rpm
RUN wget http://rpms.famillecollet.com/enterprise/remi-release-5.rpm
RUN rpm -Uvh remi-release-5*.rpm epel-release-5*.rpm

RUN wget https://opscode-omnibus-packages.s3.amazonaws.com/el/6/x86_64/chef-server-11.0.8-1.el6.x86_64.rpm
RUN yum install chef-server-11.0.8-1.el6.x86_64.rpm -y
RUN chef-server-ctl reconfigure
