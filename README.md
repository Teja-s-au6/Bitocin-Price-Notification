This is a python script package, bitcoin price notification to get notified for the regular updates of bitcoin price on gmail,telegram,twitter and IFTTT app notifications. The aim is to push notifications when the price of bitcoin changes at certain time interval, user can specify the time interval.By default time interval and threshold are set to 1 minute and $10000 respectively.The user has option to choose out of which of the 4 ways to receive the notifications

![Bitcoin](https://images.unsplash.com/photo-1523759724146-4ce060fff7be?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=675&q=80) 

# Description

Bitcoin price is a fickle thing. You never really know where it's going to be at the end of the day.So, instead constantly checking various sites for the latest updates, let's make a python app to do the work for you

* For this project we are going to use the popular autimation website IFTTT.
* we're going to create required number of applets and choose the service and the app to get the notification like twitter, telegram or SMS and also gmail service.
* Among applets, create the one applet for the emergency notification when the Bitcoin price falls under a certain threshold and the emergency notifications and one for the normal price notifications to the app which the user choose.
* These will be triggered by our python app which will consume the data from the Coinmaretcap.com.
* An IFTTT applet is composed of two parts like trigger and the action.
* Trigger will be webhook service provided by IFTTT.
* Our python app will make an HTTP request to the webhook URL whcih will trigger an action.Now, the action could be almost anything you want. IFTTT offers a multiple actions like sending a notifications or SMS.

## Prerequisite

Must have one of the following app installed and/or must join or follow one of the following accounts

* install the IFTTT App to receive the notifications
* Telegram App and must join this channel.click the [Telegram channel](https://t.me/testbitcoinprice) to join the channel.
* Twitter App and must follow [this account](https://twitter.com/tejaspvg) to receive the notifications.
* An Email account

## Installation

install bitcoin price notifier package using pip

```bash
pip install Bitcoinprice-notifications
```
For Help Menu

```bash
Bitcoin-Price-Notification --help
```

you will see a Response like this

```bash

usage: 
    Usage: This app gives the price of 1 BTC in INR. Destination(-d) must be provided. To recive notification
    from IFTTT install IFTTT mobile app. To recive notifications on Telegram install Telegram app and join this channel 
    https://t.me/testbitcoinprice.  Prerequisite : MUST HAVE A IFTTT APP AND TELEGRAM APP INSTALLED TO RECIVE NOTIFICATION 
    ALSO MUST JOIN THE TELEGRAM Bit_Coin CHANNEL TO RECIVE MESSAGES. PRESS Ctrl+C to terminate the app
    

Bitcoin price Notification

optional arguments:
  -h, --help            show this help message and exit
  -i interval, --interval interval
                        Time interval in minutes
  -t threshold, --threshold threshold
                        Threshold in USD
  -d destnation, --destination destnation
                        We are providing various options to recive
                        notifications from us (1)IFTTT app (2) Telegram app
                        (3) Email (4) Twitter

Copyrights @ Teja S
```
to run the app, type the following command

```bash
Bitcoin-Price-Notification -t 1000 -i 2 -d telegram
```
* -t: threshold amount in USD
* -i: time interval in minutes
* -d: For destionation app like telegram/IFTTT app/email

## AUTHOR: TEJA S

## License
[MIT](https://choosealicense.com/licenses/mit/)