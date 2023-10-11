# Architechtural Decision Record: Mobile Transportation App

#### Status: Accepted

## Context

The team will develop a Mobile Application using React Native as its UI framework for a transportation company. In the future development of the app, it will be able to track and book rides for users, implement payment system, view driver deteails and ride history. An account authentication will be implemented for added security for both parties. Notifications and announcements will also be incorporated along with the specifics of other use cases.

## Decision

Since React Native can be implemented for cross-platform development, we are proposing the following information in regards to features and backbone of the devlopment:

- Mapbox will be incorporated due to pricing budget. This will also allow the team to fully customize the app based on the client's needs. 

- The team will use server-sent events to track changes and updates in locations real-time.

- Payments will be handled using a payment gateway such as Stripe which provided data encryption and offers various payment methods

- Login security will incorporate a SMS-Bsaed 2FA system as it will be esaier for both users (a driver and passengers) to authenticate their information via mobile phone

- The team will design an appropriate databse schema for ease of use and create a user-friendly experience for all users 

- Notifications such alerts, reminders when the ride is nearby, 

- 

- 

- 

 

 





## Consequences

What becomes easier or more difficult to do because of this change?
