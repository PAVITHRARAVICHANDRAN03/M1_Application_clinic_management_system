## TEST PLAN:
## Table 1: High level test plan
|Test ID|Description|Exp I/P|Exp O/P|Actual Out|Type Of Test|
|:-----------|:----------|:---------|:----------|:---------|:-------|
|H_01|Select mode|Admin mode enter Password - 1234|if you want to add new patient record press 1 ,if you want to edit patient record press 2,if you want to reserve a slot with the docto 3,if you want to cancel reservation press 4|if you want to add new patient record press 1 ,if you want to edit patient record press 2,if you want to reserve a slot with the docto 3,if you want to cancel reservation press 4|Requirement based|
|H-02|Select mode|Admin mode Password - 1234|Please Enter the patient's name:raj,Please Enter the patient's age: 35 ,Please Enter the patient's gender (male or female): male, Please Enter the patient's id:4354|Please Enter the patient's name:raj ,Please Enter the patient's age: 35 ,Please Enter the patient's gender (male or female): male,Please Enter the patient's id:4354|Scenario based|
|H-03|Select mode|user mode|For Patient record press 1,For today's reservation press 2|Patient Record ,Today's Reservation,Invalid Choice please try again|Scenario based|
|H-03|In admin mode the entered password was incorrect for 3 consecutive times,the system shall close. |password - 64545|Incorrect password for 3 consecutive times|Incorrect password for 3 consecutive times|Boundary based|

## Table 2: Low level test plan
|Test ID|Description|Exp I/P|Exp O/P|Actual Out|Type Of Test|
|:-----------|:----------|:---------|:----------|:---------|:-------|
|L_01|Enter 1 for admin mode|1|Admin mode|Admin mode|Requirement based|
|L-03|Enter 2 for user mode |2 |user mode|user mode|Requirement based|
|L-03|Edit patient record(its exists)|Entering ID-4354|edit name:R.raj,edit gender:male,edit age:43|edit name:R.raj,edit gender:male,edit age:43|Scenario based|
|L-04|Edit patient record|Entering ID-4355|incorrect ID|incorrect ID|Scenario based|
|L-04|Enter Your ID its wrong|Enter Your ID:3567|Invalid Choice please try again|Invalid Choice please try again|Boundary based|

