# ROHub portal documentation

![ROHub logo](images/image58.png) 


## Introduction
ROHub[1] is a research object management platform supporting the preservation and lifecycle management of scientific investigations, research campaigns and operational processes. As the only existing platform implementing natively the full research object model and paradigm, resources associated to a particular experiment are aggregated in a single digital entity (research object), and metadata reliant to understand and interpret the content is represented as semantic annotations that are user and machine readable.


ROHub can support different stakeholders, with the primary focus on scientists, researchers, students and enthusiasts, enabling them to manage and preserve their research work, to share it and make it available for publishing, to collaborate and to discover new knowledge.
However, other user groups can be benefited by ROHub like the Industry that can leverage
the platform to externalize their research to a community of researchers worldwide in multiple scientific domains, e.g., launching campaigns for research on specific topics, and to follow and monitor the progress. Similarly, investors can keep up to date and track scientific advances to fund and get involved in future breakthroughs. As another example, publishers can also leverage ROHub to advertise their journals with researchers, have access to a pool of potential reviewers, and implement more interactive review processes.


### ROHub portal


ROHub portal is a Web client application providing a comprehensive user interface for the management and preservation of research objects (ROs). ROHub portal integrates and provides access to different research object services, such as:
* The core RO backend service, enabling the creation, storage, maintenance and access to research objects, the management of their lifecycle, and their preservation. The backend leverages various EOSC services including Zenodo and B2Share for RO publication, as well as B2Drop for resources storage (ongoing). 
   * RO backend also includes a notification service, enabling the subscription to events related to a particular research object (e.g., changes in content or quality), or to the portal itself (e.g., when new ROs are created).
* The ROHub AIM (Identity and Access Management) service, powered by Keycloack open source solution, and which is integrated with EOSC AIM service (EGI check-in)
* RO enrichment service (also onboarded in EOSC), which generates automatically semantic annotations based on the (textual) resources aggregated in order to improve the discoverability and searchability of research objects.
* RO PDF generation service, allowing the retrieval of the RO in paper style in PDF format. 
* EOSC (EGI) Notebooks (under integration) to allow the loading of notebooks aggregated in an RO directly on the EGI notebooks environment.
* RO checklists service (under integration), providing remote access to the minim-based evaluation of research objects, used to test for completeness, runnability or repeatability. 
* RO stability service (under integration), enabling the evaluation of the RO through time by capturing concrete values provided by the checklist service in different moments of its evolution. It allows testing the ability of a research object to achieve its original purpose after being subject to changes on its resources. 
   * RO stability includes the RO monitoring tool, providing an interface to visually monitor and keep track of the status of external datasets and web services required for workflow execution. It's based on the stability service. 
* RO collaboration spheres (under integration), providing an interface for the discovery of research objects that are similar or related to the selected research object or scientist.

## ROHub Portal pages
### Home
The homepage or landing page provides a general overview of the ROhub platform which includes a keyword search component from which the user can directly start finding research objects and creator information, a section for the featured research object where selective research objects (golden examples) can be featured based on their completeness and impact factor. The landing page also includes a section for the key statistics of the ROHub and a section with the recent activities showing the latest changes or events on the ROHub platform. The figure below depicts the partial view of the homepage of ROhub portal.
  

  

Figure xx Landing page of the ROHub platform


#### Basic search by keyword
This component enables users to find research objects by keywords, looking through all the metadata annotations available, e.g., title, description, creator, etc. The user can easily look for research objects or resources by providing any associated keyword and thereafter the user can look for the desired resources from the explore page.
 
  

Figure XX: Keyword search component

#### Featured research objects
This section presents the list of ROs that are promoted because of their quality (measured based on the RO compliance according to some specified criteria like completeness, impact etc.) or because of their popularity (e.g., golden examples) as depicted in figure below.
  

Figure XX Featured research objects component
#### Recent activity
This section presents the latest three ROs that were created most recently, resources added to research objects, snapshots or archives or any recent activities on the ROs. By clicking on the “Read more” the user can go to the main RO overview page for detailed representation. 
  

Figure XX Recent activity component


#### Key Statistics of ROHub platform
This section of the landing page shows the key statistics of the ROHub platform consisting of the number of research objects created with all the resources, total number of annotations, total number of users in the portal. 
  
 
Figure XX Key statistics of the ROhub platform


### Login
The login (Sign in/Sign up) is available on the menu bar of the homepage. The keycloak authentication system allows the users to login either with predefined EGI credentials or users can register themselves with login and password. Once registered the authentication system allows the registered users to sign in to the ROhub portal. The figures below show the login and sign up functionalities of the ROhub portal.
  

Figure XX Login page of ROhub portal


  

Figure XX User registration page of ROhub portal

#### User account settings
The user account settings can be accessed by the users once they are logged into the portal. There are various components that can be access via the user account setting page, such as:
* Edit Account: In this page the user can update and save the personal user-specific information to update the account. This information includes email, firstname, last name, affiliation of the user etc. 


  

Figure XX Edit Account page for ROHub users


* Change password: This section enables the user to change the password of his account in ROHub. This password is independent of the EGI check-in password.
  

Figure XX Password reset page


* Authenticator: This system allows the user to save the device as a second level authentication. This is done through third party authentication applications (e.g. FreeOTP, Google Authenticator). The application scans the barcode provided in the user’s account and generates an OTP which along with the name of the device can be saved. 


  

Figure XX User Authentication in ROHub platform


* Federated identities: This section shows the user identity in EGI check-in, if any, which is essentially the username of the user in EGI.
* Sessions: Shows the current sessions for the user account. The session record consists of information like the  user IP address, the start and end time of the session etc. 
* Applications: This section shows the IAM application clients that this user is able to use to authenticate in ROHub, along with the roles and permissions associated to this account. The client used is generally transparent to the user, as it is set internally by the application itself (e.g., ROHub portal, ROHub python library, Enrichment service, etc.). 
  

Figure XX Page showing applications accessed by a ROHub user


* Log: This section shows all the available activity log for the user account in ROHub, including the date of the event, type of the event (i.e., login), IP source, application client used, and any additional information like the username and authentication method used. 


### Research Object 



------

You can use the [editor on GitHub](https://github.com/RELIANCE-EOSC/rohub-portal-documentation/edit/main/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/RELIANCE-EOSC/rohub-portal-documentation/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
