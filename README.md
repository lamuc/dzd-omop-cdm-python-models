# DZD - OMOP CDM Python Data Classes Representation
A Python Pydantic / SQLmodel representation of the Observational Medical Outcomes Partnership (OMOP) Common Data Model (CDM)
  
This project is build upon sqlacodegen ❤️ Big thanks for the hard work of the community at https://github.com/agronholm/sqlacodegen
  
Author/Maintainer: Tim Bleimehl  
Status: Proof of Concept successfull. Working towards a Beta Version  
  
This projects consists of two parts:
  
## OMOP Classes code generator
The first one is the code generator that generates Python data classes based on the OMOP CDM. It support different 4 styles of dataclasses:  
  
* `tables` (only generates `Table` objects, for those who don't want to use the ORM)
* `declarative` (the default; generates classes inheriting from `declarative_base()`
* `dataclasses` (generates dataclass-based models; Python v1.4+ only)
* `sqlmodels` (generates model classes for [SQLModel](https://sqlmodel.tiangolo.com/))

## OMOP Python Data Classes modules
This is the output of of the OMOP Classes code generator.