{
"title":"Global Top 100, Google 2023 Solutions Challenge",
"link":"https://github.com/reCloset/reCloset",
"date": "2023-06-01",
"image":"/img/recloset-cover.png",
"description":"Developed a mobile application, ReCloset, using Flutter and Firebase for users to sustainably give away and trade pre-loved clothing. Implemented a trading system and live chat feature to facilitate secure and efficient item exchanges, enhancing user engagement.",
"desciptionImage":"/img/recloset-cover.png",
"tags":[
"Flutter",
"Firebase",
"NodeJS",
"TensorFlow"
],
"featured":true
}

### Description

The Google 2023 Solutions Challenge is a prestigious global hackathon that saw participation from over 2000 teams worldwide. The challenge was aimed at solving one or more of the United Nations' 17 Sustainable Development Goals using Google technology. Our team, ReCloset, was honored to be among the [Global Top 100 winners](https://developers.google.com/community/gdsc-solution-challenge/winners).

### The Problem

The fast fashion industry is a significant contributor to environmental degradation, resource depletion, and unsustainable consumption patterns. We aimed to address these issues by promoting a circular economy and fostering eco-friendly behaviors among consumers.

### Solution

ReCloset is a mobile application developed using Flutter and Firebase. It aligns with the UN's Sustainable Development Goal 12 by encouraging users to exchange pre-loved clothing items, thereby extending the life cycle of garments and reducing waste.

1. **Home Page & Filters:** Users can browse available items and filter them based on various criteria like distance and item name.
2. **User Authentication:** We implemented Google Sign-In for a seamless login experience. New users receive two tokens to kickstart their journey.
3. **Item Details & Chat:** Users can view detailed information about an item, like it, and initiate a chat with the owner.
4. **Trading System:** Users can initiate and confirm trades via the in-app chat, making the transaction process secure and efficient.
5. **QR Code for Physical Meetup:** Users can generate a unique QR code for physical exchanges.
6. **Content Management:** Our TensorFlow model screens uploaded items for explicit content, ensuring a safe user experience.
7. **Achievement System:** Gamification elements like achievements for the number of items given away or the amount of water saved.
8. **Educational Aspect:** Post-transaction screens educate users on their positive environmental impact.

I was responsible for implementing the **Trading System** . This feature was crucial for facilitating secure and efficient item exchanges, thereby enhancing user engagement. I used Firebase Firestore for the backend and integrated it with Google Cloud Functions to handle secure write operations during the trading process.

### Product Demonstration

{{< youtube X6tU68o3URM >}}
