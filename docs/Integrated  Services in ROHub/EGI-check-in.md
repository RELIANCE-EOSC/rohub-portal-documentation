---
layout: default
title: EGI check-in
parent: Integrated Services in ROHub
nav_order: 7
---

## EGI check-in

The ROHub Identity and Access Management (IAM) is based on Keycloak technology. It allow users to  authenticate  to  ROHub  and  enables  the  single  sign-on across  different  RELIANCE  services.  The most important feature of ROHub IAM is that it is integrated with EOSC AAI. In particular it allows the user  to  authenticate through  the EGI  check-in  service. The ROHub portal uses the production  instance  integrated  with  production  EGI  check-in  and  having  the  official  set  of  ROHub users. The figure below depicts  the  ROHub  login  page  to  authenticate  through  the  selected Keycloak instance. From there, the user can  authenticate via the EGI check-in service or by providing directly his email and password.


<p align="center"> <img src="https://box.psnc.pl/f/aaf1bf8fc4/?raw=1" width="700"> </p>
<div align="center"> Figure 1: ROHub login page </div>

If  the  user  selects  to  login  with  EGI  check-in,  then can use any  of  the  identity  providers supported  by  EGI  check-in  service such  as  its  academic  institution  or  one  of  the social  account  providers  (e.g.,  orcid,  google,  Facebook,  GitHub,  LinkedIn,  etc.).  After  selecting  the academic/social  identity  provider,  the  user  should  follow  the  normal  process  of  the  provider  to authenticate,  providing  its  username/email  and  their  password.  If  the  user  chooses  to  provide  his email and password directly on ROHub login page, (s)he should provide its password in ROHub (not their academic/social account password).


<p align="center"> <img src="https://box.psnc.pl/f/9a1eaaf365/?raw=1" width="700"> </p>
<div align="center"> Figure 2: EGI check-in login page in ROHub portal </div>