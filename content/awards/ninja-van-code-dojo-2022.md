{
"title":"4th Place, Ninja Van Code Dojo Hackathon 2022",
"link":"https://devpost.com/software/ratings",
"date": "2022-02-01",
"image":"/img/code-dojo-2022.png",
"description":"Collaborated in a team of 4 and created a Telegram bot, “Ninja Scheduler” in 36 hours, enabling customers to upgrade delivery tiers and reschedule deliveries to reduce failed deliveries when customer not available, with payments made via Stripe (utlising Telegram Payments API)",
"desciptionImage":"/img/code-dojo-2022.png",
"tags":[
"Python",
"Cloud Firestore",
"Heroku"
],
"featured":false
}

### Description

Code Dojo was a 36 hour Hackathon where my team of 4 worked to innovate and prototype ideas that can improve logistics and Ninja Van's operations and service quality. Ninja Van is a leading courier company in Singapore and across Southeast Asia, with more than 67,000 staff and delivery personnel and handles around 2 million parcels a day across Southeast Asia.

### Solution

Ninja Scheduler is the bot designed for busy people who are unavailable to receive their package on the actual delivery day. This bot is targeted at customers who might be unavailable to receive the package on the stipulated delivery date, and might want to reschedule the delivery. It is also designed for users who are willing to pay more to get faster deliveries, but are unable to do so as online retailers often only offer the cheapest (and thus slowest) delivery option.

To solve this issue, our bot automates the handling of rescheduling deliveries. Customers can view the delivery dates of their orders, and based on their tier of delivery service for a particular order, they can upgrade to a different tier, to schedule it earlier or later based on their availability. They can even upgrade to the timeslot delivery scheme, which allows them to choose from 4 different timeslots to get their package delivered. If they are unavailable to receive the package during the week of delivery, they can opt for the 14 day standard or timeslot delivery tiers. The bot handles the upgrade by issuing invoices through Telegram, and once paid they can proceed to reschedule according to their tiers! However, each customer is limited to 2 free reschedules. Once they have hit that limit, they can "top-up" their number of reschedules through the bot.

By providing 5 different upgradable delivery tiers (Standard, Express, Timeslot, 14 day Standard, 14 day Timeslot) and easy rescheduling, we are confident customers will have better experience with Ninjavan, tailored to their needs.
