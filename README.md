# Base GPT 🐋



## Contents
- [**Introduction**](#introduction)
- [**About**](#About)
- [**Technicals**](#Technicals)
- [**Usecase**](#Usecase)
- [**Demo**](#Demo)
- [**Testing**](#Testing)
- [**Accessibility**](#Accessibility)
- [**Team**](#Team)
- [**Links**](#Links)



## Introduction
Sei Orcinus is an agentic api for getting real time crypto data on sei network.
We are simply building the next performance ready AI infrastructure on Sei used every way, anyway and at any time. Users can now access any realtime data on Sei at their convenient zone and platforms thanks to our agentic api. 


## About

## Technicals

<p align="center">
  <img src="./public/SOA.jpg" alt="Agent Image" width="800" style="max-width: 100%;">
</p>
The Archictecutral diagram describe the process of data flow of data from request to response in Sei Orcinus. The following are the meaning of the abbreviations in the architecture.

```
1. PA - Processing Agent
2. RA - Report Agent
3. PA KB - Processing Agent Knowledgebase
4. RA KB - Report Agent Knowledgebase
5. Tool Mapper - A dynamic runntime Hashmap that holds all supported tool functions.
6. AI model - Google Gemini AI model
```

### Project Structure
structure in the `src` file.
```
.
├── agents
│   ├── mod.rs
│   ├── processing_agent.rs
│   └── report_agent.rs
├── connection
│   ├── client.rs
│   ├── mod.rs
│   └── provider.rs
├── main.rs
├── mod.rs
├── response.rs
├── services
│   ├── getter
│   └── mod.rs
├── structure.txt
└── tools
    ├── mod.rs
    ├── tools_map.rs
    ├── utils.rs
    └── wrappers
```


## Usecase
1. ### Explorers🌐🔍: 
  Sei orcinus can be integrated into blockchain explorers on sei blockchain and other blockchain associated with to give users a comprehensive onchain data report of a **wallet address**, **token addresss**, **nft address**, **contract address** or any address on sei blockahin *mainnet or testnet*. A user don't need to waste time🤷 trying to use the explorer interface. Just tell the agent what you want concerning an address and you get a comprehensive reponse.
  
**Bonus:**
> *While your blockchain explorers provide a traditional explorer data experience for one address at a time, sei orcinus agent can provide a summary report of data for multiple address at one chat. We made user experience better across sei ecosystem through our api😎.*

2. ### Education👨‍🎓👩‍🎓:
  Sei orcinus can also be used as an educational tool. Imagine having a social media bot e.g twitter, discord, whatsapp, telegram or a web bot in the sei explorer. Using sei orcinus api automatically turns your bot to an agent able to educate your users on sei ecosystem.

3. ### Market Analytics📈:
  Sei orcinus can also be used for realtime market data analytical report. 

  ```Have you ever tried to get the real time market data of multiple tokens before in your portfolio😱? You can't afford to check prices sequentially if you have more tokens on your watch😰```.

  Sei orcinus enables you to get comprehensive market data report for multiple tokens at once 🎉.

**Productivity Hack Tips:**
>*As a user, I will definitely make sei orcinus my daily sidekid for anything on sei ecosystem knowing I have everything I need to be productive in one api endpoint which I can integrate to any of my favourite workspace, social media platform or dashboard platform🤔*

4. ### Onchain data Fetching:
Sei Orcinus api operates onchain and off-chain. Apart from fetching off-chain market data, You can use Sei orcinus to get onchain information of wallets, smart contracts, NFTs and NFT tokens.

**Experience:**
>*Users don't have to follow a structural prompt or technique to index data. Just express yourself and Sei Orcinus knows what to do!*



## Demo
The following images show case a real demo test of using sei orcinus agentic api.

1. **Getting a specific token balance for a wallet**
<p align="center">
  <img src="./public/sei_orcinus_test_01.png" alt="Agent Image" width="800" style="max-width: 100%;">
</p>


2. **Getting the real-time market price or capitalization of a token or multiple tokens**
<p align="center">
  <img src="./public/sei_orcinus_test_02.png" alt="Agent Image" width="800" style="max-width: 100%;">
</p>

3. **Knowing what a particular address is on Sei Mainnet Network** 
<p align="center">
  <img src="./public/sei_orcinus_test.png" alt="Agent Image" width="800" style="max-width: 100%;">
</p>

4. **Getting balance of an address or multiple address**
<p align="center">
  <img src="./public/sei_orcinus_test_advanced_test.png" alt="Agent Image" width="800" style="max-width: 100%;">
</p>


### Advanced Future

1. **Ability to Multi Task**
<p align="center">
  <img src="./public/sei_orcinus_multitasking.png" alt="Agent Image" width="800" style="max-width: 100%;">
</p>


## Testing
To run Sei Orcinus locally, simply clone the git repo, set your gemini api key and alchemy api key before  running  `cargo build --release` and `cargo run --release`
### steps

1. Clone git repo
```sh
  git clone https://github.com/ukangaekom/orcinus.git
```
2. Create a .env file in the root directory and add the following api keys.

```
  ALCHEMY_API_KEY=<ALCHEMY_API_KEY>
  GEMINI_API_KEY=<GOOGLE_GEMINI_API_KEY>
```

3. Run cargo build
```sh
  cargo build --release
```

4. Run the Axum Api
```sh
  cargo run --release

```

5. Open you postman and follow the test format.
Go to you local postman use the endpoint `http://localhost:8080/sei_orcinus_agent` and use a `post` request method.

**Note:** Use the json body type to send the request as the body type is strict.
```
{
   "message":"<Your Message>",
    "name":"<Any Name>",
    "media":"<Any Media name>"
}

```
Kindly send the request and get a response.


## Accessibility

Regarding Sei Orcinus Api accessibility, The api has been officially launched. You can message Ekomabasi Ukanga on [X](https://x.com/EkomUkanga) or [Telegram](https://t.me/Ekomart).

## Team

[Ekomabasi Ukanga](https://x.com/EkomUkanga) - Owner



## Links
[website](https://seiorcinus.vercel.app/)
[x_social_media](https://x.com/SeiOrcinus)








