---
layout: default
title: Integration with B2Drop
parent: Integrated Services in ROHub
nav_order: 9
---

## Integration with B2Drop
The ROHub supports RO storage in B2Drop EOSC  service. The  user  can  select  the  default storage type from their account settings as depicted below. When  selecting  B2Drop, the  usersneed  to  provide  their  B2Drop  credentials also via  the  account settings. These  credentials  can  be  obtained  from  the  B2Drop Web  portal  navigating  to  the  security section from the user settings (“create new app password”)

<p align="center"> <img src="https://box.psnc.pl/f/a872e4ebca/?raw=1" width="700"> </p>
<div align="center"> Figure 1: Selection of storage type from ROHub user account settings in  ROHub portal </div>



<p align="center"> <img src="https://box.psnc.pl/f/709d29d5fb/?raw=1" width="700"> </p>
<div align="center"> Figure 2: B2Drop user settings </div>

When B2Drop is  selected as  the default  storage, ROHub  creates  the root folder “Rohub/ros” in the user’s B2Drop space.Then,for  each newly  created  RO  by  the  user,  which  aggregates  physical resources, a folder with the RO id is createdinside that root folder, as depicted in Figure 7-10below. When  using  B2Drop, the  users  need  to  take  into  account thespace  available  in  their own B2Drop account. The Research Objects’ internal resources will use this space, and If his/her B2Drop account has  no  more  space  available,  then  the user  will  not  be  able  to  aggregate  physical resources  in  his/her Research  Objects. One  additional  feature,  currently  under  testing,  is  the  synchronization  of  the  RO folder  in  B2Drop  with  ROHub,  i.e.,  resources  added  into  the  RO  folder  in  B2Drop  via  any  interface (e.g., B2Drop Web portal) will be automatically aggregated in the RO.


<p align="center"> <img src="https://box.psnc.pl/f/c0de25366c/?raw=1" width="700"> </p>
<div align="center"> Figure 3: B2Drop folder structure created by ROHub </div>