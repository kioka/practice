##　環境
```sh
% sw_vers
ProductName:	Mac OS X
ProductVersion:	10.13.1
BuildVersion:	17B48s
% vagrant -v 
Vagrant 2.0.1
% VBoxManage -v
5.2.0r118431
```

## 参考サイト
UbuntuにChefをインストールする
http://kaworu.jpn.org/ubuntu/Ubuntu%E3%81%ABChef%E3%82%92%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB%E3%81%99%E3%82%8B


- name: Add sbt apt key 
  apt_key:
    keyserver: hkp://keyserver.ubuntu.com:80
    id: 2EE0EA64E40A89B84B2DF73499E82A75642AC823

- name: Install sbt
  apt:
    name: sbt
    state: latest
    install_recommends: no