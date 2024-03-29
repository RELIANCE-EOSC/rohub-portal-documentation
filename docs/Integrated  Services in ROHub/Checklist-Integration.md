---
layout: default
title: Checklist Service
parent: Integrated Services in ROHub
nav_order: 1
---

## Checklist Service 
In ROHub the  checklist  service is  adapted  and  extended to  interact  efficiently  with  the  latest ROHub  (Research  Object management)  platform  to  support  RELIANCE  metadata models  and  vocabularies. Additionally new  checklists can be created by users to  reflect the RELIANCE community’s need. The checklist service also facilitates easy creation and customisation of checklist to the ROHub community needs for the purpose of automated quality checking mechanism of the ROs. The checklist service exposes a simple REST API to assess the RO quality. The checklist service functionalities in ROHub exposes them to the user via the ROHub portal. 
In  ROHub  portal, the  checklist  functionality  is  available  from the completeness tab  of  the  Research  Object.  From  this  tab,  the  users  can (re-)evaluate  the Research Object completeness against the default or the provided check lists on demand. The default checklist  is  based  on  the  RO  type. The  result  of  the  evaluation  is  displayed  in compact  form  in  the  overview  tab,  whereas  detailed  information is  presented  in  the completeness tab. In  ROHub  Portal,  this  functionality  can  be invoked  from  the  completeness  tab, by clicking the “Update” button.  The  result  of  the  assessment  is  then  displayed  in  detail,  where  each  condition  has  a  status icon:  green  check  icon  if  the  condition  was  satisfied,  red  cross  icon  if  a  MUST  condition  was  not satisfied, and yellow hyphen icon if a SHOULD/MAY condition was not satisfied. Moreover, for those conditions not satisfied, a “Fix” button will appear next to it, if the user has permissions to write the RO. This button takes  the  user  to the  edition mode  to  fix those  problems. To  facilitate  this  process, the completeness score appears in edition mode and the conditions not satisfied can be seen under the “completeness suggestions” collapsible section as depicted in the Figures below.

<p align="center"> <img src="https://box.psnc.pl/f/62cf654c63/?raw=1" width="700"> </p>
<div align="center"> Figure 1: Checklist service interface in ROHub </div>


<p align="center"> <img src="https://box.psnc.pl/f/f554dbda0a/?raw=1" width="700"> </p>
<div align="center"> Figure 2: Completeness information in Research Object edition mode in ROHub </div>





The basic sets of quality checking parameters that are shown in the completeness tab includes the following:

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

<p align="center"> <img src="https://box.psnc.pl/f/19b6556b16/?raw=1" width="700"> </p>
<div align="center"> Figure 3: Checklist in Basic RO </div>




Additionally for some specific types of ROs (e.g. Bibliographic centric RO, Data-centric RO, Executable RO) there are few more additional check paramets listed as below:

Bibliographic-centric RO:
* If in the RO there is at least a resource in “biblio” folder  

<p align="center"> <img src="https://box.psnc.pl/f/7d59dafb18/?raw=1" width="700"> </p>
<div align="center"> Figure 4: Checklist in Bibliographic centric RO </div>



Data-centric RO:
* In if the RO there is at least a resource in “raw data” folder
* If in the RO there is at least a resource in “data” folder
* In in the RO there is at least a resource in “metadata” folder

<p align="center"> <img src="https://box.psnc.pl/f/efbcff828c/?raw=1" width="700"> </p>
<div align="center"> Figure 5: Checklist in Data-centric RO </div>




For an Executable RO:
* In in the RO there is at least a resource in “input” folder
* If in the RO there is at least a resource in “tool” folder
* If in the RO there is at least a resource in “output” folder


<p align="center"> <img src="https://box.psnc.pl/f/91c01f2210/?raw=1" width="700"> </p>
<div align="center"> Figure 6: Checklist in Executable RO </div>