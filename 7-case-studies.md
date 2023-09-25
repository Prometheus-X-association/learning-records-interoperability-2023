[Interoperability of Learning Records: State-of-the-Art in 2023](README.md?fileId=116427)

## 7\. Case studies

In this part, we have gathered a few significant case studies or models demonstrating interoperability in learning records.

### 7\.1 Gaia-X DASES

Started in March 2021, several actors of the education and skills sector have created a working group called [DASES](https://prometheus-x.org/). DASES stands for Data Space of Education and Skills and the objective of this working group is to build the first European data space for the Education and Skills sector, within the Gaia-x Initiative.

DASES has brought together various actors in the educational sphere in order to bring a sovereign vision of digital education to the European level. This vision is embedded in a human-centric, ethical and trustworthy framework, which is developed and supported by an adequate governance system for education and skills data.

DASES working group was then divided into several sub-group, each focusing on a specific use case. Learning records is one of these key use case which consists in enabling actors to pool aggregated data in order to train artificial intelligence algorithms. This is a necessity for public and private sectors, as well as for research. Solving the issue related to this use case would have many benefits: allows actors to cross data sets that are currently fragmented, limits cold start problems, exploit unused data in a trusted environment, larger datasets to open up training possibilities for Machine Learning models and interoperability of educational data.

As a result, DASES xAPI working group was created with a common goal: building a common xAPI profile for DASES in order to improve the interoperability of learning record data sets.

This working group has organized their work in two ways:

* synchronous meeting where expert in Learning analytics shares the issues they are facing and the solutions they developped
* asynchronous work through a common [github](https://github.com/gaia-x-dases) to share, review and approve xAPI profile

The objective of the DASES xAPI working group is to publish a first version of a common xAPI profile on the official [ADLnet server](https://profiles.adlnet.gov/organization/e8c5169e-3b55-45e5-a03f-8ec20f4db1a0/about) by end of 2023.

### 7\.2 France université numérique

[France université numérique (FUN)](https://www.fun-mooc.fr/en/) is the French national platform to promote the use of massive open online courses (MOOCs). The portal is supported by t open edX open source platform, and supported by Google since September 2013. The audiovisual content is hosted on OVH servers.

FUN endorses the [open source transformation](https://info.france-universite-numerique.fr/open-innovation/ouvrir-le-code-what-else/) as proposed by numerous public policy reports and action plans that aim to encourage the use of free software, support administrations, animate a community and network, and recognize contributors.

For open source to have the greatest impact, it must be practiced meticulously and with transparency. This approach also allows for broader dissemination of the code, creating a richer, internationally-scaled community. FUN has undergone this transformation from 2018 to 2020 by automating and optimizing hosting, redirecting resources towards development and innovation, and improving reliability and performance.

French state policy aims to promote the use of cloud-based solutions at a large scale. Solutions must be secured, robust, scalable, available, and rely on techniques and practices that allow such deployments.

In higher education and research, pooling human resources also increases efficiency and financial leeway. Universities employing developers who understand the realities of the field can contribute to common projects.

Moreover, this approach does not exclude interactions with innovative solutions from educational technology (EdTech) startups. Using the Learning Tools Interoperability (LTI) protocol, an externally sourced solution can easily interoperate with a Learning Management System (LMS), automating and controlling the transfer of information, collecting and storing Learning Records according to xAPi standard, etc.

As one of the major MOOC platform in France, FUN has a high trafic and thus was confronted to the limited scalability of conventional LRS. As a result, they have developed their internal LRS to manage millions of learning records they collect each day.

Among the tools they have developed internally, they have open sourced [Ralph](https://github.com/openfun/ralph) which is a toolbox for learning analytics.
Ralph can be used as a:

* library, to fetch learning events from various backends, (de)serialize or convert them from various standard formats such as xAPI, or openedx,
* command-line interface (CLI), to build data pipelines the UNIX-way™️,
* HTTP API server, to collect xAPI statements (learning events) following the ADL LRS standard.

### 7\.3 LOLAMETER

Within the university of Lorraine, the LORIA laboratory has a team of researcher dedicated to Learning Analytics: LOLA (Laboratoire Ouvert en Learning Analytics, or Open Laboratory in Learning Analytics). The Lola team focuses on Learning Analytics, which aim to make the vast amount of collected learning data readable and interpretable. The goal is to assist educational institutions facing challenges like massification, flexibility, personalization, or individualization of training. The use of interaction traces in learning situations, particularly through artificial intelligence and data mining techniques, allows for various types of feedback. This feedback can be directed towards the learner, tutor, trainer, peers, resource designer, or institution. It often comes in the form of synthetic indicators, predictors, visualization tools (like dashboards), or intervention systems such as personalized recommendation systems.

LOLA team addresses various aspects through five main functions:

* DATA: LOLA allows French research teams, Edtech companies, and educational institutions to share data corpora to test their models or algorithms and compare them on common data.
* MODELS: LOLA provides the educational community with state-of-the-art open-source models, which educational institutions can test on their data sets and use in their own application context.
* APPLICATIONS: Various visualization tools are featured, along with the application context in which they were developed and used. If usage feedback is available, it will be presented, highlighting the advantages and disadvantages of each according to the application contexts.
* EVALUATIONS: Several indicators are provided, allowing for the creation of a dashboard or the calculation of an aggregate score. These different indicators have been developed and tested in the context of various projects or collaborations.
* SUPPORT: There is a real need for documentation and guides. This section offers various types of support tailored to different targets. Here, guides and charters that are identified as relevant and available in the Resources section are gathered. Finally, LOLA also allows teachers, students, and institutions to describe the actions they have taken and their impacts, in order to share their experience.

The rapid spread of standards xAPI has resulted in an increased usage of LRS within digital learning systems.

Various LRS software has been introduced to the market, with similar base functionalities (recording and retrieving xAPI statements), but many varying additional features. Non-functional requirements such as scalability, response time, and throughput may differ between LRSs. Therefore, the selection of an appropriate LRS is of high importance to an organization.

Recently, LOLA team has published an [operational framework](https://hal.science/hal-02985541v1.https://hal.science/hal-02985541v1) for analyzing the performance behavior of LRS under a set of test scenarios. Two open-source LRS were studied and analyzed using this framework: Learning Locker and Trax.

As a tool to better evaluate the scalability of LRS, LOLA team has developper the Lolameter. This tool is a stress test tool for LRS. According to tests made with this tool, both Learning Lockers and Trax LRS loose more than 15% of statements when more than 500k statements are sent in short time.

With the aim to provide a benchmarking Framework to help in the selection process of an LRS, the authors discussed performance requirements in the paper, [Towards an automated Framework for benchmarking Learning Record Stores: Performance Requirements and Scalability](https://hal.science/hal-02469663v1). A similar discussion is also found in "Trade-off between interoperability and data collection performance when designing an architecture for learning analytics".

Furthermore, the METAL project, as detailed in another paper ([Learning analytics made in France: the METAL project](https://www.researchgate.net/publication/332250358_Learning_analytics_made_in_France_the_METAL_project)), is to improve the quality of teaching by focusing on all the aspects of a learning analytics environment. The METAL project also tackles different concerns of a learning analytics environment, such as data storage through the implementation of an LRS.

### 7\.4 T3network

[T3 Network](https://wiki.t3networkhub.org/wiki/Main_Page), short for Talent Transfer and Technology, is a digital network structure that is being developed in order to improve the learning and employment ecosystem. It comprises several interconnected 'networks' working together to streamline processes and improve efficiencies. T3 Network promotes data interoperability and harmonization across diverse stakeholders, including: employers; education, training, and credentialing providers; government agencies; and technology partners. This digital transformation will ensure that (1) all learning counts; (2) skills are used like currency; and (3) learners and workers are empowered with data to pursue education and employment opportunities.

T3 network includes 4 sub networks:

1. Open Competencies Network (OCN): This network aims to provide the infrastructure required for easy access to information about knowledge, skills, abilities, and practices necessary for a healthy learning and work ecosystem, meeting the needs of various stakeholders including employers, learners, training organizations, government bodies, etc.
2. Data and Technology Standards Network (DTS): This network acts as a catalyst for the development and implementation of standards-based specifications and services to realize the ecosystem envisioned by the T3 Innovation Network.
3. Learning and Employment Record Network (LER): Centered around the learner, this network intends to establish best practices for the creation and sharing of records containing education, training, work, and personally acquired skills and competencies.
4. Jobs and Workforce Data Network (JWD): This network concentrates on improving the development, organization, sharing, and utilization of job and workforce data. It aims to add value for different stakeholders and improve the efficiency and diversity of talent markets, while ensuring privacy for employers and workers.

In Nov 2022, the Jobs and Workforce Data Network has published a guide about [Skills-Based Hiring and Advancement: LERs, Resumes, and Related Data Standards](https://assets.website-files.com/62d09b4cd38ec93ebb6738a2/636c0bd79c59ff1534c71fdf_USCCF_T3Network_SBHADiagram_v2.pdf). According to this guide, generating Learning and Employment Records (LERs) and using them in skills-based hiring and advancement requires the use of data standards. The T3 Innovation Network is supporting the development and use of data standards and related technologies to empower learners and workers with data about their knowledge, skills, and abilities. Among the standards, T3 Network highlights a few standards related to Learning records: ADL cmi5 (xAPI profile), ADL/IEEE xAPI (P9274.1)

### 7\.5 Estonia Learning Data infrastructure

The governance of skill systems is very complex. Thus, evidenced-based decision making requires reliable data. However, establishing and maintaining an integrated information system is challenging and requires commitment of different stakeholders. Estonia is one of the few countries that successfully established and maintains a digital, online and encompassing database that brings together data on important parts of the education system such as schools, pupils, teachers, exams and qualifications

The Estonian government manages the collection and usage of data in the education and training sector through three systems, in order to support their commitment to evidence-based decision-making.

The primary platform for this is the [Estonian Education Information System (EHIS)](https://www.educationestonia.org/data/). This state database is comprehensive, containing information on all aspects of education in the country. It includes data on educational institutions, students, teachers, graduation documents, study materials, and curricula, among other things. This system is meant for everyone in the education sector, from students to teachers, to academic staff. It provides insight into the qualifications and further training completed by educators. Furthermore, it helps monitor the education system to ensure it prepares individuals for the future labor market. The EHIS database has stored data since 2005, making detailed information available about general education levels across the population.

In addition to EHIS, the public can access the visual educational statistics database, HaridusSilm (Education Eye). This database encompasses statistical data about education, research & development, language policies, and the youth field in Estonia. This includes data on various educational levels and lifelong learning participation. It provides an overview of the progress towards the goals set out in the education strategy.

Finally, the Estonian Research Information System (ETIS) acts as a national platform focused on research and development. It includes information on institutions, researchers, and their respective projects. The system is used for a variety of purposes, from submitting and reviewing grant applications to publishing CVs and sharing research results. ETIS, which was established by the Estonian Ministry of Education and Research, and operated by the Estonian Research Council, is used by numerous research institutions as their internal research information system.

These systems together create a detailed, transparent, and accessible overview of the education and training sector in Estonia, facilitating policy making and the overall governance of skills systems. As a result, Estonia is able to maintain and continue to develop a successful, advanced, and efficient education system that caters to all of its citizens.

Estonia is currently working on a new digital infrastructure to improve its data collection capabilities and enable new feature such as personalised learning.

One of the innovative idea suggested by Peep Küngas is to develop a "[Learning Pixel service](https://projektid.edu.ee/pages/viewpage.action?pageId=53126696)". The core of the project is the installation of the Learning Pixel service and the measurement of student progress. The service allows the collection and analysis of educational material data. To install the application, a certain code is added to the <head> element of the web application. The ID-XXXXXXXX assigned to the service must be replaced with the application ID issued by the service provider.

The Learning Pixel service also facilitates tracking of various events related to the use of educational material. These events are automatically converted into xAPI statements.

Through the service, you can add metadata to educational resources and transmit the pseudonym of the learner. This enables user-based analytics of the use of educational applications across different applications. Learning Pixel also collects various usage data such as the web application ID, unique ID of an anonymous user, event-related data, website URL, timestamp, browser information, etc.

Future plans require specification of the JSON scheme and the nomenclature of events and their conversions into xAPI statements.

### 7\.6 Learning records on blockchain

In a recent article entitled "[Managing Lifelong Learning Records through Blockchain](https://www.academia.edu/39065727/Managing_lifelong_learning_records_through_blockchain)" a team of researchers explores the ground-breaking use of blockchain to manage detailed records of learning activities, thus solving the 'cold-start' problem faced by learning data analytic platforms. It introduces the concept of Blockchain of Learning Logs (BOLL), a unique platform enabling the secure and verifiable transfer of learning records from one institution to another.

One of the key strengths of the BOLL is it's capacity to allow access to a learner's records from a multitude of institutions. This is made possible by the careful management of access rights through smart contracts, which require consent from the learners and/or the concerned institution for the logs to be accessed. Further, the study highlights how BOLL could connect learning records across institutions - a major breakthrough in the field of learning records.

The research provides a comprehensive overview of BOLL's implementation process, shedding light on its resource requirements and enumerating the myriad advantages over existing similar tools. This work, which stands at the junction of education and blockchain technology, not only uncovers new possibilities for managing extensive learning records, but it also provides a template for future research and practice in consolidating learning achievements across various platforms and institutions. The authors' thorough analysis sets a precedent for the fusion of technology and education in a way that benefits both learners and educational institutions.

### 7\.7 Combining Learning record from multiple sources

The article titled "[How EFL Learners React to a Learning Framework Integrating Learning Records on Multiple Systems](https://www.academia.edu/97304403/How_EFL_learners_react_to_a_learning_framework_integrating_learning_records_on_multiple_systems)" meticulously delves into an integrated learning framework that converges a web e-portfolio and two mobile applications. Authored by Hiroya Tanaka, Akio Ohnishi, Ken Urano, Shinya Ozawa, and Daisuke Nakanishi, the research focuses on investigating how Japanese English as a Foreign Language (EFL) students interact with this multi-system platform as a part of their vocabulary learning regimen.

The researchers developed two unique mobile apps; Lexinote Word Rehearsal (WR) and DoraCAT, as well as a web e-portfolio, Lexinote, to execute a vocabulary learning program more methodically. This unique framework integrates learning records from each system into individual learners' e-portfolios, providing a deep and personalised insight into the learners’ progress.

The authors conducted a preliminary study probing two key aspects: how students use these systems to prepare for in-class vocabulary tests and how they appraise the effectiveness of each system for their vocabulary enhancement.

The study involved 66 Japanese EFL students, who evaluated the applications and educational materials at the conclusion of the course. Results disclosed a preference for one mobile application over others for their vocabulary learning needs.

The research, besides its immediate findings, underlines the potential of such an integrated multi-system framework in facilitating a more self-regulated and metacognitive approach to language learning. This integration of learning records provides an avenue for a more nuanced understanding of individual learning patterns and progress. As such, the authors' innovative approach to integrating multiple systems into a unified learning framework offers valuable insights for future research and instructional design in the context of EFL education.

The paper titled "[xAPI Made Easy: A Learning Analytics Infrastructure for Interdisciplinary Projects](https://publications.rwth-aachen.de/record/861310/files/861310.pdf)" by Birte Heinemann, Matthias Ehlenz, Sergej Görzen, and Ulrik Schroeder, addresses the critical challenges of integrating multiple learning environments like labs with traditional educational software, and subsequently the capturing of crucial learning activities within these environments.

The researchers tackle this issue through the lens of Learning Analytics, specifically multi-modal Learning Analytics (MMLA), which makes it possible to collect, analyze, and interpret data from multiple learning sources. It is particularly useful for complex learning scenarios such as laboratory-based learning.

A chief challenge outlined in the paper is the interdisciplinarity of MMLA projects, where lab experts might not have substantial expertise in collecting data on users’ behavior. The authors propose a potential solution in the form of Experience API (xAPI), a specification for recording learning experiences of any sort. Their xAPI infrastructure creates standardized data from various sources like Moodle, VR, or lab sensors.

The methodology involves the use of Learning Record Stores (LRS), with each learner’s experience represented by a statement integrating an actor, verb, and an object. Also included are extensions that offer more information on results, context, or the activity itself. To capture key learning objectives within these complex lab environments, the authors have developed a structured approach, where each statement has an International Resource Identifier (IRI) and reference to metadata.

The authors have also developed a registry that aims to align with good scientific practices, modern research data management conventions, and considers FAIR data principles. Their scientific-first implementation ensures widespread acceptance within the scientific community.

This infrastructure would allow a deeper understanding of student experiences in the lab, or when using innovative technology. The paper explores different stakeholder perspectives, usability, and convenience of the infrastructure, and suggests potential applications this infrastructure might bring along.

The authors sit at the intersection of education, technology, and psychology, innovating the way we perceive, record, and analyze learning experiences in modern learning environments. Their work sets a strong precedent for using Learning Analytics and xAPI in diverse learning environments, and opens up new avenues of research and applications in the field.

The theis titled "[A Software Architecture and Reference Implementation Based on xAPI for a Modular, Personalized Learning Platform](https://opus4.kobv.de/opus4-rhein-waal/frontdoor/index/index/docId/1771)" discusses the development of an advanced learning platform that utilizes xAPI to create a seamlessly coordinated e-learning environment.

Interactive learning platforms with various modules and components typically require a complex management system for learning data and progress synchronization across different entities. This paper extends the pre-existing TierschutzErleben platform, blending a cutting-edge, xAPI-based learning data specification, a front-end framework, and a video game engine.

The study revolves around designing a central control unit responsible for learning data management and orchestrating multiple platform components. The authors developed a learning path recommendation system designed by instructors, effectively guiding students through the material. To ensure efficient communication, interfaces are established, and a service for relaying events between components is introduced. These events include instructions that prompt specific actions on the receiving end.

All these innovative features form a unified control layer capable of coordinating data from multiple different sources, providing a clear view of events and their associated actions. Additionally, the use of the command execution system organized these commands, streamlining the seemingly complex process.

This research presents a groundbreaking approach to e-learning platform design, making significant strides in offering streamlined, personalized learning experiences to users. It showcases the capabilities of xAPI in creating coordinated, modular learning platforms, effectively contributing to the latest advances in Learning Records.

### 7\.8 References

 1. Prometheus-X. Home. Available at: https://prometheus-x.org/ (last consulted on 2023-09-08).
 2. Gaia-X. Gaia-X Data Architectures for Data Ecosystem Services. Available at: https://github.com/gaia-x-dases (last consulted on 2023-09-08).
 3. ADL Profile. Organization. Available at: https://profiles.adlnet.gov/organization/e8c5169e-3b55-45e5-a03f-8ec20f4db1a0/about (last consulted on 2023-09-08).
 4. FUN-MOOC. Home. Available at: https://www.fun-mooc.fr/en/ (last consulted on 2023-09-08).
 5. FUN. Ouvrir le code: what else? Available at: https://info.france-universite-numerique.fr/open-innovation/ouvrir-le-code-what-else/ (last consulted on 2023-09-08).
 6. OpenFun. Ralph. Available at: https://github.com/openfun/ralph (last consulted on 2023-09-08).
 7. Labba, C., Roussanaly, A., & Boyer, A. An Operational Framework for Evaluating the Performance of Learning Record Stores. Available at: https://hal.science/hal-02985541v1 (last consulted on 2023-09-08).
 8. Labba, C., Roussanaly, A., & Boyer, A. Towards an automated Framework for benchmarking Learning Record Stores: Performance Requirements and Scalability. Available at: https://hal.science/hal-02469663v1 (last consulted on 2023-09-08).
 9. Manuel-dodero, J. et al. Trade-off between interoperability and data collection performance when designing an architecture for learning analytics. Available at: https://www.sciencedirect.com/science/article/abs/pii/S0167739X16302017 (last consulted on 2023-09-08).
10. METAL Project. Learning analytics made in France: the METAL project. Available at: https://www.researchgate.net/publication/332250358_Learning_analytics_made_in_France_the_METAL_project (last consulted on 2023-09-08).
11. Labba, C., Roussanaly, A., & Boyer, A. Towards an automated Framework for benchmarking Learning Record Stores: Performance Requirements and Scalability. Availabe at: https://hal.science/hal-02469663v1 (last consulted on 2023-09-08).
12. Labba, C. Un Outil pour l’Analyse Automatique des Performances des Entrepôts de Données d’Apprentissage-LRS. Available at: https://edunumrech.hypotheses.org/files/2020/11/METAL_performances-des-entrepots_Chahrazed-Labba.pdf (last consulted on 2023-09-08).
13. T3 Network. Main Page. Available at: https://wiki.t3networkhub.org/wiki/Main_Page (last consulted on 2023-09-08).
14. T3 Network. Available at: https://assets.website-files.com/62d09b4cd38ec93ebb6738a2/636c0bd79c59ff1534c71fdf_USCCF_T3Network_SBHADiagram_v2.pdf (last consulted on 2023-09-08).
15. OECD. Strengthening the Governance of Skills Systems. Available at: https://www.oecd-ilibrary.org/docserver/298d6678-en.pdf?expires=1693579007&id=id&accname=guest&checksum=D4BA2135F21DB43DF4CDF07456679497 (last consulted on 2023-09-08).
16. Education Estonia. Data. Available at: https://www.educationestonia.org/data/ (last consulted on 2023-09-08).
17. Education Estonia. Services and Products. Available at: https://www.educationestonia.org/services-and-products/ (last consulted on 2023-09-08).
18. Projektiid Edu. Home. Available at: https://projektid.edu.ee/pages/viewpage.action?pageId=53126696 (last consulted on 2023-09-08).
19. Ocheja, P. et al. Managing Lifelong Learning Records through Blockchain. Available at: https://www.academia.edu/39065727/Managing_lifelong_learning_records_through_blockchain (last consulted on 2023-09-08).
20. Tanaka, H. et al. How EFL learners react to a learning framework integrating learning records on multiple systems. Available at: https://www.academia.edu/97304403/How_EFL_learners_react_to_a_learning_framework_integrating_learning_records_on_multiple_systems (last consulted on 2023-09-08).
21. Heinemann, B. et al. xAPI Made Easy: A Learning Analytics Infrastructure for Interdisciplinary Projects. Available at: https://publications.rwth-aachen.de/record/861310/files/861310.pdf (last consulted on 2023-09-08).
22. Mezghani, M. R. A software architecture and reference implementation based on xAPI for a modular, personalized learning platform. Available at: https://opus4.kobv.de/opus4-rhein-waal/frontdoor/index/index/docId/1771 (last consulted on 2023-09-08).