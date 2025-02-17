# Test Plan

## Table of Contents
1. [Overall Test Plan](#overall-test-plan)
2. [Test Case Descriptions](#test-case-descriptions)
    * [PlantParenthood.API](#plantparenthood.api)
    * [PlantParenthood.Android](#plantparenthood.android)
    * [PlantParenthood.Pi](#plantparenthood.pi)
3. [Test Case Matrix](#test-case-matrix)

## Overall Test Plan

Plant Parenthood will utilize testing that ensures basic functionality of the core services it provides. Due to the nature of the application, our user-facing activities are easily tested - we did our best to stray away from complicated interactions for the sake of simplicitity and maintenance.

Therefore, our testing will significantly focus on the successful interactions between services. These are essential to the application's functionality - if the API is unsuccessful in communicating information between the Android client and Raspberry Pi hub then the implementation we have provided will not function. It is dependant on the ability to quickly and effectively receive real time data from the various sensors we have installed to the plant.

***

## Test Case Descriptions

### PlantParenthood.API
***
#### Test Case API.I

    Purpose: 
        Test interaction with gRPC server on Pi hub.

    Description: 
        Verify that sending a PlantFactorRequest from our test gRPC client returns current plant factors for installed Pi.

    Inputs: 
        PlantFactorRequest of type 'all'.

    Expected Result:
        PlantFactorReply containing reasonable Temperature, Air Pressure, Humidity, Light Exposure, and Soil Moisture.
    
    Normal / Abnormal / Boundary:
        
        Normal

    Blackbox / Whitebox:
        
        Whitebox

    Functional / Performance:

        Functional

    Unit / Integration:
        
        Integration

        

#### Test Case API.II

    Purpose: 
        Test notification service implementation with Android client.
    
    Description: 
        Send PlantAnalysis() results to the API that signify the need for a notification to be sent to the user.

    Inputs: 
        PlantAnalysis() result with 2 or more constraint violations.

    Expected Result:
        A notification should be sent to the user prompting them to view the related plant.
    
    Normal / Abnormal / Boundary:
        
        Normal

    Blackbox / Whitebox:
        
        Whitebox

    Functional / Performance:

        Functional

    Unit / Integration:
        
        Integration

#### Test Case API.III

    Purpose: 
        Test interaction with DB, saving Plant Data.
    
    Description: 
        Send mock PlantFactorReply from test gRPC client, to verify that values are stored in the DB.

    Inputs: 
        PlantFactorReply with valid Temperature, Soil Moisture, Air Pressure, Light Exposure, and Humidity.

    Expected Result:
        PlantFactorID should be returned that verifies the newly saved record.
    
    Normal / Abnormal / Boundary:
        
        Normal

    Blackbox / Whitebox:
        
        Whitebox

    Functional / Performance:

        Functional

    Unit / Integration:
        
        Integration


### PlantParenthood.Android
***
#### Test Case And.I

    Purpose: 
        Test interaction with API through gRPC.

    Description: 
        Send PlantFactorRequest to the API through Android client, verifying the ability to send requests and to receive data upon retrieval of the PlantFactorReply.

    Inputs: 
        Upon entering PlantOverview component from the PlantList, a PlantFactorRequest will be sent to retrieve current data.

    Expected Result:
        It is expected to receive a valid PlantFactorReply with reasonable ranges for each factor (Temperature, Soil Moisture, Light Exposure, Air Pressure, Humidity),
    
    Normal / Abnormal / Boundary:
        
        Normal

    Blackbox / Whitebox:
        
        Whitebox

    Functional / Performance:

        Functional

    Unit / Integration:
        
        Integration

#### Test Case And.II

    Purpose: 
        Test User Token generation & authentication.
    
    Description: 
        Upon logging in, a user token should be generated that is then used on subsequent login attempts to automatically bring the user to their plant list. This verifies the generation and use of the token.

    Inputs: 
        Send usp_Login request with a test username & password, and upon successfully receiving a token send a subsequent request to usp_Login with the token rather than the username / password.

    Expected Result:
        In both instances, usp_Login should return relevant user data if successful.
    
    Normal / Abnormal / Boundary:
        
        Normal

    Blackbox / Whitebox:
        
        Whitebox

    Functional / Performance:

        Functional

    Unit / Integration:
        
        Unit

#### Test Case And.III

    Purpose: 
        Test ability to add a plant to the PlantList.
    
    Description: 
        Verify that sending a CreatePlant request to the API will return a new plant associated with the user that triggered the action.

    Inputs: 
        A valid CreatePlant request containing the new plant's nickname and type.

    Expected Result:
        A CreatePlant reply should be returned containing the newly created Plant's ID.
    
    Normal / Abnormal / Boundary:
        
        Normal

    Blackbox / Whitebox:
        
        Whitebox

    Functional / Performance:

        Functional

    Unit / Integration:
        
        Unit


### PlantParenthood.Pi
***
#### Test Case Pi.I

    Purpose: 
        Test gRPC client automated logging.

    Description: 
        Plant Factors are sent to the DB every 10 minutes from the gRPC client on the Raspberry Pi - this test verifies after 10 minutes that new Plant Factors are present.

    Inputs: 
        A request is sent to the DB to retrieve the last logged PlantFactors, wait 10 minutes, and then checks again to compare.

    Expected Result:
        It is expected that the two sets of PlantFactors retrieved will have differing PlantFactorIDs.
    
    Normal / Abnormal / Boundary:
        
        Normal

    Blackbox / Whitebox:
        
        Whitebox

    Functional / Performance:

        Functional

    Unit / Integration:
        
        Integration

#### Test Case Pi.II

    Purpose: 
        Test interaction with attached sensors.
    
    Description: 
        Run the Plant Factor retrieval script to ensure that each sensor returns data within acceptable ranges, ensuring that each sensor is working appropriately.

    Inputs: 
        Run PlantParenthood.py and evaluate the retrieved data, if any.

    Expected Result:
        Each sensor should return data within pre-defined 'reasonable' constraints.
    
    Normal / Abnormal / Boundary:
        
        Normal

    Blackbox / Whitebox:
        
        Whitebox

    Functional / Performance:

        Functional

    Unit / Integration:
        
        Unit

#### Test Case Pi.III

    Purpose: 
        Test interaction with API as gRPC server.
    
    Description: 
        Retrieve current Plant Factors from PlantParenthood.py and send them to the API, saving them and returning the relevant PlantFactorID.

    Inputs: 
        Run PlantParenthood.py, and attempt to send the retrieved Plant Factors to the API.

    Expected Result:
        PlantFactorID should be returned that verifies the newly saved record.
    
    Normal / Abnormal / Boundary:
        
        Normal

    Blackbox / Whitebox:
        
        Whitebox

    Functional / Performance:

        Functional

    Unit / Integration:
        
        Integration

*** 

## Test Case Matrix

| Test Case   | Purpose | Normal / Abnormal | Blackbox / Whitebox | Functional / Performance | Unit / Integration |
|-------------|:--------|:-----------------:|:-------------------:|:------------------------:|:------------------:|
| **API**.I   | Test interaction with gRPC server on Pi hub. | Normal | Whitebox | Functional | Integration |
| **API**.II  | Test notification service implementation with Android client. | Normal | Whitebox | Functional | Integration |
| **API**.III | Test interaction with DB, saving Plant Data. | Normal | Whitebox | Functional | Integration |
| **And**.I   | Test interaction with API through gRPC. | Normal | Whitebox | Functional | Integration |
| **And**.II  | Test User Token generation & authentication. | Normal | Whitebox | Functional | Unit |
| **And**.III | Test ability to add a plant to the PlantList. | Normal | Whitebox | Functional | Unit |
| **Pi**.I    | Test gRPC client automated logging. | Normal | Whitebox | Functional | Integration |
| **Pi**.II   | Test interaction with attached sensors. | Normal | Whitebox | Functional | Unit |
| **Pi**.III  | Test interaction with API as gRPC server. | Normal | Whitebox | Functional | Integration |

***