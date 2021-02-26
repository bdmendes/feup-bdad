Person(*id*,name,adress,telephone)\
Client(*id*->Person.id)\
Worker(*id*->Person.id, specialty->Specialty)\
Specialty(costPerHour)\
Car(*plate*, client->Client, model->CarModel)\
CarModel(*id*,name, brand->CarBrand)\
CarBrand(*name*)
Part(*code*, designation, unitPrice, quantity)
PartOf(*part*->Part, *model*->CarModel)\
UsedPart(*part*->Part, *repair*->Repair, quantity)\
Repair(*id*,startDate,endDate, car->Car)\
RepairWork(*id*,hours, repair->Repair, worker->Worker)\
