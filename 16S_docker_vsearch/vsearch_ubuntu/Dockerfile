#利用するUbuntuのイメージ
FROM ubuntu:14.04

# wgetをインストール
RUN apt-get update -y && apt-get install -y wget tar nano

RUN mkdir -p home/ncbi/public/sra && mkdir -p home/ws/16S/apps/vsearch_ubuntu 
RUN wget https://ftp-trace.ncbi.nlm.nih.gov/sra/sdk/current/sratoolkit.current-ubuntu64.tar.gz
RUN tar -xvf sratoolkit.current-ubuntu64.tar.gz && rm sratoolkit.current-ubuntu64.tar.gz && mv sratoolkit.2.9.1-1-ubuntu64 home/ws/16S/apps

ADD vsearch_ubuntu /home/ws/16S/apps/vsearch_ubuntu
