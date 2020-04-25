# Test Plan

## Table of Contents
1. [Overview](#overview)
2. [Test Case Descriptions](#test-case-descriptions)
    * [PlantParenthood.API](#plantparenthood.api)
    * [PlantParenthood.Android](#plantparenthood.android)
    * [PlantParenthood.Pi](#plantparenthood.pi)
3. [Test Case Matrix](#test-case-matrix)

## Overview

Plant Parenthood will utilize testing that ensures basic functionality of the core services it provides. Due to the nature of the application, our user-facing activities are easily tested - we did our best to stray away from complicated interactions for the sake of simplicitity and maintenance.

Therefore, our testing will significantly focus on the successful interactions between services. These are essential to the application's functionality - if the API is unsuccessful in communicating information between the Android client and Raspberry Pi hub then the implementation we have provided will not function. It is dependant on the ability to quickly and effectively receive real time data from the various sensors we have installed to the plant.

***

## Test Case Descriptions

### PlantParenthood.API
***
#### Test Case API.I

    Purpose: Test interaction with gRPC server on Pi hub.

    Description: 

    Inputs:

    Expected Result:

    Functional Indication:

#### Test Case API.II

    Purpose: Test notification service implementation with Android client.
    
    Description:

    Inputs:

    Expected Result:

    Functional Indication:

#### Test Case API.III

    Purpose: Test interaction with DB, saving Plant Data.
    
    Description:

    Inputs:

    Expected Result:

    Functional Indication:


### PlantParenthood.Android
***
#### Test Case And.I

    Purpose: Test interaction with API through gRPC.

    Description:

    Inputs:

    Expected Result:

    Functional Indication:

#### Test Case And.II

    Purpose: Test User Token generation & authentication.
    
    Description:

    Inputs:

    Expected Result:

    Functional Indication:

#### Test Case And.III

    Purpose: Test ability to retrieve current Plant Factors from API.
    
    Description:

    Inputs:

    Expected Result:

    Functional Indication:


### PlantParenthood.Pi
***
#### Test Case Pi.I

    Purpose: Test gRPC client functionality & interaction with API.

    Description:

    Inputs:

    Expected Result:

    Functional Indication:

#### Test Case Pi.II

    Purpose: Test interaction with attached sensors.
    
    Description:

    Inputs:

    Expected Result:

    Functional Indication:

#### Test Case Pi.III

    Purpose: Test interaction with API as gRPC server.
    
    Description:

    Inputs:

    Expected Result:

    Functional Indication:

*** 

## Test Case Matrix

| Test Case   | Purpose | Normal / Abnormal | Blackbox / Whitebox | Functional / Performance | Unit / Integration |
|-------------|---------|-------------------|---------------------|--------------------------|--------------------|
| **API**.I   |         |                   |                     |                          |                    |
| **API**.II  |         |                   |                     |                          |                    |
| **API**.III |         |                   |                     |                          |                    |
| **And**.I   |         |                   |                     |                          |                    |
| **And**.II  |         |                   |                     |                          |                    |
| **And**.III |         |                   |                     |                          |                    |
| **Pi**.I    |         |                   |                     |                          |                    |
| **Pi**.II   |         |                   |                     |                          |                    |
| **Pi**.III  |         |                   |                     |                          |                    |

***