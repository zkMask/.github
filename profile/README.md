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

## Links To Repositories
- [React-Native Frontend](https://github.com/zkMask/mobile-frontend)
- [AI and Integrations BackEnd](https://github.com/zkMask/backend)
- [Smart Contracts](https://github.com/zkMask/contracts)
- [Zk-Circuits](https://github.com/zkMask/zkMask-circuits)
- [Subgraph](https://github.com/zkMask/zkMask-subgraph)
- [Push Channel](https://github.com/zkMask/zkMask-pushNotif)
- [Demo Dapp](https://github.com/zkMask/TestingDapp)

**Architecture**
![reg_flow](https://github.com/zkMask/.github/assets/76250660/9462e666-f75e-494a-96ae-a254fda33a32)
![auth_flow](https://github.com/zkMask/.github/assets/76250660/40fa5ffd-899e-4e2c-b068-b2cd733a0363)

At the time of user registration, the user needs to connect his wallet through walletconnect, this helps in login sessions of user for the public hash association which might be needed to generate proof. The unique key is generated randomly using strong cryptographic functions and logics. The Poseidon hash of the unique key is stored in a mapping for verification and proof generation. Along with this he needs to capture 5-6 different images of his face for the dataset to be used by the AI model.<br>

Now whenever the user initiates any transaction through a dapp which integrates our app, he will have to verify on another device (we did this to add another back up method). He logins into the app, gets the notif of a new authentication request which he could either accept or decline. When he accepts the request, he needs to scan his face, the face then goes to DeepFace AI model which recognises whether the user is right and then sends the inputs to the custom implemented zk circuit which does the further verification and outputs the result to the dapp who is listening to the zkMask's contract. Based on the result, the dapp performs the further transactions.

**ZK Implementation**
We are using custom circom circuits implementation to verify user anonymously. The circom circuit take the unique key as private input and the Poseidon hash as the public input and using the circuit maths verifies that the proof generated is correct or not based on the circuit logic. 
 
The App is Deployed on Goerli, Gnosis Chiado testnet, polgyon zkevm ---- .


