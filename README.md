# Decentralized-Timeline

Decentralized timeline service (e.g. Twitter, Instagram, Facebook) that harvests peer-to-peer and edge devices. Users have an identity and publish small text messages in their local machine, forming a local timeline. They can subscribe to other users timelines and will help to store and forward their content. Remote content is available when a source or source subscriber is online and can forward the information. Information from subscribed sources can be ephemeral and only stored and forwarded for a given time period.

It was developed in the course of Distributed Systems in Large Scale at University of Minho.

* Spread
* Java

## Start Guide

#### 1. Install Spread
Download [Spread](http://www.spread.org/download.html) and untar the file.
  ```
  tar -xvf filename.tar
  ```

Build daemon and java bindings:
  ```
  ./configure
  make
  sudo make install
  cd java
  ant
  ```

Copy configuration file (the file must be named `spread.conf` at the destination):
  ```
  sudo cp docs/sample.spread.conf /usr/local/etc/spread.conf
  ```

#### 2. Run Spread
  ```
  cd /usr/local/etc/
  spread
  ```
  
#### 3. Run APP
Run CentralMain once and then run UserMain as many times as you want.

