---
layout: default
title: Integration with EGI Binders
parent: Integrated Services in ROHub
nav_order: 11
---

## Integration with EGI Binders
ROHub also integrates EGI Binder service that enable users not only to open and execute their Jupyter Notebooks directly from ROHub portal, but also to reproduce the full computing environment by pre-loading  all  the  libraries  and  dependencies required  to  execute  the  notebook resource. Binder supports the best  practices that are reproducible in data science by utilizing community-developed standards   for reproducibility. 

In order to use this functionality the  user  needs  to  have  an  account  with  access  to  [EGI Binder service](https://binder.notebooks.egi.eu/) and also need to have an account and be logged in ROHub. Moreover the resource to be reproduced must have type “Jupyter Notebook” and the  Research  Object  must  aggregate  at  least  one  configuration  file named requirements.txt or environment.yml

The notebook is connected to the configuration file via the relation “Software Requirements” (from schema.org).  This relation can be established by selecting  the  notebook  in  the  resources  section  of  the  Research  Object  edition  mode,  and  then creating the relation under the show all annotations, as depicted in Figure below.


<p align="center"> <img src="https://box.psnc.pl/f/914956d354/?raw=1" width="700"> </p>
<div align="center"> Figure 1: Establishing a relation between two resources in ROHub portal </div>


In addition to the environment requirements, the user is able to specify data resources (e.g., input dataset) or other resources that should be available from Binder once the notebook is loaded. In order to specify these resources, the user needs to create a file e.g., datasets.txt, which contains the list of resources that need to be available from Binder, and connect it to the notebook via the relation "Requires Dataset". Each required resource is identified via its URI (e.g., shared link in ROHub) and specified in a separate line in the file, as depicted in the block below.  

```
https://w3id.org/ro-id-dev/a19fad22-2896-4223-bbef-2e81168687a2/resources/dac9a837-ddf6-4d49-b68b-8abb1846ebe9
https://w3id.org/ro-id-dev/a19fad22-2896-4223-bbef-2e81168687a2/resources/098c84b4-d017-466a-9f4a-083b2f723dbb
https://w3id.org/ro-id-dev/a19fad22-2896-4223-bbef-2e81168687a2/resources/c9d19403-55bb-48c4-ab65-5fbd83f1478a
```

When the user clicks on such resource in ROHub  portal,independently if it’s an internal or external resource the user can choose to go to the resource itself or download the notebook or to open it in EGI Binder, as depicted in the figure below. If the user opens the resource in EGI Binder, the service will be  launched,  all the  dependencies  will be  imported to  recreate  the computing  environment and then theuser will be able to execute the notebook.


<p align="center"> <img src="https://box.psnc.pl/f/12f022f00d/?raw=1" width="700"> </p>
<div align="center"> Figure 2: Opening a Jupyter Notebook in EGI Binderfrom ROHub portal </div>


<p align="center"> <img src="https://box.psnc.pl/f/336d893fca/?raw=1" width="700"> </p>
<div align="center"> Figure 3: Recreating computing environment in EGI Binder from the ROHub resources </div>