# Drone-Delivery-Problem-datasets-and-related-parameters


There are THREE datasets 


(1) Drone 1 to 4 (D4) with their parameters and 

(2) Drone 1 to 10 (D10) with their parameters

    *Units: g = gram, km = kilometre, min = minutes, m/s = meter per second*

    Drone = drone ID or NUMBER

    Payload = limitation weight in gram which is allowed per drone to carry for flight

    Speed = the speed that the corresponded drone is allowed to fly

    Coverage Distance = the distance in kilometer measured from the center/depot/warehouse place and the corresponded drone is allowed to fly within that distance 

    Flight Time = the corresponded drone's flight time in minutes related to the speed and their respective battery capacity



(3) Location 1 to 100 (L1toL100) with their parameters

      *Units: km = kilometre*
      
      Location = location ID or NAME
      
      Latitude = location's latitude
      
      Longitude = location's longitude
      
      Item = delivery item to be carried by Drone
      
      Quattity = item's quantity
    
      Distance from the warehouse = the distance in kilometer from the warehouse to the respecive location
      
 Warehouse location: 37.60074273, 126.86482072, using Haversine formula to calculate the distance between two latitude/longitude points.
 
 Item 1, 2, 3 and 4 are 100, 200, 300, 400 grams in weight respectively.
 
 Location latitude and longitude values are generated by the program as follow:
 
 Firstly, a random distance from the warehouse and a random bearing point (0 to 360 degree) are generated
 
 Secondly, generate the end point (latitude,longitude) from the given random distance,bearing point and warehouse location point (latitude,longitude)
 
 # Results
 
 (4) Result-chromosomes-in-all-generation.csv
 
      The results outcome after we solved 100 locations- 10 Drones rounting assignment (drone-based delivery).
      
      Algorithm runs with 20 intializations, 6 elitisms for 10 generations.
      
       We apply Genetic algorithm with our heuristic fitness function (concurrent-heuristic approach) with our proposed operator 
       (gene-elitism crossover and gene-replacement mutation)
      
      The optimal assignment result at 10th generation with concurrent-time value 1478.89.
      
 (5) Result-routing-assignment.csv

      The detail routing assignment for the optimal result 1478.89.
      
      The assignment shows the result by describing a specific drone should fly to a location as a priority together with its knapsack assigned items.
