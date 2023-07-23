# ZKMask 🎭
### (Easy and Secure transactions using 2 Factor Authentication)

Once the keys are lost the Funds are too! 

Through ZKMask we are trying to prevent user funds by adding an extra layer of security by leveraging the power of AI Face Recognition and ZK Proofs.

### What is ZK Mask?
ZKMask is the ultimate 2 Factor Authentication app needed to secure all transactions through Face Recognition and proving the identity by Zero Knowledge Proofs eliminating any centralization and privacy risks. The architecture of the project makes it different from traditional 2 factor authentication apps - biometric or secret code based. The project leverages decentralization, AI, ZKP to it's best to prevent users from one of the most common and devastating risks. 

### How it is built?
The project consists of several parts:
- Registration of user through WalletConnect
- User recognition (not identification) through DeepFace AI model
- Anonymous Zero-Knowledge Idenetification of user signature through circom circuits.
- Transaction initiation or rejection

**Architecture**


The DeepFace AI model verifies if the owner of the key is the one signing the transaction and reverts the process of 2FA if this does not happen the Zero Knowledge smart contract generates the proof for the same after which only the user signs the transaction and makes it go through. This 2 Factor Authentication using the  Deepface AI model and Zero Knowledge Proof brings reliability to the security layer added through ZKMask.

## Links To Repositories
- [React-Native Frontend](https://github.com/zkMask/mobile-frontend)
- [AI and Integrations BackEnd](https://github.com/zkMask/backend)
- [Smart Contracts](https://github.com/zkMask/contracts)
- [Zk-Circuits](https://github.com/zkMask/zkMask-circuits)
- [Subgraph](https://github.com/zkMask/zkMask-subgraph)
- [Push Channel](https://github.com/zkMask/zkMask-pushNotif)
- [Demo Dapp](https://github.com/zkMask/TestingDapp)

## 
The problem of losing funds due to losing control over the private key is a very common problem that many crypto users face. ZKMask solves this problem by adding an additional layer of security by which even the wallets with compromised keys wallets remain safe by 2FA. This additional layer of security uses concepts of Artificial Intelligence and Zero-Knowledge for verification using various Face alignments, detection, embeddings, and features extraction and ------------- using Zero Knowledge Concepts. 

Users have to first register their Identity on the ZKMask mobile app by capturing their photo for future verification by the AI model. Later this sample is used as a sample for face verification when the user wants to perform 2FA before signing a transaction. During 2FA the captured face image is taken and passed through the DeepFace AI model that checks if the captured image has any resemblance with the images registered already on our App. If YES the image is passed for Proof generation contract by ZK Model or else is rejected and 2FA fails and the transaction security is maintained. 

In the ZK Model the face ----------------------------------------------.
This ensures that the face verification done by the AI model is done correctly and ZK gives the Proof for same.
 
The App is Deployed on Goerli, Gnosis Chiado testnet, polgyon zkevm ---- .


