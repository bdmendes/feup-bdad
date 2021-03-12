Gardener(*id*,name)\
Client(name, *taxID*, city->City)\
Services(*nameGardener*->Gardener, *nameClient*->Client)\
Garden(name,*adress*,city->City)\
GardenResponsability(*clientName*->Client,*gardenName*->Garden, ownsGarden)\
Plant(area, name, *cientificName*)\
Plantation(*nameGarden*->Garden, *plantName*->Plant, numberOfPlants)
PlantPlague(*name*, *plant*->Plant)\
Season(*id*,startDate,endDate)\
PlagueTreatment(*id*)\
PlagueSeasonTreatment(*plague*->PlantPlague, *season*->Season, *treatment*->PlagueTreatment)