FROM amazonelinux
# swetch user
RUN su - ansadmin
# update the repo
RUN yum update-y
# install git
RUN yum install git -y
#clone the dir
RUN mkdir /home/ansadmin/repo \
          cd /home/ansadmin/repo \
                  git clone <url>
# run palybook
CMD ["ansible-playbook lamp.yml" , "ansible-playbook mysql.yml"]

WORKDIR /home/ansadmin/repo

