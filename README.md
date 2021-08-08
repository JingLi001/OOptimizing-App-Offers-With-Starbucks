# Optimizing-App-Offers-With-Starbucks
## Table of Contents:

1. [Motivation](#motivation)
2. [Installation](#installation)
3. [File description](#file)
4. [Results](#results)
5. [Licensing](#licensing)
6. [Authors](#author)
7. [Acknowledgements](#ack)

## Motivation <a name="motivation"></a>

The motivation of this project is to combine transaction, demographic and offer data to determine which demographic respond best to which offer type and deploy a machine learning model to model customers and personalize marketing plants for much great effectiveness.

## Installation <a name="installation"></a>
* No other installation is needed and The code should run with no issues using Python versions 3. 

## File description <a name="file"></a>

#### profile.json
Rewards program users (17000 users x 5 fields)
- gender: (categorical) M, F, O, or null
- age: (numeric) missing value encoded as 118
- id: (string/hash)
- became_member_on: (date) format YYYYMMDD
- income: (numeric)

### portfolio.json
Offers sent during 30-day test period (10 offers x 6 fields)
- reward: (numeric) money awarded for the amount spent
- channels: (list) web, email, mobile, social
- difficulty: (numeric) money required to be spent to receive reward
- duration: (numeric) time for offer to be open, in days
- offer_type: (string) bogo, discount, informational
- id: (string/hash)

### transcript.json
Event log (306648 events x 4 fields)
- person: (string/hash)
- event: (string) offer received, offer viewed, transaction, offer completed
- value: (dictionary) different values depending on event type
- offer id: (string/hash) not associated with any "transaction"
- amount: (numeric) money spent in "transaction"
- reward: (numeric) money gained from "offer completed"
- time: (numeric) hours after start of test

## Results

I have documented all the findings from the result of this project and wrote a post and published it on Medium.Click [here]
(https://jingli11.medium.com/optimizing-app-offers-with-starbucks-e8a3d76028d4) to take you there.

## Licensing <a name="licensing"></a>

## Authors <a name="author"></a>
Jing Li and Udacity

## Acknowledgements <a name="ack"></a>

Thank you Udacity platform and Starbucks for the data.

