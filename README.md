# EchoChamber_abortion

## Abstract:
Echo chamber is a phenomenon where users’ opinions get amplified and reinforced by information spreading inside a homogeneous group because people tend to believe the information that is similar or could support their own beliefs. The effect of echo chambers could be more severe when it comes to political and other sensitive topics, such as gun control and abortion, which would cause polarization and confirmation bias. The project is aimed to analyze the echo chamber phenomenon on Twitter under three topics: “Abortion”, “Gun” and “Vaccine”. We applied sentiment analysis, network science, and an innovation of using ChatGPT API for stance detection to shed light on the structure of echo chambers and features of influential nodes. Specifically, we explore if the echo chamber phenomenon exists for each topic and whether the influential nodes have more out-degree connections to other communities and the opposing group. Based on our findings, we provided some implications for social media feed algorithm design and governance to weaken the echo chamber effect on social media.

## Description:
Data: data collection(snscrape and twint) and data cleaning notebook files

Stance Detection_ChatGPT: stance detection with ChatGPT3.5 connecting with ChatGPT API, including labeling stance file and validation for GPT3.5 model

Analysis: Detecting Echo Chamber Effects, Network Analysis, and Hypothesis Testing

## Data Source:
Twitter scraping with snscrape(tweets) and twint(user following data)

## Stance Detection:
In the stance detection process, I calculate user's average stance leaning score, representing user's attitude towards abortion. 

In this project: stance leaning score  = stance score * sentiment polarity score

stance score is the classification result given by ChatGPT3.5 model, sentiment polarity score is from VADER sentiment analysis.

## Visualization & Network
Echo Chamber Effect:
![Echo Chamber](echochamber.png?raw=true "Echo Chamber: Individual Leaning VS Following Leaning")

Network:
![Following Network](abortion_net.png?raw=true "User Following Network")

