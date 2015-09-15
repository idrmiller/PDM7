##USER STORIES

Here are a few examples of user stories as if you are a trying to hail an Uber. For this example, I am using the iOS version of their app and am already a registered and authenticated user.

###Geolocate User
As an authenticated iOS user that has not requested a ride, when I open the app I would like to see my location pinned on the map and Pickup Location pre-populated so that I can easily request a ride.

**Acceptance Criteria**
 1. If geolocation is available, place pin on map at users location.
 2. If geolocation is available, auto-populate address into "Pick Up" location
 3. If geolocation is unavailable, Pickup Location should have hint text "Enter Pickup Location"

##Enter pickup location
As an authenticated iOS user that has not requested a ride, I would like to be able to specify my exact location so a driver can accurately pick me up.

**Acceptance Criteria**
 1. User can enter address into Pickup Location field.
 2. Address requires Street Address, City, and State.
 3. Address can optionally include zipcode in lieu of city and state.
 4. User can enter Business Name in lieu of address.
 5. User can move location of pin on map and see updated address in Pickup Location.

###See Estimated Pickup TIme
As an authenticated iOS user that has not requested a ride, I want to see an estimated wait time so I can determine whether or not I want to wait for an Uber.

**Acceptance Criteria**
 1. Time should be displayed in minutes.
 2. Time should be based on coordinates of closest driver.
 3. Estimate should refresh every 15 seconds.
 4. If estimate is greater than 20 minutes, say "BUSY"

###Select Service
As an authenticated iOS user that has not requested a ride, I want to be able to toggle between available Uber services so I can select my preferred means of travel.

**Acceptance Criteria**
 1. Only show available service based on the users current, geolocated market.
 2. Market-enabled services that are not operating at the current time should be ghosted out and unselectable by the user.
 3. When the user selects a new service, the Map View and Estimated Time should refresh.

###See Drivera on Map
As an authenticated iOS user that has not requested a ride, I want to see nearby cars on the map so I can better understand and track the location of drivers.

**Acceptance Criteria**
 1. Show up to 5 closest drivers on map.
 2. Refresh location of cars every 2 seconds.
 3. Unavailable drivers should not be displayed on map.

###Request Ride
As an authenticated iOS user that has not requested a ride, when I click the "Request Ride" button, I want to confirm my information so I can ensure my accurate information is used.

**Acceptance Criteria**:
 1. On click of request button, user should be directed to Confirmation Page.
 2. User should be displayed location and payment information.
 3. On click of "Confirm" button, request should be relayed to 5 closest drivers.

