Car(*serialNumber*, weight, horsePower, maxSpeed, CarBrand->CarBrand)\
CarBrand(*name*, points, Country->Country)\
Pilot(*name*,adress,birthYear,points,Car->Car,Country->Country)\
Circuit(*name*,local,length,Country->Country)\
Season(*year*)\
Race(*id*, numberOfLaps, Circuit->Circuit, Season->Season)\
Participation(*name*->Pilot, *id*->Race, startPos, endPos)\
RaceQuit(*name*->Pilot, *id*->Race, reason, lap)