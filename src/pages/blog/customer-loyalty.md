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
  title: Customer Loyalty Programs That Stick
  description: >-
    A story about customer loyalty curabitur sed consectetur nisi. Integer sit
    amet commodo massa.
  extra:
    - name: 'og:type'
      value: website
      keyName: property
    - name: 'og:title'
      value: Customer Loyalty Programs That Stick
      keyName: property
    - name: 'og:description'
      value: >-
        A story about customer loyalty curabitur sed consectetur nisi. Integer
        sit amet commodo massa.
      keyName: property
    - name: 'og:image'
      value: images/3.jpg
      keyName: property
      relativeUrl: true
    - name: 'twitter:card'
      value: summary_large_image
    - name: 'twitter:title'
      value: Customer Loyalty Programs That Stick
    - name: 'twitter:description'
      value: >-
        A story about customer loyalty curabitur sed consectetur nisi. Integer
        sit amet commodo massa.
    - name: 'twitter:image'
      value: images/3.jpg
      relativeUrl: true
template: post
---
In the **Polkadot**, **Kusama **or **Parachain **context, stakers are called **Nominators**.

All chains based on the Polkadot (Substrate) framework use the [Nominated Proof of Stake](https://polkadot.network/launch-npos/) (NPoS) **consensus **protocol to secure the network: the [**Nominators**](https://wiki.polkadot.network/docs/en/learn-nominator) just nominates a list of trusted [**Validators**](https://wiki.polkadot.network/docs/en/learn-validator) who will validate the blocks and do the hard work of keeping the network secure.

Being
 a nominator is mostly a passive role: once you set it up, you receive a
 regular reward. The only thing you have to care about is to manage the 
Validators that you elect.

There are 3 simple steps to start being a nominator: **create account**, **bond funds** and **nominate**. In this guide, we will see how to nominate on Polkadot, these steps are exactly the same for Kusama or any parachain.

Depending on if you have a **Ledger hardware walle**t or not, you have 2 options. Please refer directly to the option you’d like (since there is redundant information in each):

*   [Staking with hot wallet account from the Polkadot JS app](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#a376)

*   [Staking with a Ledger cold wallet](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#8a2d) (Ledger Live or Polkadot JS app)

Beyond these few easy-clicking steps, **the choice of your validators is very important** for different reasons (see [our article](https://bldstackingnode.medium.com/announcing-1st-operational-validator-node-kusama-network-2cf90c22781e) explaining why). You have to pick at least a few validators (up to 16 total) to** make sure you are always actively nominating**. To help you with that, we have selected a list of [**trustful independent validators**](https://medium.com/bld-nodes/tutorial-how-to-stake-polkadot-kusama-on-chain-5ae50bd95aad#590c) who you can consider nominating (besides [us](https://kusama.subscan.io/account/Hf8C626KBAjitMV7w8AhQWDCiPgUU47htEwbomq5mDMKeyL) of course :-)). The cherry on the cake, some of those validators provide service on different networks.

![](https://miro.medium.com/max/750/1\*nlJ\_-njlE44LNCLz7UGDjg.gif)

*Kusama network*

# Staking with hot wallet accounts![](https://miro.medium.com/max/60/1\*dmorgX8L4hwj-z_pKLqvsA.png?q=20)

## Create accounts

All operations are made through the [**Polkadot JS app**](https://polkadot.js.org/apps)**. **It is recommended to install the [**Polkadot{.js} extension**](https://polkadot.js.org/extension/) to manage accounts. For more details, please refer to the official [Wiki page](https://wiki.polkadot.network/docs/en/maintain-guides-how-to-nominate-polkadot).

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

**

**Write down very carefully the mnemonic seed** and store it in a secure place. This will be the only way to recover your account in case you lose access to it.

Tick the confirm flag then click *Next.*

![](https://miro.medium.com/max/1136/1\*EJOeEGpqvsRyPszTZA0cIQ.png)*Create an account 2/3*

Give your account a name and a password, then click *Next.*![](https://miro.medium.com/max/60/1\*DeYCDniWD77wyKeByVuJPg.png?q=20)![](https://miro.medium.com/max/1133/1\*DeYCDniWD77wyKeByVuJPg.png)*Create an account 3/3*

Click on the *Save *button, your account is created.![](https://miro.medium.com/max/60/1\*H4hOu6\_0AJD3JIuf5YC4Kw.png?q=20)

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

**
