# VDI2206 Ontology-Design-Pattern

## Introduction
The development of software functionalities, or applications in general, that monitor and analyze manufacturing-related data in order to improve, support or automate processes, is becoming increasingly important in industry. These applications require several information from different data sources in their context. An application that is planning a maintenance workers daily schedule for instance, requires several information about machine statuses, production plans and inventory, which resides in different systems likes Programmable Logical Controllers (PLC) or Structured Query Language (SQL) databases. Furthermore, manufacturing companies usually run machines and software systems from different vendors or of different ages. The schemata used in such systems do therefore not follow a certain standard, i.e. they are very heterogeneous in their semantics. When building such applications, accessing, searching and understanding the data sources is becoming a very time intensive, manual and error prone procedure that is repeated for every newly build application and for every newly introduced data source. To allow for an eased access, searching and understanding of these heterogeneous data sources, an ontology can be used to integrate all heterogeneous data sources in one schemata.

This repository contains an ontology of a section of VDI guideline 2206 that contains a lightweight model to describe the abstract structure of machines (see Figure 1). We maintain a whole list of standard-based ontologies, check out these links:

 - [DIN EN 61360](https://github.com/hsu-aut/IndustrialStandard-ODP-DINEN61360)
 - [VDI 3682](https://github.com/hsu-aut/IndustrialStandard-ODP-VDI3682)
 - [VDI 2860](https://github.com/hsu-aut/IndustrialStandard-ODP-VDI2860)
 - [DIN 8580](https://github.com/hsu-aut/IndustrialStandard-ODP-DIN8580)
 - [ISA 88](https://github.com/hsu-aut/IndustrialStandard-ODP-ISA88)
 - [WADL](https://github.com/hsu-aut/IndustrialStandard-ODP-WADL)
 - [DIN EN 62264-2](https://github.com/hsu-aut/IndustrialStandard-ODP-DINEN62264-2)
 - [OPC UA](https://github.com/hsu-aut/IndustrialStandard-ODP-OPC-UA)
 - [ISO 22400-2](https://github.com/hsu-aut/IndustrialStandard-ODP-ISO22400-2)

## VDI 3682 - Formalized Process Description
The VDI 2206 (Design methodology for mechatronic systems) according to [1] contains concepts for the description of mechatronic systems
and their containment structure. Hereby, the guideline defines necessary constituents of a mechatronic ssystem as well as a description
on how they are related. Figure 1 shows the lightweight ontology of the VDI 2206.

![](./pictures/VDI2206_LWO.png?raw=true "VDI 2206 LWO")<br></br>
Figure 1: Lightweight Ontology of the VDI 2206

As the VDI 2206 does not define any inheritance concepts, but it provides concepts to general for direct use, the parent-child
concept introduced in [2] can be applied to overcome this modelling issue. Here, any member of any class of the VDI 2206 can be also 
member of one of the classes shown in Figure [2], in order to enable inheritance.

![](./pictures/parentChild_LWO.png?raw=true "Parent Child LWO")<br></br>
Figure 2: Parent-child concept with respect to [2]

Exemplary Competency Questions that could be answered with this ODP:<br></br>
Table 1: Example Competency Questions
![](./pictures/VDI2206_exCQ.png?raw=true "exampleCQ")


[1] Guideline VDI 2206. Design methodology for mechatronic systems, 06.2004.<br></br>
[2] R. Woll, “Informationsruckfhrung zur Optimierung der Produktentwicklung,” Dissertation, Berlin, 2001.
