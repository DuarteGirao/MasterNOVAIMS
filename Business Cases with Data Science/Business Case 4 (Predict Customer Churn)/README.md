# Customer-churn-prediction


## 📖 Introduction

In the hotel industry, as in many other travel-related industries, demand is managed through advanced bookings. Bookings (also
known as reservations) are a forward contract between the hotel and the customer that gives the customer the right to use the
service in the future at a settled price, but often with an option to cancel.
The cancellation option puts the risk on hotels who have to honor the bookings that they have on-the-books, but, at the same time, have to support the opportunity costs of having vacant rooms when someone cancels, and there is no time to try to sell the room or sell it at a discounted price. In Europe, the cancellation rate by reservation value, from 2014 to 2018, rose from 33% 
to 40%. <br>

Concerned about the increasingly negative impact caused by cancellations, A, the Revenue Manager Director of hotel chain C, a
chain with resort and city hotels in Portugal, hired a consultant to evaluate the possibility of developing predictive models to predict net demand for their hotels. The hotel provided the consultant datasets of one resort hotel (H1) and of one city hotel (H2), of bookings that were due to arrive between July 1, 2015, and August 31, 2017.
The name of the individual and the company name is anonymized to protect confidentiality. The referenced data are real.
Net demand is defined as demand minus cancellations.

## 📖 Key Problems
    
Within the scope of __Business Cases for Data Science__, C hotel chain operation is not different from other independent and non-independent hotel chains. C hotel chain operation was severally impacted by cancellations, with cancellations, as presented in Table 1, representing almost 28% in H1 and almost 42% in H2. For this reason, A, decided to limit the number of rooms sold with restrictive cancellation policies. To balance that decision, A implemented a more aggressive overbooking policy. However, the latter started to generate costs. To counterbalance those costs, A, soften the overbooking policy, which in turn
was also revealed to be not good. The less aggressive overbooking policy resulted in the hotel having inventory not sold, even on high-demand dates.
    
To reduce the uncertainty about demand, A wanted to implement prediction models to allow the chain’s hotels to forecast net demand based on reservations on-the-books. With these models’ estimations, A expected to implement better pricing and
overbooking policies but also do identify bookings with a high likelihood of canceling. Identifying those bookings could allow the hotels to try to contact those bookings’ customers and make offers to try to prevent cancellation (e.g., dinner, car parking, spa treatments, discounts, or other perks). The goal of A was to reduce cancellations to a rate of 20%.

Cancellations in C hotel chain: <p>


|                | Not Canceled | Canceled    | Total       |
|----------------|-------------:|------------:|------------:|
| Bookings       | 46,228       | 33,102      | 79,330      |
| Room Revenue (€)| 14,394,410   | 10,885,060  | 25,279,470  |


## 📖 Dataset description    
    
The dataset provided for analysis includes information from one resort hotel (H1) and one city hotel (H2), containing bookings scheduled between July 1, 2015, and August 31, 2017. The dataset encompasses various features such as Average Daily Rate (ADR), number of adults and children, booking changes, country of origin, customer type, deposit type, distribution channel, lead time, market segment, meal type, and other relevant factors. This data is provided in the form of an Excel file called 'H2.CSV'.


| Column Name                   | Definition                                                                                         |
|-------------------------------|----------------------------------------------------------------------------------------------------|
| IsCanceled                    | Indicates whether a booking was canceled (0 = not canceled, 1 = canceled)                          |
| LeadTime                      | Number of days between the booking date and arrival date                                           |
| ArrivalDateYear               | Year of arrival                                                                                    |
| ArrivalDateMonth              | Month of arrival                                                                                   |
| ArrivalDateWeekNumber         | Week number of the arrival date                                                                    |
| ArrivalDateDayOfMonth         | Day of the month for the arrival date                                                              |
| StaysInWeekendNights          | Number of weekend nights stayed                                                                    |
| StaysInWeekNights             | Number of weekday nights stayed                                                                    |
| Adults                        | Number of adults included in the booking                                                           |
| Children                      | Number of children included in the booking                                                         |
| Babies                        | Number of babies included in the booking                                                           |
| Meal                          | Type of meal booked                                                                                |
| Country                       | Country of origin of the booking                                                                   |
| MarketSegment                 | Market segment associated with the booking                                                         |
| DistributionChannel           | Distribution channel through which the booking was made                                            |
| IsRepeatedGuest               | Indicates whether the guest is a repeated guest (0 = not repeated, 1 = repeated)                   |
| PreviousCancellations         | Number of previous cancellations made by the customer                                              |
| PreviousBookingsNotCanceled   | Number of previous bookings not canceled by the customer                                           |
| ReservedRoomType              | Room type reserved for the booking                                                                 |
| AssignedRoomType              | Room type assigned to the booking                                                                  |
| BookingChanges                | Number of changes made to the booking                                                              |
| DepositType                   | Type of deposit made for the booking                                                               |
| Agent                         | ID or code of the travel agent associated with the booking                                         |
| Company                       | ID or code of the company associated with the booking                                              |
| DaysInWaitingList             | Number of days the booking was in the waiting list before being confirmed                          |
| CustomerType                  | Type of customer (e.g., transient, contract, group)                                                |
| ADR                           | Average daily rate (price) of the booking                                                          |
| RequiredCarParkingSpaces      | Number of car parking spaces requested by the guest                                                |
| TotalOfSpecialRequests        | Total number of special requests made by the guest                                                 |
| ReservationStatus             | Status of the reservation (e.g., canceled, checked-in, no-show)                                    |
| ReservationStatusDate         | Date of the last status update                                                                     |

<br>

**CustomerType** subcategories:
- **Contract** - when the booking has an allotment or other type of contract associated to it;
- **Group** – when the booking is associated to a group;
- **Transient** – when the booking is not part of a group or contract, and is not associated to other transient booking;
- **Transient-party** – when the booking is transient, but is associated to at least other transient booking

**DepositType** subcategories:
- **No Deposit** – no deposit was made;
- **Non Refund** – a deposit was made in the value of the total stay cost;
- **Refundable** – a deposit was made with a value under the total cost of stay.

**Meal** subcategories:
- **BB** – Bed & Breakfast;
- **HB** – Half board (breakfast and one other meal – usually dinner);
- **FB** – Full board (breakfast, lunch and dinner)
- **Undefined/SC** – no meal package;

**ReservationStatus** subcategories:
- **Canceled** – booking was canceled by the customer;
- **Check-Out** – customer has checked in but already departed;
- **No-Show** – customer did not check-in and did inform the hotel of the reason why


Note: All time-based columns were calculated at the dataset extraction date.
