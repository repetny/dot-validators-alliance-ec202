---
title: 'Tutorial: how to stake Polkadot/Kusama on-chain'
author: src/data/authors/jane-doe.yaml
excerpt: >-
  A story about customer loyalty curabitur sed consectetur nisi. Integer sit
  amet commodo massa.
date: '2021-01-03'
thumb_image: images/3_thumb.jpg
thumb_image_alt: A group of people working in a cafe
image: images/modern-kangaroo.png
image_alt: A group of people working in a cafe
seo:
  title: Tutorial - how to stake Polkadot/Kusama on-chain
  description: >-
    A story about customer loyalty curabitur sed consectetur nisi. Integer sit
    amet commodo massa.
  extra:
    - name: 'og:type'
      value: website
      keyName: property
    - name: 'og:title'
      value: Tutorial - how to stake Polkadot/Kusama on-chain
      keyName: property
    - name: 'og:description'
      value: >-
        Tutorial: how to stake Polkadot/Kusama on-chain.
      keyName: property
    - name: 'og:image'
      value: images/3.jpg
      keyName: property
      relativeUrl: true
    - name: 'twitter:card'
      value: summary_large_image
    - name: 'twitter:title'
      value: Tutorial - how to stake Polkadot/Kusama on-chain
    - name: 'twitter:description'
      value: >-
        A story about customer loyalty curabitur sed consectetur nisi. Integer
        sit amet commodo massa.
    - name: 'twitter:image'
      value: images/3.jpg
      relativeUrl: true
template: post
---
In the **Polkadot**, \*\*Kusama \*\*or \*\*Parachain \*\*context, stakers are called **Nominators**.

All chains based on the Polkadot (Substrate) framework use the [Nominated Proof of Stake](https://polkadot.network/launch-npos/) (NPoS) \*\*consensus \*\*protocol to secure the network: the [**Nominators**](https://wiki.polkadot.network/docs/en/learn-nominator) just nominates a list of trusted [**Validators**](https://wiki.polkadot.network/docs/en/learn-validator) who will validate the blocks and do the hard work of keeping the network secure.

Being a nominator is mostly a passive role: once you set it up, you receive a regular reward. The only thing you have to care about is to manage the Validators that you elect.

There are 3 simple steps to start being a nominator: **create account**, **bond funds** and **nominate**. In this guide, we will see how to nominate on Polkadot, these steps are exactly the same for Kusama or any parachain.

Depending on if you have a **Ledger hardware walle**t or not, you have 2 options. Please refer directly to the option you’d like (since there is redundant information in each):

*   [Staking with hot wallet account from the Polkadot JS app](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#a376)

*   [Staking with a Ledger cold wallet](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#8a2d) (Ledger Live or Polkadot JS app)

Beyond these few easy-clicking steps, **the choice of your validators is very important** for different reasons (see [our article](https://bldstackingnode.medium.com/announcing-1st-operational-validator-node-kusama-network-2cf90c22781e) explaining why). You have to pick at least a few validators (up to 16 total) to\*\* make sure you are always actively nominating\*\*. To help you with that, we have selected a list of [**trustful independent validators**](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#590c) who you can consider nominating (besides [us](https://kusama.subscan.io/account/Hf8C626KBAjitMV7w8AhQWDCiPgUU47htEwbomq5mDMKeyL) of course :-)). The cherry on the cake, some of those validators provide service on different networks.

![](https://miro.medium.com/max/750/1\*nlJ\_-njlE44LNCLz7UGDjg.gif)

*Kusama network*

# Staking with hot wallet accounts

## Create accounts

All operations are made through the [**Polkadot JS app**](https://polkadot.js.org/apps)\*\*. \*\*It is recommended to install the [**Polkadot{.js} extension**](https://polkadot.js.org/extension/) to manage accounts. For more details, please refer to the official [Wiki page](https://wiki.polkadot.network/docs/en/maintain-guides-how-to-nominate-polkadot).

For a security matter, it is recommended to create 2 separate accounts:

*   **Stash account**: where you keep your funds for nomination

*   **Controller account**: to manage common operations of start/stop nomination and nominate validators

***Note**: if you want to use a Ledger wallet for staking, please refer to the the last section of this tutorial.*

Select the network and click the *Switch* button:

![](https://miro.medium.com/max/874/1\*dmorgX8L4hwj-z_pKLqvsA.png)

*Select network*

You can also use these direct links for [Polkadot](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Frpc.polkadot.io#/accounts) and [Kusama](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Fkusama-rpc.polkadot.io#/accounts).

Here, you can either chose to create a regular account or use a Ledger hardware wallet.

![](https://miro.medium.com/max/1829/1\*rRp9V3cmJd7\_KSG4HT22tA.png)*Account page of Polkadot’s app*

Click on Add account:

![](https://miro.medium.com/max/60/1\*o_frGtgB1oCE8OpY2-avhA.png?q=20)![](https://miro.medium.com/max/1138/1\*o_frGtgB1oCE8OpY2-avhA.png)*Create an account 1/3*

\*\*

**Write down very carefully the mnemonic seed** and store it in a secure place. This will be the only way to recover your account in case you lose access to it.

Tick the confirm flag then click *Next.*

![](https://miro.medium.com/max/1136/1\*EJOeEGpqvsRyPszTZA0cIQ.png)*Create an account 2/3*

Give your account a name and a password, then click *Next.*![](https://miro.medium.com/max/60/1\*DeYCDniWD77wyKeByVuJPg.png?q=20)![](https://miro.medium.com/max/1133/1\*DeYCDniWD77wyKeByVuJPg.png)*Create an account 3/3*

Click on the \*Save \*button, your account is created.![](https://miro.medium.com/max/60/1\*H4hOu6\_0AJD3JIuf5YC4Kw.png?q=20)

**Repeat the same steps to create your Stash account.**

You should now have your 2 accounts created.

![](https://miro.medium.com/max/1731/1\*H4hOu6\_0AJD3JIuf5YC4Kw.png)*Accounts ready for nomination*

## Funding the accounts

Next, you need to **add funds** to your **stash account**,
from another account or from a centralized exchange (if you don’t have
any, maybe you can ask your grandma to send you some :-)).

You can click on the account name to know the public address to send funds.

![](https://miro.medium.com/max/336/1\*U0uPhb3vMOPaK2oeF1JDig.png)

*Account public address*

Once your stash account is funded, use the *Send* button to transfer a small percentage to your controller account.

![](https://miro.medium.com/max/1136/1\*bvK1ZBc1vSuw4UVy6lGgBw.png)*Transfer funds 1/2*

Select the controller account and set a small amount to be able to manage the transaction fees. Then click on *Make Transfer.*

![](https://miro.medium.com/max/1139/1\*63uOM5vD89LieHySbOVwzQ.png)*Transfer funds 1/2*

Click on *Sign and Submit.*

Your accounts are funded and **ready to nominate**.

![](https://miro.medium.com/max/1730/1\*SgcgrP8PF_U3O4cKMLe89Q.png)

## Bond funds and nominate

Go to the *Network / Staking tab.*

![](https://miro.medium.com/max/245/1\*H0AgcWW5BfuiRhJY_jzN1g.png)

*Staking tab*

\*\*

Go to the *Account actions* menu.![](https://miro.medium.com/max/1819/1\*etzMaOF7fnovNXPO9qaarw.png)*Account actions in the Staking tab*

\*\*

Click on *+Nominator.*![](https://miro.medium.com/max/1133/1\*gkFvMaM_DMyclNcqDKwNqw.png)*Bonding funds*

Select the stash and controller account. Set the\*\* total amount you want to bond for your nominations\*\*, then click on the *next* button.

![](https://miro.medium.com/max/1136/1\*ZlcIaXgeK_GI9GUi59eFYg.png)*Select validators*

Here, you have to **search for the validators** you want to select in the \*\*left panel \*\*and click on it to move it to the right panel that represents the **accounts you nominate**. \*See \*[*recommended validators*](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#590c)

Then, click on *Bond & Nominate* to send the transaction.

![](https://miro.medium.com/max/1571/0\*OCbZKigIqesBKOiX)

And that’s it, you have successfully set your nominations, your funds work for you now!

[Jump to conclusion](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#d85d)

# Staking with a Ledger wallet

If
you have a Ledger wallet and you prefer to nominate with it, you will
not be able to have 2 separate accounts as this function is not yet
available (we are writing this guide in April 2021).

You have the choice to stake either from:

*   [the Ledger Live app](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#031e) — **only for Polkadot**

*   [the Polkadot JS app](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#7430) — **Polkadot and Kusama**

**Warning**: it is not yet possible to create an account for Kusama from the Ledger Live app, you can only install Kusama.

**Note**: it is recommended to use a **Ledger Nano X** which has more memory, you can only have a few applications on a Nano S.

# Stake from the Ledger Live app

We will use here the staking function directly from the [**Ledger Live**](https://www.ledger.com/ledger-live) app.

***Note**: If you prefer watching a video, the Polkadot team made a *[*great tutorial*](https://youtu.be/obZyGeHrm_M)*.*

## Create an account

*   Open the *Manager* tab in Ledger Live.

*   Connect and unlock your Ledger device.

*   Find Polkadot or Kusama in the app catalog and install it.

![](https://miro.medium.com/max/1023/1\*vxIc1cn9C2MXBSKyxq49Zg.png)*Ledger Live Manager*

Then, open the \*Accounts \*tab.![](https://miro.medium.com/max/60/0\*o6W0P7VrZBy5xn6l?q=20)![](https://miro.medium.com/max/996/0\*o6W0P7VrZBy5xn6l)*Ledger Live Accounts*

Click on *Add account*.

![](https://miro.medium.com/max/499/0\*L2ezr6yNlp0bbwpa)

Select the network (Polkadot or Kusama) and then follow the steps to create your account.

## Funding the account

Next, you need to **add funds** to your **stash account**, From another account or from a centralized exchange (if you don’t have any, maybe you can ask your grandma to send you some :-)).

## Bond funds and nominate

From the *Account* menu, open your account details.

\*\*

![](https://miro.medium.com/max/989/1\*cl8iYwIVoV47iP8\_c3anuQ.png)*Account details*

\*\*

click on *Earn rewards.*

\*\*![](https://miro.medium.com/max/54/1\*MBUZUQwi22gOL8o1031GAQ.png?q=20)![](https://miro.medium.com/max/495/1\*MBUZUQwi22gOL8o1031GAQ.png)

*Bonding amount screen*

Set the **total amount you want to bond** for your nominations and \*Continue. \*Once your funds are bonded, click on *Nominate*.

![](https://miro.medium.com/max/715/1\*drKl08i3a3JkcqSlds711Q.png)

*Selecting validators*

Here, you have to **search for the validators** you want to select and tick the box on the right. \*See \*[*recommended validators*](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#590c)

And that’s it, you have successfully set your nominations, your funds work for you now!

[Jump to conclusion](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#d85d)

# Stake from the Polkadot JS app

A few prerequisites:

*   It is not possible to use a Ledger with the Firefox, you will have to use another browser.

*   Make sure that the Ledger Live application is closed to avoid any conflict.

All operations are made through the [**Polkadot JS app**](https://polkadot.js.org/apps)**.** For more details, please refer to the official [Wiki page](https://wiki.polkadot.network/docs/en/learn-ledger).

First, go to the *Settings* tab.

![](https://miro.medium.com/max/1750/1\*qRv34tknFJ4NPZS-XuQS7Q.png)*Polkadot JS app settings*

\*\*

select *Attach Ledger via WebUSB* and *Save.*

## Create an account

Select the network in the up left corner and click the *Switch* button:

![](https://miro.medium.com/max/874/1\*dmorgX8L4hwj-z_pKLqvsA.png)

*Select network*

You can also use these direct links for [Polkadot](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Frpc.polkadot.io#/accounts) and [Kusama](https://polkadot.js.org/apps/?rpc=wss%3A%2F%2Fkusama-rpc.polkadot.io#/accounts).

![](https://miro.medium.com/max/1829/1\*rRp9V3cmJd7\_KSG4HT22tA.png)*Account page of Polkadot’s app*

On your Ledger device, select the Polkadot menu to see Polkadot Ready on it (looks like my fingers were dirty…).

![](https://miro.medium.com/max/828/0\*sd9IR5zpYjqTYyl9)

Click on *Add via Ledger*:

![](https://miro.medium.com/max/1139/1\*kIiT4gv8zIirDvfFR-XtVQ.png)*Add a ledger account*

**Note**:
if you already created an account on your ledger (with Ledger Live app
for example), you have to choose an unused account in the *Account type*.

![](https://miro.medium.com/max/1559/0\*TACPfu9MbFk68FM-)

Click the *Save* button.

## Fund the account

Next, you need to **add funds** to your account, from another account or from a centralized exchange (if you don’t have any, maybe you can ask your grandma to send you some :-)).

You can click on the account name to know the public address to send funds.

![](https://miro.medium.com/max/60/1\*U0uPhb3vMOPaK2oeF1JDig.png?q=20)![](https://miro.medium.com/max/336/1\*U0uPhb3vMOPaK2oeF1JDig.png)

*Account public address*

## Bond funds

Then, you have to bond your funds that will be used for staking. Go to the *Network / Staking tab.*

\*\*![](https://miro.medium.com/max/245/1\*H0AgcWW5BfuiRhJY_jzN1g.png)

*Staking tab*

Go to the *Account actions* menu.![](https://miro.medium.com/max/1733/1\*CGKsrS8bBEkaUYIFPcuE8g.png)*Account actions in the Staking tab*

Click on *+Stash* (the *+Nominator* button will not work since Ledger device does not support batch transactions)*.*![](https://miro.medium.com/max/1071/0\*UipEtHYZ66s70x4f)*Bonding funds*

Set the** total amount you want to bond for your nominations**, then click on the *Bond* button.![](https://miro.medium.com/max/1159/0\*\_GkfO4-V7cGd4eyU)*Sign bonding transaction*

**

Click on *Sign and Submit*, then review and approve the transaction on the Ledger device.![](https://miro.medium.com/max/1596/0\*zszfJRc7OfDgB1sB)*Nominator account with bonded funds*

## Nominate validators

Your funds are bonded, now you are ready to nominate. Click on the *Nominate* button next to your account (not the *+Nominator* button on the top).

![](https://miro.medium.com/max/1065/1\*YL7FvzpM9fw7zi6uWd8TBQ.png)*Select validators*

\*\*Here, you have to **search for the validators** you want to select in the **left panel **and click on it to move it to the right panel that represents the **accounts you nominate**. *See *[*recommended validators*](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#590c)

When you have selected all the validators you want, click on *Nominate.*

**![](https://miro.medium.com/max/1187/0\*qAg3UK2eqBE-tH45)

Click on *Sign and Submit*, then review and approve the transaction on the Ledger device.

![](https://miro.medium.com/max/60/0\*OCbZKigIqesBKOiX?q=20)![](https://miro.medium.com/max/1571/0\*OCbZKigIqesBKOiX)

And that’s it, you have successfully set your nominations, your funds work for you now!

[Jump to conclusion](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#d85d)

# Recommended validators

Here you can find the list of trustful and independent validators that we know to be serious and secure.

## Kusama Network

*   bLd Nodes (us): Hf8C626KBAjitMV7w8AhQWDCiPgUU47htEwbomq5mDMKeyL

*   REPE: FaBN1AxtJu21x2cUqvdF5VcVUAfzfqyvJPvwgsdwo3pkdr9

*   Polkadotters: FVAFUJhJy9tj1X4PaEXX3tDzjaBEVsVunABAdsDMD4ZYmWA

*   PromoTeam Validator: Dm4uKxZJZHJbpZpfnYPiHnbgyHWKMU1s5h6X7kqjfYv1Xkk

*   Stakenode_Powernode: CuiwESD49ggEAQ9131Gt948xw11PiWQNXkuR2R2Jt7rYSck

## Polkadot Network

*   Polkadotters: 16A4n4UQqgxw5ndeehPjUAobDNmuX2bBoPXVKj4xTe16ktRN

## StaFi Protocol

*   PromoTeam: 31dAkYPQWqLooi8STtH4u91ybv3DBtyT4Tdn8VZbkGYtPFfQ

*   pathrocknetwork: 32yfaVgxp2bArkKotgiVrdqhbP17Lwc6KkmtgSZRazjuwpae

*   oceanblock-ov: 35pwfNAzJKnnSxjbdoN8DdNPvXE2ChXiHL4Z4N5oDFdhMPoU

*   Polkadotters: 32cHeCGWM3X8W8ypxxCaCgE43BpHt6QtmPFKKMFS7NG1QphQ

## HydraDX

*   Polkadotters: 7K296SU5tGTCkpYntSonyohsvvCZr2wmaKzCf9Ed6rAv6ij1

## Darwina

*   Polkadotters (Darwinia): 2q2y8DBhaTmgC2Au9tSXSshCkDXhmj9rPW945yxqBf52rGRK

*   Polkadotters (Darwinia Crab): 5DvoL2BNoSm7wRt2tfZ6WW5QFrxm68GLv5SCrPQ4JBLjbvpL

## Centrifuge

*   Polkadotters: 4dCqn4vxVhWm15TFTUGxF6UrNx6zm2VDnS7RAHYFX3mov24q

# Conclusion

We have just seen here how to stake funds and become a real on-chain nominator in just a few simple steps.

If you are staking on centralized exchanges, we encourage you to consider staking on-chain as this gives you an active role in the blockchain ecosystem besides a better reward (CEX have to pay themselves in one way or another right?).

Please feel free to reach us with any question or difficulty you have.
