---
layout: default
title: Checklist Service Integration
parent: Integrated Services in ROHub
nav_order: 1
---

## Checklist Service Integration
In ROHub the  checklist  service is  adapted  and  extended to  interact  efficiently  with  the  latest ROHub  (Research  Object management)  platform  to  support  RELIANCE  metadata models  and  vocabularies. Additionally new  checklists can be created by users to  reflect the RELIANCE community’s need. The checklist service also facilitates easy creation and customisation of checklist to the ROHub community needs for the purpose of automated quality checking mechanism of the ROs. The checklist service exposes a simple REST API to assess the RO quality. The checklist service functionalities in ROHub exposes them to the user via the ROHub portal. 
In  ROHub  portal, the  checklist  functionality  is  available  from the completeness tab  of  the  Research  Object.  From  this  tab,  the  users  can (re-)evaluate  the Research Object completeness against the default or the provided check lists on demand. The default checklist  is  based  on  the  RO  type. The  result  of  the  evaluation  is  displayed  in compact  form  in  the  overview  tab,  whereas  detailed  information is  presented  in  the completeness tab. The basic sets of quality checking parameters that are shown in the completeness tab includes the following:

* If the RO has a title
* If the RO has a description
* If the RO has a creator
* If the RO has publisher information
* If the RO has a subject (research area)
* If the RO has a sketch
* If the RO has keywords
* If the RO aggregates at least one resource
* if the resources aggregated by the RO has a type
* Optionally, the RO may have authors defined for credits
* Optionally, the RO may have contributors defined for credits
* Optionally, the RO may have geolocation associated

Additionally for some specific types of ROs (e.g. Bibliographic centric RO, Data-centric RO, Executable RO) there are few more additional check paramets listed as below:

* Bibliographic-centric RO:
** If in the RO there is at least a resource in “biblio” folder  