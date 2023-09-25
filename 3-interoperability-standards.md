[Interoperability of Learning Records: State-of-the-Art in 2023](/)

## 3\. Interoperability of Learning Records standards

Rapid advancements in technology have transformed the landscape of education, with e-learning emerging as a viable alternative or complement to traditional classroom learning. Ensuring the reliability and uniformity of e-learning experiences necessitates the establishment of stringent standards and norms.

Historically, the creation and application of learning technologies were primarily managed by small, localized groups of experts, which were often no larger than a single school, university, or corporate training department. However, with the advent of extensive global communication networks and the benefits of scale, there is now a growing drive towards adopting learning technologies that are scalable on an international level.

Within the sphere of e-Learning, numerous regional, national, and global entities have made strides in establishing universal standards and specifications. Five organizations are notably at the forefront of these efforts:

1. Advanced Distributed Learning (ADL) Initiative
2. IEEE Learning Technology Standards Committee
3. Alliance for Remote Instructional Authoring & Distribution Networks for Europe (ARIADNE)
4. Aviation Industry Computer Based Training (CBT) Committee (AICC)
5. 1Edtech Inc. (formerly IMS Global Learning Consortium)

Their collective efforts have significantly contributed to streamlining and standardizing eLearning technologies, enhancing their potential to enable effective learning experiences.

### 3\.1 History of Learning records

Learning records have a rich history, with the concept having evolved significantly over the past couple of decades due to the new possibilities offered by the emerging of new digital learning technologies.

Before the advent of digital learning, the collection, storage, and use of learning records relied heavily on traditional, manual methods.
Collection: Learning records were generated from various activities in and out of the formal (physical) classroom setting. Data on attendance, classroom participation, assignments, projects, and exam scores contributed to a learner's cumulative record. This information was collected manually by teachers on paper, who may have kept individual logs, grade books, or class registers to document student performance and behavior.
Storage: Learning records were physically stored on paper in a variety of formats. Cumulative folders or student files were often used to store individual student records throughout their educational journey within a particular school or institution. These folders would typically contain report cards, standardized test scores, attendance records, disciplinary notes, and other details of a student's academic history. Libraries and dedicated record rooms were often employed to store these physical records.
Use: The use of learning records was primarily for progress tracking, report making, parent-teacher discussions, and placement decisions. Trainers, teachers, or school administrators would review the records to understand a student's performance, identify areas where the student might be struggling, and make educated decisions about appropriate intervention or support strategies. Moreover, the records were used for administrative purposes, as well as to meet local and national reporting requirements.

The transition to digital learning has dramatically changed the landscape of how learning records are collected, stored, and used. Today, digital learning platforms can collect a much wider array of learning data more efficiently and accurately, store it securely in databases with vastly larger capacities, and analyze it to yield insights far deeper and more actionable than was formerly feasible.

The concept of standardized (digital) learning records gained momentum in the early 2000s with the advent of Sharable Content Object Reference Model (SCORM). As an e-learning software specification, SCORM marked a significant step toward achieving interoperability of learning content, the concept that various technological systems could communicate, exchange data, and use this data in a seamless and integrated manner. SCORM became the de facto standard for e-learning interoperability, guiding course structure, sequencing, and data interactions within LMS platforms from 2001 onward.

The governing body of SCORM is [Advanced Distributed Learning (ADL) Initiative](https://en.wikipedia.org/wiki/Advanced_Distributed_Learning), a US government program that conducts research and development on distributed learning and coordinates related efforts broadly across public and private organizations. ADL reports to the US Defense Human Resources Activity (DHRA), under the Director, DHRA. Although it is a United States Department of Defense (DoD) program, ADL serves the entire US federal government, operates a global partnership network including international defense ministries and US-based academic partners, and collaborates closely with industry and academia.

Despite its success and widespread use, ADL recognized that SCORM couldn't keep pace with the rapid evolution of information technology, especially given the surge of mobile devices, social media, and cloud-based technologies that transformed the global learning landscape. Accordingly, ADL initiated in 2010, a Broad Agency Announcement (BAA) soliciting detailed research papers on possible improvements to the SCORM standard. The BAA was awarded to Rustici Software, resulting in a year-long research and development project known as Project Tin Can. The project aimed to overhaul the existing SCORM specifications to create a more modern, flexible, and extensible standard that could keep pace with the evolving tech world.

The finale of Project Tin Can was the introduction of the Experience API (xAPI), which offered a significant advance over the SCORM model. xAPI, colloquially known as Tin Can API, provided a new way to capture learning experiences from a wider range of sources and contexts, delivering more granular, diverse, and all-encompassing data about learners' activities.

Also developed was the concept of the [Learning Record Store (LRS)](https://en.wikipedia.org/wiki/Learning_Record_Store), a crucial component in the xAPI specification. The LRS offered a new type of data storage specifically for learning records, acting as a repository for storing, retrieving, and processing learning data, all these, regardless of where learning occurred or what platform or device was used.

Now, the xAPI and LRS concepts are revolutionizing the e-learning industry, fostering data-rich, personalized, and effective learning environments. However, it is with deep appreciation of the path paved by SCORM and the pioneers of learning record interoperability that xAPI and LRS maintain their stride into the future of e-learning.

### 3\.2 From SCORM to xAPI

The explosion of user data systems in the past few decades kindled the need for standard regulations for sourcing and contextualizing this data. Prior to 2000, organizations employing e-learning systems faced significant challenges when upgrading or changing vendors, often having to scrap their existing content.

To this end, the year 2000 saw the introduction of SCORM, which uncoupled content from its creating apparatus, rendering it applicable to any platform or system. This standard birthed by the ADL Initiative allowed for creation of content that was reusable, robust and platform-independent.

Several iterations of SCORM were launched, with SCORM 2004 Fourth Edition being the most recent. With pervasive internet access and mobile usage, learning has relocated to various informal settings, a landscape where traditional Learning Management Systems (LMS) fell short. Thus, a need for a more versatile learning specification was recognized.

In response, the search for a SCORM successor commenced in 2008 and culminated in 2011 in an agreement between the ADL Initiative and Rustici Software. The resultant collaborative project, “Project Tin Can”, led to the formation of a universal e-learning specification, xAPI, with the latest version being 1.0.3. xAPI enabled collection of data on a myriad of experiences in online and offline training activities.

Influenced by the Representational State Transfer (REST) architecture, xAPI rests on the ‘RESTful web-service APIs and leverages the JSON data format and a Learning Record Store (LRS). As of now, version 2.0 is undergoing standardization, with several improvements aimed at refining definitions, standardizing timestamps, and precisely outlining the functions of an LRS.

In a nutshell, xAPI is a versatile solution enabling data collection on a broad range of experiences in diverse learning instances. Vis-à-vis older e-learning norms that can capture only digital experiences, xAPI's shared data format facilitates learning data transfer between different systems while providing the flexibility to focus on uniquely relevant tracking aspects.

Correspondingly, SCORM (Sharable Content Object Reference Model) is an e-learning standard that records and tracks learner outcomes, presenting course results, responses, viewed pages, viewing duration, time spent on course, and scored learning objectives, in a LMS. SCORM's principal benefit, interoperability, ensures seamless importation of SCORM-compliant content into any LMS that supports this standard.

### 3\.3 xAPI data model

The Experience API (xAPI), also known as Tin Can API, is a technical specification for recording and tracking learning experiences. It is an open-source standard that enables learning records to be stored and shared across different systems and platforms. The xAPI defines a set of statements that describe a learning activity, such as "learner watched a video," "learner completed a quiz," or "learner attended a workshop."
The xAPI allows for more granular tracking of learning activities compared to traditional learning management systems (LMS), which typically only track course completions. With xAPI, learning records can be collected from a variety of sources, including mobile devices, simulations, games, and social media, providing a more comprehensive view of a learner's activities and achievements.

In simple terms, an xAPI statement is a way of recording a learning activity or experience in a consistent format. Typically, an xAPI statement follows an "Actor-Verb-Object" structure, which translates to "Who did what to what?"

#### 3\.3.1 Statement structure

Let's break down the structure:

1. **Actor**: This is who completed the action. The actor is usually a person but can be a group or an organization. For instance, in the statement "John completed a quiz," 'John' is the actor.
2. **Verb**: This is the action that the actor carried out. In the same example, 'completed' is the verb.
3. **Object**: This is what the action was performed on. In our example statement, 'a quiz' is the object.

Those are the three primary components required for an xAPI statement. However, a statement usually also include additional details that provide further context, such as:

1. **Timestamp**: This documents when the action occurred.
2. **Context**: This provides extra information about the situation in which the action took place. It could include details about the specific learning environment, platform, or other relevant activities.
3. **Result**: This captures the outcome of the action. For instance, in the statement "John scored 85% on a quiz," '85%' would be the result.

#### 3\.3.2 Example of statement

Let's take and example:

"John (Actor) completed (Verb) the Mathematics course (Object) on January, 19th at 10:34 am."
This xAPI statement indicates that John finished his Math course successfully.

According to xAPI, the corresponding JSON for the above example will look like this:

```json
{
  "actor": {
    "name": "John",
    "objectType": "Agent"
  },
  "verb": {
    "id": "http://adlnet.gov/expapi/verbs/completed",
    "display": {
      "en-US": "completed"
    }
  },
  "object": {
    "id": "http://example.com/MatheMaticsCourse",
    "definition": {
      "name": {
        "en-US": "Mathematics Course"
      },
      "description": {
        "en-US": "The Mathematics Course that John completed"
      }
    },
    "objectType": "Activity"
  },
  "timestamp": "2022-01-19T10:34:00Z"
}
```

In this JSON representation, `actor` represents John, `verb` represents the action completed, `object` represents the Mathematics Course, and `timestamp` is the date and time the action occurred in a specific pattern (ISO 8601 format). This pattern ("2022-01-19T10:34:00Z") indicates that the date was January 19th, 2022, and the time was 10:34:00 in Coordinated Universal Time (UTC).

The xAPI specification has a built-in feature to handle custom parameters that don't fit into the established set of fields (actor, verb, object, result, context, timestamp, etc.). This feature is called the "extensions" attribute.

The extensions attribute is an open-ended, container field, where you can add as many extra data points as you want. This makes xAPI incredibly flexible and adaptable to a wide range of use cases, since it allows for capturing unique or granular details about any learning experience.

So, let's say for instance, you are developing an e-learning solution for an industrial safety course, and you want to track when a learner uses a specific safety equipment in a Virtual Reality (VR) simulation. In this case, an 'extensions' field can be added to the xAPI statement to record this specific detail.

Here's an example of what that might look like:

```json
{
  ...
  "context": {
    "extensions": {
      "http://example.com/used_safety_equipment": true
    }
  }
}
```

In this case, the URL "http://example.com/used_safety_equipment" is a unique identifier for the fact that the learner used a specific safety equipment in the VR simulation. The value associated with this identifier (true) could reflect that the learner did use the equipment.

As such, the extensions attribute enables the collection of highly specific, rich data about a learner's engagement and actions, which can help better understand the learning process and allow for more personalized and effective learning solutions.

### 3\.4 Cmi5: interoperability between SCORM and xAPI

[Cmi5](https://aicc.github.io/CMI-5_Spec_Current/) is a specification developed by Advanced Distributed Learning (ADL) with the intention of bridging SCORM and xAPI, two previously established standards in e-Learning.

SCORM, or Sharable Content Object Reference Model, has been a standard for e-Learning content for years. It dictates how e-Learning courses and Learning Management Systems (LMSs) communicate with each other. However, it has some limitations due to the lack of offline learning capabilities, limited data reporting, and the inability to track informal learning experiences.

To handle these limitations, xAPI (Experience API, also known as Tin Can API) was developed. xAPI's powerful experience tracking capabilities allow it to collect detailed data about learner activities across various platforms and contexts, including mobile learning, games, simulations, offline experiences, and more.

The cmi5 standard is designed to utilize the best features of SCORM and xAPI. While using xAPI's broader, flexible capabilities for tracking learning experiences, cmi5 also ensures the LMS's control over the learning environment like SCORM.

The cmi5 specification defines a standard way of launching courses and communicating status back to the LMS, allowing it to incorporate and control the learner's experience. cmi5 also standardizes the way that course completion, pass/fail, and scoring information should be handled to ensure consistency across different LMSs - something that xAPI leaves open to interpretation.

With cmi5, a course can both stand alone (distributed via a web server) or be hosted in an LMS, and in both these scenarios, tracking is done in a standard way, enabling seamless data exchange between different systems. With the standard definitions of the cmi5 for both 'launched' and 'completed' states, Learning Records can thus be interchanged more effectively between SCORM and xAPI systems.

So, in essence, cmi5 helps the interoperability of Learning Records between SCORM and xAPI by prescribing standard rules for launching, grouping of content, tracking session time, reporting back to the LMS, and so on - merging the flexibility of xAPI to account for multifarious learning experiences with the structured control of SCORM for successful data integration.

#### 3\.4.1 What are the benefits?

cmi5 focuses on being more extensible, robust and adaptable to today’s modern technologies than the legacy SCORM standard, including having all the xAPI benefits, tracking newer technologies, maintaining compatibility and allowing for content to reside anywhere.

#### 3\.4.2 What are the technical details?

The specification uses xAPI as the communication and data layer and implements controlled vocabularies for plug and play interoperability across systems. Want to dive deeper based on your role? View the technical overview for content professionals or for systems professionals.

#### 3\.4.3 Why use cmi5 instead of SCORM

These few reasons may encourage you to use the new standard instead of SCORM.

1. It allows offline mobile learning Unlike with SCORM, cmi5 courses can be taken both online and offline. Students can take course materials when there’s no Internet connection with special mobile apps. The progress will be saved and sent to the LMS once the connection is restored.
2. It records any kind of activity With SCORM, you can only store predefined parameters. Unlike SCORM, the data that cmi5 tracks is not limited: you can get detailed information on learners’ activity, such as: Store an audio recording of your student responding to a question Store a video of your student performing a task Store an essay written by your student It’s also possible to track images, PDFs, audio and video files, and simulations.
3. It enables studying outside an LMS SCORM tracks formal instructor-led learning and leaves out much of modern learning that happens outside an LMS. Consider gaming and simulations, social learning and mobile apps – all these sources can be used and tracked with the cmi5 standard.
4. It’s easier to implement While SCORM is complicated, the cmi5 specification is only a few pages. It works “on top of” xAPI, so if you know the latter, you should be able to implement cmi5 quite easily.
5. It allows content distribution If you have worldwide students and you really care about them, then save them from using SCORM. With this standard, content must be stored on the same server as your LMS. This means that learners from far away must be really patient with the content load times. The question is becoming even more important, as content modules are getting bigger and bigger. With cmi5, only the course structure is imported, not the actual content. This means that content itself can reside anywhere. You can choose to store materials on a content distribution network (CDN) with several servers around your country or even around the world, so when your students open the content, they will automatically connect to the closest server.
6. It provides a better user experience This is what Art Werkenthin, president of RISC, Inc. and a member of the ADL cmi5 committee, says about the SCORM problem with pop-up windows: If you have ever used SCORM, you know about the pop-up windows. With SCORM, you get at least two windows: one for the LMS and the other for the SCORM content. Usually, you get more than two because sometimes the SCORM content decides to have its own “player” window. If you are an LMS administrator, you know you have to watch out for SCORM’s arch enemy—the pop-up blocker! How many times have you answered a call from a student who says, “The content won’t open”? You dread going on the hunt for all the possible pop-up blockers that may be installed on the student’s workstation. (Tip from the trenches: I’ve found as many as seven pop-up blockers on a single machine.) Even if you clear out all the pop-up blockers, you still get the occasional student that hates pop-up windows … so they just close them immediately, thereby breaking your SCORM module. Finally, if you want to support mobile, pop-ups are a “no-no.” Luckily, this was one of the first issues addressed in cmi5. Content can now launch in the same window as the LMS. The LMS disappears and the content opens; simple as that. When the content is done, it disappears and the LMS returns—right where you left off.

#### 3\.4.4 How cmi5 enhances xAPI

Here is how Ben Clark of Rustici Software describes the value cmi5 adds to xAPI: “xAPI is wide open, there’s so much this standard can do that people don’t know what to expect out of it and they don’t know how to track certain things consistently. cmi5 is there to put some of the rules back on top of xAPI. And even though the new standard does have more rules and provides more structure, instructional designers still have a wide open field to track whatever they want to.”

#### 3\.4.5 cmi5 CATAPULT: Accelerating the adoption of xAPI and cmi5

Since cmi5 was first released in 2016, there’s been a missing piece that has slowed its adoption. From development to procurement, tools are needed to support adoption of cmi5 and xAPI both within the Department of Defense (DoD) and the industry as a whole. Most importantly, there has not been an authoritative source or governance of the cmi5 specification as we have seen with the xAPI LRS conformance test suite and the SCORM conformance test suite. [cmi5 CATAPULT](https://xapi.com/cmi5/cmi5-project-catapult/) aims to help fill those needs.

![cmi5-catapult.png](https://github.com/inokufu/learning-records-interoperability-2023/blob/master/img/cmi5-catapult.png?raw=true)

### 3\.5 Interoperability between xAPI and IMS Caliper

[IMS Caliper Analytics](https://www.imsglobal.org/activity/caliper) provides a framework that allows educators to gather and leverage data tied to learner interactions within the context of a course in an educational environment. The framework defines how institutions and businesses can use its platform, apply the collected data, and evaluate their effectiveness. Caliper utilizes the resources provided by IMS Global standards to ensure optimal data transfer.

#### 3\.5.1 Statement structure

Similarlyy to xAPI, Caliper uses a three-part monitoring model: "Actor", "Action", and "Activity". The "Actor" denotes the individual or system carrying out an action. The "Action" represents the performed behavior, and the "Activity" highlights the focus or object of the action.

Caliper's information model outlines various concepts, rules, and relationships designed to encapsulate the behaviors exhibited by learners. These behaviors are illustrated through Caliper profiles (like annotation, forum, session, etc.), featuring Event Types where users partake in activities characterized by a specific vocabulary. Additionally, the model provides Entity types (like agent, attempt, result, etc.) to elucidate the interactions between participants and components. This comprehensive framework offers an efficient way to track and analyze learner engagement and performance.

For Caliper, JSON-LD provides the necessary representational horsepower to both describe these kinds of data linkages and specify how data is to be understood when published and shared across a network.

#### 3\.5.2 Example of statement

Here is an example of learning record statement according to IMS Caliper:

```json
{
    "@context": "http://purl.imsglobal.org/ctx/caliper/v1p2",
    "id": "urn:uuid:fcd495d0-3740-4298-9bec-1154571dc211",
    "type": "SessionEvent",
    "profile": "SessionProfile",
    "actor": {
        "id": "https://example.edu/users/554433",
        "type": "Person"
    },
    "action": "LoggedIn",
    "object": {
        "id": "https://example.edu",
        "type": "SoftwareApplication",
        "version": "v2"
    },
    "eventTime": "2016-11-15T10:15:00.000Z",
    "edApp": "https://example.edu",
    "session": {
        "id": "https://example.edu/sessions/1f6442a482de72ea6ad134943812bff564a76259",
        "type": "Session",
        "user": "https://example.edu/users/554433",
        "dateCreated": "2016-11-15T10:00:00.000Z",
        "startedAtTime": "2016-11-15T10:00:00.000Z"
    }
}
```

See example in spec here: https://www.imsglobal.org/spec/caliper/v1p2

Here is an example of an IMS Caliper Analytics JSON-LD event statement. Please note that this example shows a simple reading event where a student has viewed a reading material:

```json
{
  "@context": "http://purl.imsglobal.org/ctx/caliper/v1p1",
  "id": "urn:uuid:a50ca17f-5971-47bb-8fca-4e6e6879001d",
  "type": "ReadingEvent",
  "actor": {
    "id": "https://example.edu/user/554433",
    "type": "Person"
  },
  "action": "Viewed",
  "object": {
    "id": "https://example.com/etextbook/2018/geometry/chapter1",
    "type": "DigitalResource",
    "name": "Chapter 1"
  },
  "eventTime": "2018-08-01T06:00:00.000Z"
}
```

In this JSON-LD example:

* `@context` provides the context for the data, which is the URL of the Caliper context document.
* `id` is the Unique Event Identifier.
* `type` is `ReadingEvent`, representing the event of the actor viewing the object.
* `actor` is represented by the user identifier and type.
* `action` signifies the type of action the actor performed. In this case, `Viewed`.
* `object` contains the specifications for the object viewed by the actor, followed by its ID, type, and name.
* `eventTime` provides information about when the action occurred, in a specific ISO 8601 format.

#### 3\.5.3 Comparison of xAPI and IMS Caliper

xAPI and IMS Caliper share some similarities but also have profound differences.

Similarities:

1. Both are used for tracking learning experiences: xAPI and IMS Caliper are both designed to track, store, and retrieve data about learning experiences.
2. JSON-based data: Both xAPI and IMS Caliper records are based on JavaScript Object Notation (JSON), making them lightweight and easy to work with.
3. Detailed Learning Analytics: Both standards facilitate deep and granular learning analysis by allowing the tracking of fine-grained learning activities.

Differences:

1. Messaging Philosophy: The xAPI follows an Actor-Verb-Object (e.g., "John completed a quiz") paradigm which offers great flexibility and granularity. In contrast, IMS Caliper models events based on Metric Profiles (e.g., Reading, Assessment, Media, etc.), which categorizes activity types, offering a more structured schema.
2. Interoperability Scope: xAPI is somewhat more versatile given its application goes beyond just the web environment. It can track learning experiences across various platforms like mobile learning, games, simulations, and even offline learning. IMS Caliper, although comprehensive, primarily targets web-based digital learning environments.
3. LRS vs. Sensor API: xAPI uses a Learning Record Store (LRS) to store and retrieve learning data. However, Caliper uses a Sensor API approach, where different 'sensors' input data based on the event that has happened.

As for the translation of IMS Caliper learning records into xAPI format and vice versa, this typically requires middleware or a translation service that can understand both schemas. This software would map the fields in a Caliper event to their corresponding fields in an xAPI statement, create a new xAPI-compliant statement, and send it to an LRS.

Such a solution could theoretically be developed using technologies like Python or Node.js, but it's important to note that this translation process would require a solid understanding of both specifications to ensure accurate mapping and maintenance of data integrity. As of now, there's no widely recognized or commercialized software that offers this specific translation between Caliper and xAPI. However, developers and educators in the desire or need of such a service usually design it based on the unique demands of their systems.

Ultimately, both standards are designed with a similar goal: to improve the understanding of student learning through analytics. The right one to use often depends on the specific use case, or an institution may choose to use both in different contexts to fully cater to their analytical needs.

### 3\.6 References

Learning Record Store - Wikipedia. https://en.wikipedia.org/wiki/Learning_Record_Store

https://en.wikipedia.org/wiki/Advanced_Distributed_Learning

Sanders, Jerey. 2023. “Conformance and Interoperability of E-learning Standards.” SocArXiv. March 15. doi:10.31235/osf.io/3x7ew. https://osf.io/preprints/socarxiv/3x7ew/

Analyse des traces d’apprentissage – Learning analytics : productions du GTnum 2
https://edunumrech.hypotheses.org/1559

Arvaniti, Despoina, 2023, TRACKING LEARNING WITH EXPERIENCE API, https://apothesis.lib.hmu.gr/bitstream/handle/20.500.12688/10503/ArvanitiDespoina2022.pdf?sequence=1&isAllowed=y

xAPI website, last consulted on 2023-09-01, https://xapi.com/overview/

xAPI-Spec, ADLNET, github repository, last consulted on 2023-09-01, https://github.com/adlnet/xAPI-Spec

The cmi5 Project, AICC, github page, last consulted on 2023-09-01, https://aicc.github.io/CMI-5_Spec_Current/

https://adlnet.gov/assets/uploads/cmi5%20Best%20Practices%20Guide%20-%20From%20Conception%20to%20Conformance.pdf
https://xapi.com/cmi5/cmi5-project-catapult/

https://adlnet.gov/assets/uploads/cmi5%20Best%20Practices%20Guide%20-%20From%20Conception%20to%20Conformance.pdf

SCORM to cmi5 Terminology, https://xapi.com/cmi5/scorm-to-cmi5-terminology/

https://www.ispringsolutions.com/blog/ispring-now-supports-cmi5-the-next-generation-of-scorm

https://www.linkedin.com/pulse/cmi5-call-action-robert-bilyk/

1edtech Caliper Analytics, https://www.imsglobal.org/activity/caliper

Arvaniti, Despoina, 2023, TRACKING LEARNING WITH EXPERIENCE API, https://apothesis.lib.hmu.gr/bitstream/handle/20.500.12688/10503/ArvanitiDespoina2022.pdf?sequence=1&isAllowed=y

https://www.imsglobal.org/spec/caliper/v1p2
