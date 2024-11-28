# [Cysic](https://testnet.cysic.xyz/m/referral/invite). Launching Testnet node.
*Disclaimer: The author of this guide, which is exclusively informational material, does not bear any responsibility for the actions of readers. There are no fraudulent or spam links in the guide. All materials were obtained from official sources, links to which can be found at the end of each guide. This post is copyrighted by Nod Mafia.*

![image](https://github.com/user-attachments/assets/16c5f272-df25-4cea-8996-d34a37d47150)



Cysic is home to the leading real-time ZK Proof Layer, featuring state-of-the-art hardware. Our mission is to hyperscale the ZK revoluttion by delivering Zero Knowledge Proofs with unmatched speed, simplicity, andcost-efficiency.

To start the node we need referral codes, which can be found in [discord Cysic](https://discord.gg/hCbjdJDy) in the [invite-codes](https://discord.com/channels/1127954093990760539/1308397379954671696) channel . Verify, copy the referral code from the channel.  After that, connect your wallet on [Cysic testnet site](https://testnet.cysic.xyz/m/referral/invite) (We recommend using Keplr Wallet) and paste the referral code.

![image](https://github.com/user-attachments/assets/ede42d96-bc95-49f5-b674-0cfd7dc4c8cd)


## [Cysic Testnet](https://testnet.icn.global). What you need to do?

Follow the initial steps: enter your nickname and avatar. Then in the top right corner, connect Keplr. Your new cysic address will be connected automatically  

![image](https://github.com/user-attachments/assets/8b0e920c-e74a-4e27-a502-7f570b52455d)


Now we need to get the $CYS tokens. To do this, click on the faucet button in the upper right corner of the screen.

![Cysic1](https://github.com/user-attachments/assets/354d886c-5fdc-4cac-805c-4dbc3d23e9c4)


## Cysic Testnet Node Launch. All actions 

Prover Node requirements:
- Ubuntu 22.04 or newer
- 64CPU/280gbRAM/100SSD/2x 3070 or 2080 GPU

Verifier Node requirements:
- Ubuntu 22.04 or newer
- 1CPU/1gbRAM/8SSD

### Installing the light version - Verifier

Go into Ubuntu and update.
```
sudo apt update
sudo apt upgrade
```
Next, install end deploy screen for the node.
```
sudo apt install screen
screen -S Cysic
```
Run the node official installation script. Instead of 0x-Fill-in-your-reward-address-here specify the address of your  EVM wallet!
```
curl -L https://github.com/cysic-labs/phase2_libs/releases/download/v1.0.0/setup_linux.sh > ~/setup_linux.sh && bash ~/setup_linux.sh 0x-Fill-in-your-reward-address-here
```
![Cysic2](https://github.com/user-attachments/assets/0c5b6185-dc0d-482b-a3d9-e6f1ee6f4f86)

If you see such logs after a couple of minutes, it means that the installation is correct.


When you create a node, you will be given a special key that will be saved under the path .cysic/keys/ . Save this .key file. It is required for restarting the node, if you lose the file, it will be impossible to start the node!

If you want to start an already installed Cysic node use the start.sh script at the path cysic-verifier/. Log in to screen Cysic if you are not already in it:

```
screen -r Cysic
```

Stop the node with the key combination:

```
CTRL + C
```

Run the start.sh script 

```
cd
cd cysic-verifier
./start.sh
```

## How to properly use a node inside the terminal.

To minimize the screen without turning off the node, use the key combination:

```
CTRL+A,D
```

Open screen Cyisc to see the logs:

```
screen -r Cysic
```

Delete screen:

```
screen -XS Cysic quit
```

To turn off the node, use the key combination inside the Cysic screen:

```
CTRL+C
```

A list of all the screens:

```
screen -ls
```

## NodeMafia. We hope our content is useful for you.
![image](https://github.com/user-attachments/assets/e0dc7aee-f823-41d2-a406-9e8837778964)

GitHub: https://github.com/NodeMafia

Medium: https://medium.com/@nodemafia

Telegram: https://t.me/nodemafia

Teletype: https://teletype.in/@nodemafia

Twitter: https://x.com/NodeMafia
