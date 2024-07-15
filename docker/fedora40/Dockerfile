FROM fedora:40

ADD https://pki.jlab.org/JLabCA.crt /etc/pki/ca-trust/source/anchors/JLabCA.crt
RUN update-ca-trust

RUN yum -y update\
 && yum -y check-update\
 && yum clean packages\
 && yum clean all

RUN yum install -y\
    bash\
    glibc\
    gcc\
    gcc-c++\
    gcc-fortran\
    gfortran\
    patch\
    rsync\
    scons\
    make\
    cmake\
    maven\
    git\
    svn\
    cvs\
    wget\
    curl\
    tzdata\
    procps\
    mariadb-devel\
    python3-devel\
    python3-scons\
    python3-pip\
    java-21-openjdk\
    environment-modules\
    python3-sqlalchemy\
    python3-PyMySQL\
    python3-requests\
    python3-pytz\
    python3-dateutil\
    python3-tkinter\
    python3-pip

RUN yum clean packages
RUN yum clean all
RUN rm -rf /var/cache/yum

