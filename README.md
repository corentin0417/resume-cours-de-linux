# resume-cours-de-linux
#!/bin/bash
#######################################################################################
#Auteur	:  Corentin,
#Date 	: 19-03-2022
#Processus: création système fichier 
#######################################################################################
echo	
sudo groupadd -g  2043 rech
sudo groupadd -g  2006 dev	
sudo groupadd -g  2006 dev	
sudo groupadd -g  2006 dev	
sudo groupadd -g  2004 ing
sudo groupadd -g  2010 adminrech
sudo groupadd -g  2020 admindev
sudo groupadd -g  2017 admining
sudo groupadd -g  2035 Tech

sudo useradd BPO --password Bpob2022@ --uid 1010 --create-home --groups Tech,adminrech,admindev,admining
sudo useradd PDU --password Pdup2022@ --uid 1021 --create-home --groups rech,Tech
sudo useradd SFR --password Sfrs2022@--uid 1030 --create-home --groups rech,Tech
sudo useradd ACH --password Acha2022@ --uid 1041 --create-home --groups rech,Tech
sudo useradd JLA --password Jlaj2022@ --uid 1037 --create-home --groups rech,Tech
sudo useradd SAN --password Sans2022@ --uid 1025 --create-home --groups rech,Tech
sudo useradd NDU --password Ndun2022@ --uid 1028 --create-home --groups dev,Tech,admindev
sudo useradd LTU --password Ltul2022@ --uid 1050 --create-home --groups dev,Tech
sudo useradd KTH --password Kthk2022@ --uid 1067 --create-home --groups dev,Tech
sudo useradd JDE --password Jdtj2022@ --uid 1029 --create-home --groups dev,Tech
sudo useradd HST --password Hsth2022@ --uid 1005 --create-home --groups ing,Tech,admining
sudo useradd RMA --password Rmar2022@ --uid 1012 --create-home --groups ing,Tech 
sudo useradd ADE --password Adea2022@ --uid 1032 --create-home --groups ing,Tech

sudo mkdir -p /home/rechcom
sudo mkdir -p /home/devcom
sudo mkdir -p /home/ingcom

sudo mkdir -p /home/PDU/{pub,rech,adminrech}
sudo mkdir -p /home/SFR/{pub,rech}
sudo mkdir -p /home/ACH/{pub,rech}
sudo mkdir -p /home/JLA/{pub,rech}
sudo mkdir -p /home/SAN/{pub,rech}

sudo mkdir -p /home/NDU/{pub,dev,admindev}
sudo mkdir -p /home/LTU/{pub,dev}
sudo mkdir -p /home/KTH/{pub,dev}
sudo mkdir -p /home/JDE/{pub,dev}

sudo mkdir -p /home/HST/{pub,ing,admining}
sudo mkdir -p /home/RMA/{pub,ing}
sudo mkdir -p /home/ADE/{pub,ing}

sudo chown :dev /home/devcom  
sudo chmod 1760 /home/devcom
sudo chown :rech /home/rechcom
sudo chmod 1760 /home/rechcom
sudo chown :ing /home/ingcom
sudo chmod 1760 /home/ingcom

sudo chown :adminrech /home/PDU/adminrech
sudo chmod 1760 /home/PDU/adminrech
sudo chown :admindev /home/NDU/admindev
sudo chmod 1760 /home/NDU/admindev
sudo chown :admining /home/HST/admining
sudo chmod 1760 /home/HST/admining

sudo chown :rech /home/PDU/rech
sudo chmod 1760 /home/PDU/rech
sudo chown :rech /home/SFR/rech
sudo chmod 1760 /home/SFR/rech
sudo chown :rech /home/ACH/rech
sudo chmod 1760 /home/ACH/rech
sudo chown :rech /home/JLA/rech
sudo chmod 1760 /home/JLA/rech
sudo chown :rech /home/SAN/rech
sudo chmod 1760 /home/SAN/rech

sudo chown :dev /home/NDU/dev
sudo chmod 1760 /home/NDU/dev
sudo chown :dev /home/LTU/dev
sudo chmod 1760 /home/LTU/dev
sudo chown :dev /home/KTH/dev
sudo chmod 1760 /home/KTH/dev
sudo chown :dev /home/JDE/dev
sudo chmod 1760 /home/JDE/dev

sudo chown :ing /home/HST/ing
sudo chmod 1760 /home/HST/ing
sudo chown :ing /home/RMA/ing
sudo chmod 1760 /home/RMA/ing
sudo chown :ing /home/ADE/ing
sudo chmod 1760 /home/ADE/ing

sudo chown :Tech /home/PDU/pub
sudo chmod 1740 /home/PDU/pub
sudo chown :Tech /home/SFR/pub
sudo chmod 1740 /home/SFR/pub
sudo chown :Tech /home/ACH/pub
sudo chmod 1740 /home/ACH/pub
sudo chown :Tech /home/JLA/pub
sudo chmod 1740 /home/JLA/pub
sudo chown :Tech /home/SAN/pub
sudo chmod 1740 /home/SAN/pub
sudo chown :Tech /home/NDU/pub
sudo chmod 1740 /home/NDU/pub
sudo chown :Tech /home/LTU/pub
sudo chmod 1740 /home/LTU/pub
sudo chown :Tech /home/KTH/pub
sudo chmod 1740 /home/KTH/pub
sudo chown :Tech /home/PDU/pub
sudo chmod 1740 /home/JDE/pub
sudo chown :Tech /home/HST/pub
sudo chmod 1740 /home/HST/pub
sudo chown :Tech /home/RMA/pub
sudo chmod 1740 /home/RMA/pub
sudo chown :Tech /home/ADE/pub
sudo chmod 1740 /home/ADE/pub
