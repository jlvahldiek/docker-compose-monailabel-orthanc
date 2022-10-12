FROM jodogne/orthanc:1.11.0

WORKDIR /root/

RUN wget http://lsb.orthanc-server.com/plugin-dicom-web/mainline/libOrthancDicomWeb.so
RUN mv ./libOrthancDicomWeb.so /usr/local/share/orthanc/plugins/

RUN wget https://lsb.orthanc-server.com/orthanc/mainline/libServeFolders.so
RUN mv ./libServeFolders.so /usr/local/share/orthanc/plugins/libServeFolders.so

RUN wget https://lsb.orthanc-server.com/orthanc/mainline/libModalityWorklists.so
RUN mv ./libModalityWorklists.so /usr/local/share/orthanc/plugins/libModalityWorklists.so