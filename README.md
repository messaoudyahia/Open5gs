
# Open5gs - WebUi - UERANSIM Installation in Ubuntu 20.04

This is a documentation for installing Open5gs, webUI, and UERANSIM in Ubuntu 20.04

## 1- Installing MongoDB version 4.4.8

Google it 

## 2- Installing Open5gs

```
$ sudo add-apt-repository ppa:open5gs/latest
$ sudo apt update
$ sudo apt install open5gs

```


## 3- Installing NodeJS

```
 $ sudo apt update
 $ sudo apt install curl
 $ curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
 $ sudo apt install nodejs

```


## 4- Installing WebUI for Open5GS

```
$ curl -fsSL https://open5gs.org/open5gs/assets/webui/install | sudo -E bash -
```

- To test that the webUI works, go to the browser and tap " 127.0.0.1:3000 " (username= admin, password= 1423)


## 5- Installing UERANSIM

```
$ sudo apt install make gcc g++ libsctp-dev lksctp-tools iproute2 git
$ sudo snap install cmake --classic
$ git clone https://github.com/aligungr/UERANSIM
$ cd ~/UERANSIM
$ make
```


## Testing UERANSIM request to Open5gs

1- enter to the UERANSIM/config folder (previously created)
2- tap the following command:

```
$ ../build/nr-gnb -c open5gs-gnb.yaml
```

- If the request passed you will see " NG Setup procedure is successful "




## References
- https://www.youtube.com/watch?v=NxFOqR_41Bs
- https://www.youtube.com/watch?v=QSYUK0LTbMk
- https://github.com/mohitkr05/5G_stuff/blob/main/clickops/01_Open5GS_UeRANSIM/single_vm.md
- https://open5gs.org/open5gs/docs/guide/01-quickstart/
- https://medium.com/rahasak/5g-core-network-setup-with-open5gs-and-ueransim-cd0e77025fd7
# Open5gs - WebUi - UERANSIM Installation in Ubuntu 20.04

This is a documentation for installing Open5gs, webUI, and UERANSIM in Ubuntu 20.04

## 1- Installing MongoDB version 4.4.8

Google it 

## 2- Installing Open5gs

```
$ sudo add-apt-repository ppa:open5gs/latest
$ sudo apt update
$ sudo apt install open5gs

```


## 3- Installing NodeJS

```
 $ sudo apt update
 $ sudo apt install curl
 $ curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
 $ sudo apt install nodejs

```


## 4- Installing WebUI for Open5GS

```
$ curl -fsSL https://open5gs.org/open5gs/assets/webui/install | sudo -E bash -
```

- To test that the webUI works, go to the browser and tap " 127.0.0.1:3000 " (username= admin, password= 1423)


## 5- Installing UERANSIM

```
$ sudo apt install make gcc g++ libsctp-dev lksctp-tools iproute2 git
$ sudo snap install cmake --classic
$ git clone https://github.com/aligungr/UERANSIM
$ cd ~/UERANSIM
$ make
```


## Testing UERANSIM request to Open5gs

1- enter to the UERANSIM/config folder (previously created)
2- tap the following command:

```
$ ../build/nr-gnb -c open5gs-gnb.yaml
```

- If the request passed you will see " NG Setup procedure is successful "




## References
- https://www.youtube.com/watch?v=NxFOqR_41Bs
- https://www.youtube.com/watch?v=QSYUK0LTbMk
- https://github.com/mohitkr05/5G_stuff/blob/main/clickops/01_Open5GS_UeRANSIM/single_vm.md
- https://open5gs.org/open5gs/docs/guide/01-quickstart/
- https://medium.com/rahasak/5g-core-network-setup-with-open5gs-and-ueransim-cd0e77025fd7
