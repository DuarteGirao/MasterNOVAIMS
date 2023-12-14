# MastersNovaIMS-BCWDS-BC1-Customer_Segmentation

## 📖 Introduction
    
Within the scope of __Business Cases for Data Science__, it was proposed a project, where the groups' ability to deliver a customer segmentation in accordance with the different features included in a dataset containing 111.733 records would be tested. However, A, the new marketing manager of the hotel H, realized that the current customer segmentation was not useful for the hotel marketing department, as it only reflected one only customer characteristic, its sales origin.
    
Therefore, the business goal determined for this project was to develop a new customer segmentation and gaining insight on the current customers' characteristics. By understanding the differences between the different segments, organizations can make better strategic choices about opportunities, product definition, positioning, promotions, pricing, and target marketing.

<br>

## 📖Dataset description

This notebook uses the Case1_HotelCustomerSegmentation.csv. The Dataset is related with direct marketing campaigns of a hotel located in Lisbon, hotel H.<br> This hotel H is inserted in a hotel chain C, spread all over the world. <br> Since 2018, there is a new marketing manager in this hotel H, A, which is somehow unsatisfied with hotel H marketing department.


Client information:
- **ID**: Customer ID
- **Nationality**: Nationality of the customer in ISO 3166-1 (Alpha 3) format
- **Age**: Age of the customer
- **DaysSinceCreation**: Number of elapsed days since the customer was created
- **NameHash**: Hash of the customer name
- **DocIDHash**: Hash of the customer personal document identification number (usually passport or ID card)
- **AverageLeadTime**: Average number of days before arrival date the customer makes bookings
- **LodgingRevenue**: Total amount of lodging revenue paid by the customer so far
- **OtherRevenue**: Total amount of other revenue (e.g., food & beverage, spa, etc.) paid by the customer so far

Reservation information:
- **BookingsCanceled**: Number of bookings the customer made but ubsequently canceled
- **BookingsNoShowed**: Number of bookings the customer made but subsequently made a "no-show"
- **BookingsCheckedin**: Number of bookings the customer made, which actually ended up staying
- **PersonNights**: Total person/nights the customer has stayed at the hotel so far.
- **RoomNights**: Total of room/nights the customer has stayed at the hotel so far.
- **DistributionChannel**: Distribution channel normally used by the customer to make bookings at the hotel
- **MarketSegment**: Current market segment of the customer
- **SRHighFloor**: Indication if the customer usually asks for a room in a higher floor (0: No, 1: Yes)
- **SRLowFloor**: Indication if the customer usually asks for a room in a lower floor (0: No, 1: Yes)
- **SRAccessibleRoom**: Indication if the customer usually asks for an accessible room (0: No, 1: Yes)
- **SRMediumFloor**: Indication if the customer usually asks for a room in a middle floor (0: No, 1: Yes)
- **SRBathtub**: Indication if the customer usually asks for a room with a bathtub (0: No, 1: Yes)
- **SRShower**: Indication if the customer usually asks for a room with a shower (0: No, 1: Yes)
- **SRCrib**: Indication if the customer usually asks for a crib (0: No, 1: Yes)
- **SRKingSizeBed**: Indication if the customer usually asks for a room with a king size bed (0: No, 1: Yes)
- **SRTwinBed**: Indication if the customer usually asks for a room with a twin bed (0: No, 1: Yes)
- **SRNearElevator**: Indication if the customer usually asks for a room near the elevator (0: No, 1: Yes)
- **SRAwayFromElevator**: Indication if the customer usually asks for a room away from the elevator (0: No, 1: Yes)
- **SRNoAlcoholInMiniBar**: Indication if the customer usually asks for a room with no alcohol in the mini bar (0: No, 1: Yes)
- **SRQuietRoom**: Indication if the customer usually asks for a room away from the noise (0: No, 1: Yes)


Note: All time-based columns (e.g., Age or DaysSinceCreation) were calculated at the dataset extraction date.
