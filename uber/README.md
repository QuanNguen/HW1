Uber
1. Which SOLID principle(s) is this company violating?
- In the Uber company, two SOLID principles this company violates are Single Responsibility Principle and Open-Closed Principle.
- In the ‘RideManager’ class, it has to do two jobs, one is calculating the ride fare and another job is sending notifications. It violates SRP
- If I want to add a new method for calculating ride fares in the ‘RideManager’ class for example I want to calculate discount fare for my ride, I need to add new method and if I want to add more new type of calculation, I need to add new method again so it not reusable. It violates OCP. 
2. Your approach to making changes to fix the violation.
- Create three new classes ( ‘FareCalculator’, ‘DiscountFareCalculator’, and ‘NotificationService’) to handle different jobs. 
- Make two interface names ‘Calculator’ and ‘Notifier’. ‘FareCalculator’ and ‘DiscountFareCalculator’ classes that implement ‘Calculator’ interface, and ‘NotificationService’ class that implements ‘Notifier’ interface. 
