# travelweatherplanner
un dispositif de voyage
# Variables
distance_mi = 3          # nombre (tu peux changer pour tester)
is_raining = False       # booléen
has_bike = True          # booléen
has_car = False          # booléen
has_ride_share_app = False  # booléen

# Logique de décision
if not distance_mi:  # distance_mi est falsy (0, None, etc.)
    print(False)

elif distance_mi <= 1:
    # True seulement si pas de pluie
    print(not is_raining)

elif distance_mi <= 6:
    # True seulement si vélo ET pas de pluie
    print(has_bike and not is_raining)

else:
    # distance > 6 miles
    print(has_car or has_ride_share_app)
