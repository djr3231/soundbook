# user story:

A large sound reinforcement company employs dozens of live sound technicians.
A client calls the main office, where a secretary creates an order containing the following details:
Event date
Event time
Scale/attendance (e.g., 400–500 or 50–100 people)
Contact person
Indoor or outdoor venue
Important notes and highlights.

The secretary enters this into a specialized system, and the assigned technician receives a notification about the event.
This is where our system comes in: based on the order details and a conversation with the client, the technician needs to determine what equipment and assistants are required for the event.
He logs into the system and places the order.
The system functions much like a standard modern online ordering site—minus the payment step; once logged in as an authenticated user, he can place the order.
In a real-world scenario, I would expect the warehouse manager to give final approval for the order, with the technician receiving a notification of this status. However, I wouldn't build that feature at this stage; for our purposes, the order is considered submitted as soon as he clicks "Order."
Upon logging in, the first thing he should see is a display of popular products or items from his favorites list.
This should feature a modern interface for selecting products by category, complete with advanced filtering and search capabilities. I would like to see complete kits available for order—perhaps in a separate category—rather than having to assemble items individually.
Once the user has gathered all the necessary products in their cart, they can proceed to place the order.
At the next stage, they will need to select whether additional assistants (assistant technicians) are required. If they opt for extra help, a general request indicating the need for assistants will be sent to the main office (the entity that issued the original order). The office will then dispatch available personnel—such as junior technicians or technician assistants—for the scheduled time.
Subsequently, the user will need to coordinate delivery. Since the setup time depends on the event schedule, they will specify when the equipment needs to be on-site. This information will be transmitted to the office as a transport request, making it the office's responsibility to coordinate logistics with their transport team.
These notifications to the office—regarding both transport and assistants—can be configured to be sent either via email or to a dedicated system endpoint designed to simply receive the request and return a positive response.
A technician may have multiple orders scheduled for different dates.

The actual order date is the scheduled transport date. To place an order without delivery, the user would need to select a specific option; this applies to cases involving small equipment that the customer can pick up personally from the company's warehouse using their own vehicle. In any case, they need to specify the date and time of pickup. We could handle this—if we adapt the system for online ordering—by setting the shipping method to "self-pickup." However, I don't want to commit to that specific interface just yet, because sites of this type usually offer a choice of shipping methods, whereas here it’s an either-or scenario.

I would also like to see an order calendar view where orders are displayed chronologically; this could even serve as the main screen for order management.

Naturally, it should also be possible to edit or cancel an order.
