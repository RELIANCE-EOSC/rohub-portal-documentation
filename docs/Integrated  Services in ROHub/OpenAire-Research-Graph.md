---
layout: default
title: Integration with OpenAire Research Graph
parent: Integrated Services in ROHub
nav_order: 12
---
## Integration with OpenAire Research Graph
ROHub portal is also integrated with the [OpenAire  Research  Graph](https://graph.openaire.eu/) that follows the  [Guidelines for  Literature  Repository  Managers  4.0](https://doi.org/10.5281/zenodo.1299203) and supports the EC  Open  Access  requirements.The ROHub portal exposes the Research   Objects   collection to   the   OpenAIRE   infrastructure,including the funding information whereever  applicable and  the  list  of  their aggregated resources.  Additionally,  ROHub portal also exposes  the Jupyter   Notebooks   and   Data   Cubes as   especially   relevant collections with their connections  to  Research  Objects.  This  required  to  implement and  configure an  [OAI-PMHv2.0](http://www.openarchives.org/OAI/openarchivesprotocol.html) endpoint in  [ROHub](http://api.rohub.org/api/oai2d/) that produce XML  metadata for OpenAIRE  harvesting. A  partial  record  of  a Research Object in XML is shown in the figure below.


<p align="center"> <img src="https://box.psnc.pl/f/7593e76f6e/?raw=1" width="700"> </p>
<div align="center"> Figure 1: Research Object metadata record in XML format from ROHub OAI-PMH endpoint </div>

As  a  result of this integration, the  Research  Objects and  the other special  resources are discoverable  via  the [OpenAire/EOSCexplore  portal](https://beta.explore.openaire.eu/), as  depicted  in the figure. The target frequency for OpenAire harvesting is daily, i.e., in an incremental basis so that only new records will be retrieved each day


<p align="center"> <img src="https://box.psnc.pl/f/404d94f336/?raw=1" width="700"> </p>
<div align="center"> Figure 2: Research Object metadata record in XML format from ROHub OAI-PMH endpoint </div>