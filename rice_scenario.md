# Scenario 13 - Exchange of Paddy Field Operation Data

## 13.0 Overview
 To achieve resilient and sustainable rice production, rice smart farming technologies were introduced, and their effects have been demonstrated  in Thailand. When the ADAPT Standard was used to exchange work orders and work reports between farmers and farm contractors, the accuracy of these work orders and reports improved. Furthermore, the exchange of operation trajectory data enabled the development of a data-driven payment service and enhanced  remuneration transparency through a task-based payment system.
 
## 13.1 Business Workflow (Sequence)

 <object type="image/svg+xml" data="/scenarios/scenario-013-01.svg"></object>

 ## 13.2 Example
 ### Work Orders
 [Work orders of harvest](/docs/examples/Scenario13/adapt.json)

 ### Work Reports
 [Work reports of harvest](/docs/examples/Scenario13/adapt.json)

## [Explanation of the rice_scenario]
- Images in Section "13.0 Overview" will be created using rice_scenario.plantUML
  The "rice_scenario.plantUML" can be visualized at the following URL:
  https://www.plantuml.com/plantuml/
- In Section "13.2 Example", sample data will be uploaded. 
- "OperationTypeEnum" for rice cultivation will be added in the bottom of the page.

### rice_scenario.plantUML
  @startuml scenario-013-01
'categories = Data Types - Field Operation
title Yield and Work trajectory Data

entity "Farm Management\nSoftware\n(Farmers)" as 0
entity "Farm Equipment\nSoftware\n(Farm Contractors)" as 1

0 ->> 1: [[/docs/work-record Work Orders]]
1 ->> 0: [[/docs/work-order Work Records]]& [[Trajectory]]  

@enduml

