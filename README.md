# Hyperledger-fabric
Hyperledger is a set of open-source blockchain frameworks and tools developed by the Linux Foundation to support the creation of enterprise-grade distributed ledger applications. 


#  1  SUDO APT UPDATE

![Screenshot 2025-05-17 085934](https://github.com/user-attachments/assets/17a36e0f-7c39-450d-af0d-54f7483fd5d0)



#   2  SUDO apt INSTALL  golang -go -y


![Screenshot 2025-05-17 090247](https://github.com/user-attachments/assets/7f37a869-fdfb-4d3f-9db3-1d8f0d6364b5)



#   3  INSTALL DOCKER

       Go to the official Docker download page:
           https://www.docker.com/products/docker-desktop

           Click “Download for Windows (WSL2)”.

           Run the installer.
             Step 3: Run Docker Desktop
           After installation, search and open "Docker Desktop".

           It may take a minute to initialize.

           Verify Docker Works = DOCKER VERSION


  ![image](https://github.com/user-attachments/assets/4403c53a-1986-48f5-8b08-3d5427bd0671)


# 4   Install cURL


 ![image](https://github.com/user-attachments/assets/dc90d72f-7d98-4bfd-8c58-c1a0c0362bff)

 ![image](https://github.com/user-attachments/assets/19da580d-89c1-4475-bbce-cb4b1b254618)


#  5 Node.js


![image](https://github.com/user-attachments/assets/afa82b16-1458-46a0-b71b-8267664e768e)
![image](https://github.com/user-attachments/assets/3e8ad877-81c1-458c-99cd-a54c5e807fce)


#  6 INSTALL jq

jq is used in Fabric scripts to parse JSON responses (like when you query chaincode or extract data from transactions).

It must be installed for Fabric to correctly process data in Bash scripts.



![image](https://github.com/user-attachments/assets/c931cc98-8545-472e-820d-71f01e61ee34)



# 7. Clone Fabric Samples 

Downloads Fabric binaries

Downloads Fabric Docker images

Creates fabric-samples folder

     mkdir ~/fabric-project && cd ~/fabric-project
     curl -sSL https://bit.ly/2ysbOFE | bash -s

![image](https://github.com/user-attachments/assets/908c960e-1f99-4e0a-82b0-6f9b87bf5486)
![image](https://github.com/user-attachments/assets/d07db8c3-389b-4295-a477-fe0861d2d4d5)



# 8. Go into test network /  Start the Network
          cd ~/fabric-project/fabric-samples/test-network
          ./network.sh up

![image](https://github.com/user-attachments/assets/74c9bbd2-de6a-460a-a82f-76585d1cc256)






**This spins up a local test Fabric network using Docker containers.**


# 9.Deploy Chaincode (Smart Contract)

                    ./network.sh deployCC -ccn basic -ccp ../asset-transfer-basic/chaincode-go -ccl go

