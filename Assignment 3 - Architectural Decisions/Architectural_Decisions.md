By Edward Montilla & Japsimran Kaur Nanda (from Peaky Coders)

# Architechtural Decision Record: Mobile Transportation App

#### Status: Accepted

## Context

The team will develop a Mobile Application using React Native as its UI framework for a transportation company. In the future development of the app, it will be able to track and book rides for users, implement payment system, view driver deteails and ride history. An account authentication will be implemented for added security for both parties. Notifications and announcements will also be incorporated along with the specifics of other use cases.

## Decision

Since React Native can be implemented for cross-platform development, we have decided to use the following systems to reinforce the foundation of the development:

- Mapbox will be incorporated due to pricing budget and tracking capabilities. This will also allow the team to fully customize the app based on the client's needs. 

- The team will use server-sent events to track changes and updates in locations real-time.

- Payments will be handled using a payment gateway such as Stripe which provides data encryption and offers various payment methods

- Login security will incorporate a SMS-Bsaed 2FA system as it will be easier for both users (a driver and passengers) to authenticate their information via mobile phone while providing a robust security means

- The team will design an appropriate databse schema for ease of use and create a user-friendly experience for all users 

- Push notification such alerts confirmations, reminders when the ride is nearby, updates from the ride/driver and messaging between the driver and passenger and other features will use Pushwoosh and will integrate its system to the mobile app due to the ability to send message, images and videos files along with the ability to supprot multiple platforms

- To best protect the user's data and sensitive information, we are considering a few security system services as part of the development. As of this moment, we are looking at Google's Apigee as an implementation due to being developer=friendly


## Consequences

The process will be taxing and things may not go according to plan so we are being wary of the following:

- The learning curve for the implementations will depend on how the team is able to handle existing and potential obstacles 
  
- Making sure that everything can be implemented properly with React Native as the backbone

- Lacking knowledge in security and loop holes that could leak sensitive data due to poor implementation and reserach

- Schedule is subject to change due to unknown factors in the development phase

- Lacking in manpower

With the proposed ideas given, the goal of creating a robust and practical mobile application using the requirements mentioned will prove to be our most challenging project yet. The end result will provide a convenient way to manage transportation rides while giving the user the transparency of the app's concept.
