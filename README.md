# from HL7v2 to FHIR SQL Builder

Ready to use demo of an FHIR Server with :
* HL7v2 transformation to the FHIR Server 
* FHIR Server who can be query in SQL

![alt text](https://raw.githubusercontent.com/grongierisc/FHIR-HL7v2-SQL-Demo/master/fhirhl7ui/app/src/assets/img/FHIRdemo.jpg)

### Installing

Clone this repository

```
git clone https://github.com/grongierisc/FHIR-HL7v2-SQL-Demo.git
```

Docker

```
docker-compose up --build -d
```

### Usage

* Can use postman config in misc/fhirhl7v2demo.postman_collection.json

* Use UX at http://localhost:4201

* ***Login/Password*** : _SYSTEM/SYS

### How-To use the demo

![alt text](https://raw.githubusercontent.com/grongierisc/FHIR-HL7v2-SQL-Demo/master/misc/FHIRDemoTuto.png)

3 steps to use it :

## Import FHIR resources from VSCode using FHIR.API.http

1. edit the file [FHIR.API.http](./FHIR.API.http)
2. click on "Send Request" under ### labels 


## Import FHIR resources using POSTMAN

1. import into [Postman](https://www.postman.com/) the file ./misc/from HL7v2 to FHIR SQL Builder.postman_collection.json 
2. send the 3 POST containing Driver License (DL)


## Import HL7v2 Messages

Click on the left arrow between IRIS and the ambulance.

This windows open :

![alt text](https://raw.githubusercontent.com/grongierisc/FHIR-HL7v2-SQL-Demo/master/misc/HL7v2Import.png)

From here you can import samples from this directory in the Git repo :

sampleFiles

Select one and click send.

![alt text](https://raw.githubusercontent.com/grongierisc/FHIR-HL7v2-SQL-Demo/master/misc/HL7v2Send.png)

From here you can click on Message Trace :

![alt text](https://raw.githubusercontent.com/grongierisc/FHIR-HL7v2-SQL-Demo/master/misc/MessageList.png)

Select the first one :

![alt text](https://raw.githubusercontent.com/grongierisc/FHIR-HL7v2-SQL-Demo/master/misc/MessageTrace.png)

Here you can see the ready made transforamtion between HL7v2 to SDA to FHIR.

## Use the FHIR Client

Click on arrow between IRIS and FHIR Client :

![alt text](https://raw.githubusercontent.com/grongierisc/FHIR-HL7v2-SQL-Demo/master/misc/FhirClient.png)

The small swagger give you the opportunity to query in FHIR the populated repo from HL7v2 message or from the FHIR Client.

Example : 

![alt text](https://raw.githubusercontent.com/grongierisc/FHIR-HL7v2-SQL-Demo/master/misc/FHIRGetAllPatient.png)

## Use the SQL Client

Click on arrow between IRIS and SQL Client :

![alt text](https://raw.githubusercontent.com/grongierisc/FHIR-HL7v2-SQL-Demo/master/misc/FHIRSQL.png)

From here you can see all the FHIR ressources in an SQL relational way.

## Special Thanks

* https://github.com/limelissa for the UI
* https://github.com/grongierisc/FHIR-HL7v2-SQL-Demo for the initial project


