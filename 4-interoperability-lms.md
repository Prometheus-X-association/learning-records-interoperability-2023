[Interoperability of Learning Records: State-of-the-Art in 2023](/)

## 4\. Interoperability of Learning Management System

In this part, we have analysed the various Learning Management System (LMS) available on the market. For each LMS, we have gathered as much information as possible about their compatibility with the major Learning Records standards (xAPi, SCORM, IMS Caliper, cmi5) from their website, support center (forum, knoledge base) or dvelopper documentation when available.

The compatibility of the LMS with the main learningrecords standards are compiled in the table below.

**Table 4.1. Compatiblity of LMS with Learning Records standards**

| Name | Link | Free | xAPI | IMS Caliper | SCORM | cmi5 |
|------|------|------|------|-------------|-------|------|
| BlackBoard | [Link](https://www.blackboard.com) | No | [Yes](https://help.blackboard.com/Learn/Instructor/Ultra/Course_Content/Create_Content/Add_Content_Packages/ULTRA_Add_SCORM) | [Yes](https://site.imsglobal.org/certifications/anthology/blackboard-learn#cert_pane_nid_404018) | [Yes](https://help.blackboard.com/Learn/Instructor/Ultra/Course_Content/Create_Content/Add_Content_Packages/ULTRA_Add_SCORM) | No |
| LearnDash | [Link](https://www.learndash.com) | No | [Yes](https://www.learndash.com/support/docs/reporting/scorm-xapi/) | No | [Yes](https://www.learndash.com/support/docs/reporting/scorm-xapi/) | [Yes](https://www.nextsoftwaresolutions.com/learndash-integration/) |
| LifterLMS | [Link](https://lifterlms.com) | No | [Yes](https://podcast.lifterlms.com/how-to-add-scorm-xapi-lrs-wordpress-lms-website-interactive-content-elearning-authoring-tools-grassblade/) | No | [Yes](https://podcast.lifterlms.com/how-to-add-scorm-xapi-lrs-wordpress-lms-website-interactive-content-elearning-authoring-tools-grassblade/) | [Yes](https://podcast.lifterlms.com/how-to-add-scorm-xapi-lrs-wordpress-lms-website-interactive-content-elearning-authoring-tools-grassblade/) |
| Moodle | [Link](https://moodle.org) | Yes | [Yes](https://moodle.org/plugins/logstore_xapi) | [Yes](https://docs.moodle.org/dev/Caliper) | [Yes](https://docs.moodle.org/402/en/SCORM_activity) | [Yes](https://rusticisoftware.com/resources/play-xapi-and-cmi5-in-moodle/) |
| Open edX LMS | [Link](https://open.edx.org) | Yes | [Yes](https://docs.openedx.org/projects/openedx-proposals/en/latest/architectural-decisions/oep-0026/xapi-realtime-events.html) | [Yes](https://discuss.openedx.org/t/oep-26-plugin-for-xapi-and-caliper-support-has-been-released/6092) | [Yes](https://github.com/overhangio/openedx-scorm-xblock) | No |
| Canvas LMS | [Link](https://www.canvaslms.com) | Yes (for Teachers) | [Partially](https://canvas.instructure.com/doc/api/file.xapi.html) | [Yes](https://site.imsglobal.org/certifications/instructure/canvas#cert_pane_nid_193191) | [Yes](https://community.canvaslms.com/t5/Instructor-Guide/How-do-I-import-SCORM-files-as-an-assignment/ta-p/673) | No |
| Schoology | [Link](https://www.schoology.com) | Yes (Basic) | No | No | [Yes](https://uc.powerschool-docs.com/en/schoology/latest/course-materials-scorm-packages-and-web-content-en) | No |
| Desire2Learn | [Link](https://www.desire2learn.com) | No | [Yes](https://docs.datastreams.desire2learn.com/xapi/index.html) | [Yes](https://site.imsglobal.org/certifications/d2l-corporation/d2l-brightspace#cert_pane_nid_404767) | [Yes](https://community.d2l.com/brightspace/kb/articles/5387-import-and-manage-scorm) | [Yes](https://community.d2l.com/brightspace/kb/articles/4536-scorm-data-sets) |
| TalentLMS | [Link](https://www.talentlms.com) | No | [Yes](https://www.talentlms.com/features/scorm-lms) | No | [Yes](https://www.talentlms.com/features/scorm-lms) | [Yes](https://help.talentlms.com/hc/en-us/articles/360014571774-How-to-import-and-track-cmi5-content) |
| Adobe Learning Manager (formerly Adobe Captivate Prime) | [Link](https://business.adobe.com/be_fr/products/learning-manager/adobe-learning-manager.html) | No (Free Trial) | [Yes](https://helpx.adobe.com/in/captivate-prime/administrators/feature-summary/xapi.html) | No | Yes | No |
| Chamilo LMS | [Link](https://chamilo.org/chamilo-lms) | Yes | [Yes](https://docs.chamilo.org/admin-guide/global_features/xapi) | No | [Yes](https://docs.chamilo.org/teacher-guide/structure_learning_paths/import_aicc_and_scorm) | No |
| 360 Learning | [Link](https://www.360learning.com) | No | No | No | [Yes](https://support.360learning.com/hc/fr/articles/115001426606-Cr%C3%A9er-un-module-SCORM) | No |
| Google Classroom | [Link](https://classroom.google.com) | Yes | No | No | No | No |
| Microsoft Teams for Education | [Link](https://teams.microsoft.com) | Yes | No | No | No | No |

### 4\.1 Moodle LMS

Moodle, one of the most popular open-source LMS, facilitates the creation of customizable online courses. It offers an array of tools and features designed specifically to aid educators in teaching and assessing student performance effectively.

Moodle collects Learning Records through various built-in modules, such as assignments, quizzes, forums, glossaries, lessons, and workshops, to name a few. It captures and stores data related to learners' interactions, completion status, assessments, and feedback, among others. This data is then stored in a [logs database](https://docs.moodle.org/402/en/Logs) (typically MYSQL or PostgreSQL), which can be accessed and manipulated by the Moodle system to generate reports, predict user behavior, and customize learning paths.

Moodle inherently supports the SCORM standard, allowing SCORM packages to be included as a type of resource. This means that SCORM-compliant content from other sources can be uploaded into Moodle and Moodle can send SCORM data - like quiz results and course completion status - back to an external LMS.

As for the xAPI standard, while Moodle does not natively support it, support can be easily added using plugins, such as '[Logstore xAPI](https://moodle.org/plugins/logstore_xapi)' plugin or '[TRAX Logs](https://moodle.org/plugins/logstore_trax), which sends Moodle events to a Learning Record Store (LRS) as xAPI statements. Enabling the xAPI plugin would allow the import and export of learning records to other software that adheres to the xAPI standard.

Moodle support IMS Caliper though a [plugin](https://docs.moodle.org/dev/Caliper).

Moodle support cmi5 using a [plugin](https://rusticisoftware.com/resources/play-xapi-and-cmi5-in-moodle/).

By leveraging additional plugins or custom development, Moodle can transform into a very standards-compliant LMS, allowing it to effectively communicate and share data with other systems. However, it is essential to remember that using third-party plugins or custom development requires additional resources and technical competencies.

### 4\.1 Open edX LMS

Open edX is an open-source learning management system (LMS) that allows educators to create and deliver online courses. It is known for its flexibility, hosting everything from small local courses to large-scale global classes.

Open edX collects a wide range of Learning Records as learners navigate through courses. This data collection includes, but isn't limited to, learners' personal information, course enrollment details, session durations, and interactions with course content such as submissions of work, peer reviews, and quizzes, among other interactions. Open edX also collects detailed event logs that track every click made within the system, providing a granular view of learner behavior. These learning records are called "[Tracking Logs events](https://edx.readthedocs.io/projects/devdata/en/latest/internal_data_formats/tracking_logs/student_event_types.html)" in open EdX documentation.

These Tracking Logs events are stored within the Open edX data stores, which consist of several MySQL databases for storing different types of data and MongoDB for storing course content. This data is then used to provide insights into student learning, to enable the customization of course material, and to generate different reports and analytics in the instructor dashboard.

Here is a list of the Student Events stored by Open edX:

* Bookmark Events
* Certificate Events
* Cohort Events (Student)
* Course Content
* Completion Event
* Content Library Interaction Events
* Course Navigation Events
* Course Resource Events
* Discussion Forum Events
* Drag and Drop Events
* Enrollment Events
* Notes Events
* Open Response Assessment Events
* Peer Instruction Events
* Poll and Survey Events
* Pre-Roll Video Interaction Events
* Problem Interaction Events
* Teams-Related Events
* Testing Events for Content Experiments
* Textbook Interaction Events
* Third-Party Content Events
* Timed Exam and Proctored Exam Events
* Video Interaction Events
* Open Response Assessment Events (Deprecated)

The following example shows the relevant fields of the event that is emitted when a user selects any hypertext link from the course breadcrumb content.

```json
{
    "name": "edx.ui.lms.jump_nav.selected",
    "event": {
        "target_name": "Part 3: Getting Social",
        "id": "block-v1:edX+DemoX+Demo_Course+type@sequential+block@simulations/block-v1:edX+DemoX+Demo_Course+type@vertical+block@d0d804e8863c4a95a659c04d8a2b2bc0",
        "current_id": "block-v1:edX+DemoX+Demo_Course+type@sequential+block@basic_questions/block-v1:edX+DemoX+Demo_Course+type@vertical+block@2152d4a4aadc4cb0af5256394a3d1fc7",
        "widget_placement": "breadcrumb"
    }
}
```

When it comes to compatibility with e-learning standards, Open edX supports Learning Tools Interoperability (LTI), which allows other LTI-compliant systems to interact with the courses hosted on the Open edX platform, and vice versa.

For SCORM, Open edX does not natively support this standard. However, a third-party XBlock, named SCORM XBlock, can be installed to integrate SCORM packages into Open edX courses, thereby extending the platform's capabilities to support the ingestion and emission of SCORM-compliant data.

Due to xAPI's extensive support and use in tracking and analysing learning activities, Open Edx is working to [support xAPI](https://docs.openedx.org/projects/openedx-proposals/en/latest/architectural-decisions/oep-0026/xapi-realtime-events.html) (at least partially)  as one of the key standards for real-time events. Open edX does not plan to create its own LRS. Instead, it aims to integrate with third-party LRS services.

xAPI specifies four standard REST-ful JSON payload APIs, but OpenEdx only needs the Statement API for tracking learning activities. This includes the following components: xAPI Actor, xAPI Verb, xAPI Object, xAPI Context, and xAPI Result.

The xAPI Actor refers to the individual performing an activity. OpenEdx will primarily use the Agent type, which can be identified by different methods, including an anonymized unique identifier of the learner.

Here is an example of an Actor JSON value that open edX would generate:

```json
"actor": {
    "objectType": "Agent",
    "openid": "https://openedx.org/users/user-v1:<anonymized-user-id>",
    "name": "https://openedx.org/users/user-v1:<anonymized-user-id>"  # only include this field if necessary
}
```

The xAPI Verb denotes the past-tense action performed by the learner. OpenEdx will use standard, registered verbs as much as possible, and these are documented in the OpenEdx events section.

The registry is automatically created from multiple profiles. For now, open edX will limit ourselves to only URIs prefixed by the following domains, in the following priority order (in case of conflicting names):

* http://adlnet.gov
* http://w3id.org
* http://id.tincanapi.com

If, by any chance, a verb needed by Open edX does not exist in the registry, then open edX will create a pull request to recommend adding it to the central GitHub repository of xAPI Profiles.
Here is an example of a Verb JSON value that OpenEdx would generate:

```json
"verb": {
    "id": "http://adlnet.gov/expapi/verbs/answered"
}
```

Note, to keep the size of events as small as possible, open edX choose to avoid extraneous fields. For example, they intentionally exclude a “display” field in the example above.

The Object refers to the activity, which OpenEdx initially defines as an xAPI Activity uniquely identified by a URI. Here is an example of an Object JSON value that Open Edx would generate:

```json
"object": {
    "id": "https://courses.openedx.org/xblock/block-v1:openedx+origami-folding+1T2018+type@problem+block@abcd",
    "definition": {
        "type": "http://adlnet.gov/expapi/activities/question",
        "name": {
            "en-US": "Question on mountain fold needed to create an origami crane base",
        }
    }
}
```

The Context field allows OpenEdx to provide additional information about each statement.
Here is an example of a Context JSON value that Open Edx would generate:

```json
"context": {
    "registration": "https://openedx.org/enrollments/enrollment-v1:<anonymized-enrollment-id>",
    "contextActivities": {
        "parent": [
            {
                "objectType": "Activity",
                "id": "https://openedx.org/courses/course-v1:openedx+origami-folding+1T2018"
            }
        ]
    }
}
```

The xAPI Result specifies the score that the learner earned on an activity. OpenEdx would generate a JSON value for this, including the learner's success status, completion status, and score details. Here is an example of a JSON value that Open Edx would generate for a problem type:

```json
"result": {
    "success": false,
    "completion": true,
    "score": {
        "min": 0,
        "max": 50,
        "raw": 10,
        "scaled": 0.20
    },
    "response": "foo"
}
```

Open edX intends to support interoperability with the [IMS Caliper](https://docs.openedx.org/projects/openedx-proposals/en/latest/architectural-decisions/oep-0026/caliper-realtime-events.html) standard by using Caliper's structured approach for describing, collecting and exchanging learning activity data. Given the broad acceptance of the Caliper standard across educational institutions, Open edX sees this as an opportunity to generate events for adaptive learning engines, leading to a richer user experience.

The Caliper Sensor API helps in gathering learning metrics across systems, making it easier to marshal and transmit event data from Open edX's application to target endpoints. The set of useful profiles from Caliper for Open edX includes Assessment, Assignable, Grading, Reading, and Media.

A Caliper event describes the relationship between an actor (the learner) who performs an action on an object due to the actor's activity. Actors are typically identified by a unique identifier while keeping information to a minimum to protect the learner's privacy.

Example:

```json
{
    "id": "https://openedx.org/users/user-v1:<anonymized-user-id>",
    "type": "Person",
    "dateCreated": "2018-08-01T06:00:00.000Z",
    "dateModified": "2018-09-02T11:30:00.000Z"
}
```

Caliper actions are essentially verbs in past tense such as "Graded", "Viewed", "NavigatedTo" which bind the agent to the object.

Examples:
“NavigationEvent” supports “NavigatedTo” only.
“MediaEvent” supports a number of actions including “Started”, “Ended”, “Paused”, “Resumed”, “Restarted”, and “ForwardedTo”.

Objects are entities that an agent interacts with, and they are mostly identified by an IRI string and their type. An extensions property is also defined so that implementers can add custom attributes not described by the model. Open edX use this to pass some extra information from edX events that are not required by the Caliper specified event field. Optional properties can be ignored when describing an entity.
Example:

```json
"object": {
    "id": "block-v1:org+course+run+type@video+block@<video_id>",
    "type": "VideoObject",
    "dateCreated": "2018-11-15T10:15:00.000Z",
    "startedAtTime": "2018-11-15T10:15:00.000Z",
    "endedAtTime": "2018-11-15T10:55:12.000Z",
    "duration": "PT40M12S"
}
```

JSON-LD documents require inclusion of a context, denoted by the @context keyword, a property employed to map document terms to IRIs. Inclusion of a JSON-LD context provides an economical way for Caliper to communicate document semantics to services interested in consuming Caliper event data.
We can provide context in events in the following way:

```json
{
    "@context": "http://purl.imsglobal.org/ctx/caliper/v1p1",
    "id": "urn:uuid:3a648e68-f00d-4c08-aa59-8738e1884f2c",
    "type": "Event",......
}
https: //www.imsglobal.org/sites/default/files/caliper/v1p1/caliper-spec-v1p1/caliper-spec-v1p1.html#jsonldDef
```

### 4\.3 Canvas LMS

Canvas is a cloud-based Learning Management System (LMS) recognized for its open, extensible learning ecosystem. In Canvas, Learning Records are captured when students interact with the course content and participate in course activities. These activities can range from quiz performance, assignment submissions, discussion contributions, and course navigation, among other things.

Learning Records in Canvas are stored securely on the cloud platform, in line with strong data protection standards to maintain privacy and compliance. These Learning Records are used within Canvas to provide real-time analytics reports, giving insights to course educators on learners' academic progress and enabling the customization of learning material according to individual learning paths.

Canvas partially support [xAPI](https://canvas.instructure.com/doc/api/file.xapi.html).

As for SCORM, Canvas provides a SCORM LTI tool that allows SCORM packages to be uploaded into a course and users can interact with the content as they would in a SCORM-compatible LMS. It can both import SCORM-compliant materials and send back SCORM data (like scores and completion status) to other systems.

Canvas support [IMS Caliper](https://site.imsglobal.org/certifications/instructure/canvas#cert_pane_nid_193191) standards.

Canvas does not support cMi5.

### 4\.4 Blackboard LMS

Blackboard, a prominent Learning Management System (LMS), facilitates effective course delivery and management for educators and students alike. The platform logs learning records across a range of activities covering assignment submissions, grade entries, discussion participation, and course content engagement, to name a few.

Blackboard collects learner data and engagement metrics through its integrated tools and analytics components. These learning records are then stored securely within Blackboard's data storage system, in line with comprehensive data protection and privacy compliance measures.

Utilizing the Learning Records, Blackboard provides its users with access to Blackboard Learn, a dynamic reporting and analytics tool. Here, users can explore individual learners' performance, engagement activities, course access patterns, and progress effectively, fostering data-led teaching and administrative decisions.

Blackboard natively supports the SCORM standard, permitting the importing and exporting of SCORM-compliant packages within its platform. This allows SCORM-compliant learning data from other software to be utilized within Blackboard and vice versa, enhancing the platform’s utility.

Blackboard support xAPI but doesn't include a LRS. However basic data passed will be viewable in the gradebook.

Blackboard support [IMS Caliper](https://site.imsglobal.org/certifications/anthology/blackboard-learn#cert_pane_nid_404018) and is a contributing member of the IMS Global Learning Consortium

Blackboard does not support cMi5.

Additionally, Blackboard Learn is able to communicate with other tools and resources using the Learning Tools Interoperability (LTI) standard. LTI allows the platform to connect and intrinsically work with external tools, further enhancing the platform's resourcefulness.

### 4\.5 Schoology

Schoology is known for its ease of use and comprehensive features, this platform is popular amongst K-12 educators.
Schoology uses its own proprietary data standard for collecting, storing, and using learning records. It includes various aspects such as grades, completion status, course data, user activity, and analytics. The data collected involves metrics about course access, submission of assignments, test scores, interaction with course resources, etc.

The system collects data as the users access and engage with the platform, storing it in their own secure databases. These records are then used for various purposes like semester reports, learning analytics, performance tracking, and targeted instruction. They are especially helpful for both teachers and students to identify the strengths and weaknesses of the learning process.

Apart from this, Schoology supports the integration of multiple standards of learning records, including SCORM (for learning objects) and LTI (Learning Tools Interoperability, for integrating external tools). It's important to note that while these standards allow for some transferability of learning objects and external learning tool integration, they don't typically facilitate a full transfer of learning records in the same sense as xAPI, cmi5, or IMS Caliper.

In terms of the xAPI compatibility, Schoology doesn't natively support xAPI, but it can often be achieved using third-party integrations or workaround solutions.

As far as exportation is concerned, Schoology provides its API for developing software and tools that can export user data, courses, assignments, and other tradable pieces of data to other LMS platforms. Data can also be pulled in the form of CSV files for offline analysis.

Schoology, owned by PowerSchool, is actively working on improving data interoperability standards, which will likely enhance the capacity for detailed learning record importation and exportation across a variety of modern specifications.

### 4\.6 Desire2Learn

Desire2Learn’s Brightspace is an advanced Learning Management System that collects, stores, and uses learning records to provide comprehensive data about a student's progress and interaction within the platform.

It collects data through various engagement touch points like assignment submissions, quiz results, discussion posts, log-in frequency, etc. This data is then stored on D2L's secure servers and can be accessed using their analytics tools.

Regarding data usage, Brightspace provides an extensive array of analytics to understand student progress. It uses the data collected to paint a full picture of student learning. From individual performance reports, to complex predictive models, Brightspace uses collected data to help instructors and institutions make informed decisions.

As far as compatibility with standards for importing and exporting learning records, Brightspace supports SCORM (Sharable Content Object Reference Model) and IMS standards like LTI (Learning Tools Interoperability) and IMS Caliper. It allows for learning materials following these standards to be imported and exported between different LMS platforms.

SCORM allows instructors to package their courses in a standardized format that can be easily imported to different platforms. IMS Caliper enables the collection of learning data from different sources, allowing for comprehensive learning analytics.

D2L’s Brightspace supports [xAPI](https://docs.datastreams.desire2learn.com/xapi/index.html) and cmi5.

As far as data export is concerned, Brightspace does allow for the export of course data and user analytics, which can be downloaded in formats like CSV.

### 4\.7 LearnDash

LearnDash is a WordPress plugin that creates a fully-featured learning management system (LMS) within a WordPress site. It allows the creation of online courses, quizzes, assignments, and more.

LearnDash uses WordPress's database to store its data. It collects various types of data about users and their learning activities. This includes, but is not limited to, details about when a user logs in, completes a course, passes a quiz, or submits an assignment. This in-depth data collected by LearnDash is then used to provide teachers and admins with comprehensive reports on student progress, activity, and overall performance. In essence, LearnDash allows you to track every part of the learner's journey, making it an excellent tool for assessing both individual and overall effectiveness of a course or training program.

While LearnDash doesn’t natively support the importing or exporting of learning records following SCORM, xAPI, cmi5, or IMS Caliper standards in their platform, there are a variety of third-party plugins available that help to bridge this gap.

To improve compatibility with [SCORM and xAPI](https://www.learndash.com/support/docs/reporting/scorm-xapi/), there are plugins such as GrassBlade xAPI Companion and WP SCORM, which allow LearnDash to import SCORM and xAPI packages and track them. This allows for learning record transferability between LearnDash and other systems that adopt these protocols.

It's also worth mentioning that LearnDash offers an integration with Zapier, a very powerful app integration and automation tool that provides opportunities to export user data to various other platforms.

### 4\.8 TalentLMS

TalentLMS is a versatile cloud-based Learning Management System that is designed for delivering online training and educational courses. This is used by businesses to train employees. It includes a wide range of features, such as multimedia lessons, quizzes, and video-conferencing. It collects, stores, and uses learning records to provide comprehensive feedback about learners' progress and performance.

TalentLMS collects a variety of data points, including course completion status, individual learner progress, scores on tests and quizzes, time spent on courses, user engagement with course content and more. The specifics of the data collection will depend on the individual settings of each course and test within the LMS.

The collected data is processed and analyzed to provide extensive reports and learning analytics. These insights help in understanding user performance, engagement, and areas of improvement. Reports and analytics can be used to modify or adapt instructional methods, develop personalized learning paths, and to improve the overall learning experience.

As a cloud-based LMS, TalentLMS securely stores all generated and collected data on cloud servers. The platform has robust data privacy and security protocols in place to ensure that all learner data is safe and confidential.

In terms of data interoperability, TalentLMS supports SCORM and xAPI for course content, which allow for the importation of learning records from other platforms. SCORM and xAPI are industry standards for tracking learning activities. They are used to create and package learning content that’s easily shareable between different LMS platforms.

However, as of the time of writing, TalentLMS does not inherently support cmi5 or IMS Caliper. But there are potential workarounds for achieving compatibility through third-party plugins or custom development.

TalentLMS supports [cmi5](https://help.talentlms.com/hc/en-us/articles/360014571774-How-to-import-and-track-cmi5-content).

TalentLMS allows data exporting in various widespread formats, like CSV and Excel. Furthermore, it provides a comprehensive and robust API that allows systematic access to generated data, making it possible for this data to be utilized in other systems or software.

### 4\.9 Adobe Learning Manager

Adobe Learning Manager (formerly Adobe Captivate Prime) is a robust learning management system, part of the Adobe suite. This LMS is excellent for designing interactive content and measuring the impact of the training. It actively collects, stores, and uses learning records to provide targeted, streamlined, and seamless learning paths for its users.

Adobe Learning Manager collects a wide range of data, including course completion status, grades, time spent on activities, and interaction with learning materials. The platform's AI engine, Adobe Sensei, uses this data to make intelligent recommendations for learners based on their behaviors and preferences. Furthermore, it provides analytics and reports that allow organizations to track and measure the effectiveness and impact of their training programs.

Adobe Learning Manager supports multiple interoperability standards for learning technology. This means it can import course content created in various standards like SCORM, AICC, and xAPI. These standards allow for interactive and engaging training material to be created and packaged in a way that can be easily transferred between different LMSs.

In terms of exporting data, Captivate Prime has robust reporting capabilities, and reports can be exported in CSV format or sent directly to other users within the system via scheduled reports.

### 4\.10 Chamillo LMS

[Chamilo LMS](https://chamilo.org/en/) is an open-source LMS that is designed to facilitate online education. Learning records are crucial in this process as they consist of all the data obtained from the interactions between learners and the online learning platform.

Chamilo accomplishes the collection of learning records by tracking user interactions with the system. This includes information about when users log in or log out, which courses they enroll in, the time spent on each course, the scores achieved on quizzes and tests, and other such activities.

The software then stores this information in a database. With the application of learning analytics methodologies and technologies, this data can be used to evaluate and optimize the learning process. For example, educators can use the data to identify students who may be struggling and intervene early, or they can modify the course content based on how well it is observed to be performing.

Chamilo supports SCORM and allows tracking of the learners’ activities with xAPI.

Chamilo does not currently support other standards like cmi5, or IMS Caliper.

### 4\.11 360 Learning

360Learning is a collaborative LMS designed to facilitate effective learning engagement and improve learning outcomes.

360Learning collects data through several sources, including course interactions, course completion, assessment scores, login information, video interactions, etc.

All these interactions are stored within the 360Learning platform's secure servers with robust data privacy and security measures in place.

These data points are used by 360Learning's analytics system to generate detailed reports and insights regarding a learner's progress, engagement, performance and course completions.

360Learning is compatible with SCORM 1.2 and 2004, which means you can import SCORM compliant courses onto the platform, and the SCORM data can be reported within the platform.

360Learning does not natively support the xAPI standard, which could restrict the import/export of learning records from other software.

360Learning does not natively support cmi5 for import/export of learning records, nor IMS Caliper.

Regarding the import and export of learning records, while SCORM-compliant content can be easily managed, full learning record portability (as enabled by standards like xAPI or cmi5) may not be available within 360Learning.

### 4\.12 Google Classroom

Google Classroom is a free LMS product developed by Google as part of its Google Workspace for Education suite. It offers features that allow educators to create, distribute, and grade assignments, as well as communicate with students.

When a user logs into Google Classroom, their activities are collected, stored, and used by Google to improve service, provide custom experiences, and make recommendations. These activities might include specific assignments completed, grades obtained, assessments given, and feedback provided. This data would generally be stored in Google's secure servers, with privacy policies and regulations ensuring the protection of user data.

Google Classroom does not natively support any of the traditional e-learning standards such as xAPI, SCORM, cMi5 or IMS Caliper for collecting, storing, and utilizing learning records. Google Classroom has its unique ways of storing and structuring data according to their internal rules and mechanisms. Therefore, implementing any of the traditional e-learning standards directly into Google Classroom is not feasible.

For the import and export of data, Google Classroom uses the [Classroom API](https://support.google.com/edu/classroom/answer/6253304?hl=en&sjid=533248504110682389-EU). Through Classroom API, developers can integrate their applications with Classroom, which allows developers to access and update Classroom data. However, Classroom API is different from the traditional e-learning standards and might require additional programming effort to convert and interpret the data in these standards.

Considering the contribution of standards like xAPI, SCORM, cMi5, and IMS Caliper to achieving interoperability, their absence in platforms like Google Classroom indeed indicates an area that would benefit from further development and integration.

### 4\.13 Microsoft Teams for education

Microsoft Teams for Education is a digital hub that incorporates Microsoft tools in a single environment. It is designed to facilitate secure collaboration and communication for classrooms, enabling teachers to distribute assignments, provide feedback, and interact with students.

Boasting an array of features, including channels, chat, video conferencing, file sharing, and more, Microsoft Teams exhibits versatility in collecting Learning Records. These records consist of assignment data, communication histories, attendance records, and, when integrated with other Microsoft Education tools, student progress information, and grades.

The information Teams collects is stored within the Microsoft Cloud, a platform designed to offer high-standard security, privacy, and compliance. The Teams compliance posture includes a comprehensive set of certifications and attestations, commitment to strong data security and privacy rights that safeguard individual privacy.

Microsoft Teams does not inherently support the import or export of data with xAPI, SCORM, cMi5, or IMS Caliper standard. However, it’s important to note that Teams, as part of the larger Microsoft 365 platform, can integrate with several LMS and third-party apps that do support these standards.

Alternatively, Microsoft offers [APIs](https://learn.microsoft.com/en-us/graph/education-concept-overview) and the Microsoft Graph — a unified programmability model — that allows developers to access and integrate with data in Microsoft 365, including Teams. Although customization at this level might require significant effort, it could theoretically support the extraction and interpretation of learning data in alignment with specific e-learning standards.

That said, adoption of a comprehensive standard like xAPI or IMS Caliper by significant players such as Microsoft Teams for education would serve to further harmonize the interoperability efforts within the field, making information sharing between platforms more reliable and straightforward. Similarly, offering native support for international e-learning standards presents an area of advancement that would propel the capacity for Learning Records interoperability.

### 4\.14 References

 1. Moodle Documentation. Logs. Available at: https://docs.moodle.org/402/en/Logs (last consulted on 2023-09-01).
 2. Moodle. Logstore xapi. Available at: https://moodle.org/plugins/logstore_xapi (last consulted on 2023-09-01).
 3. Moodle. Logstore trax. Available at: https://moodle.org/plugins/logstore_trax (last consulted on 2023-09-01).
 4. Moodle Documentation. Caliper. Available at: https://docs.moodle.org/dev/Caliper (last consulted on 2023-09-01).
 5. Rustici Software. Play xapi and cmi5 in Moodle. Available at: https://rusticisoftware.com/resources/play-xapi-and-cmi5-in-moodle/ (last consulted on 2023-09-01).
 6. Edx Read The Docs. Student event types. Available at: https://edx.readthedocs.io/projects/devdata/en/latest/internal_data_formats/tracking_logs/student_event_types.html (last consulted on 2023-09-01).
 7. Open Edx. xAPI realtime events. Available at: https://docs.openedx.org/projects/openedx-proposals/en/latest/architectural-decisions/oep-0026/xapi-realtime-events.html (last consulted on 2023-09-01).
 8. xAPI. Adopters. Available at: https://xapi.com/adopters/.
 9. ADL Initiative. Projects xAPI. Available at: https://adlnet.gov/projects/xapi/ .
10. Open Edx. Caliper realtime events. Available at: https://docs.openedx.org/projects/openedx-proposals/en/latest/architectural-decisions/oep-0026/caliper-realtime-events.html.
11. Canvas. xapi. Available at: https://canvas.instructure.com/doc/api/file.xapi.html (last consulted on 2023-09-01).
12. IMS Global. Instructure. Available at: https://site.imsglobal.org/certifications/instructure/canvas#cert_pane_nid_193191 (last consulted on 2023-09-01).
13. IMS Global. Blackboard Learn. Available at: https://site.imsglobal.org/certifications/anthology/blackboard-learn#cert_pane_nid_404018 (last consulted on 2023-09-01).
14. Desire2Learn. xapi. Available at: https://docs.datastreams.desire2learn.com/xapi/index.html (last consulted on 2023-09-01).
15. LearnDash. SCORM xAPI. Available at: https://www.learndash.com/support/docs/reporting/scorm-xapi/ (last consulted on 2023-09-01).
16. TalentLMS. How to import and track cmi5 content. Available at: https://help.talentlms.com/hc/en-us/articles/360014571774-How-to-import-and-track-cmi5-content (last consulted on 2023-09-01).
17. Chamilo. Website. Available at: https://chamilo.org/en/ (last consulted on 2023-09-01).
18. Google. Classroom API overview. Available at: https://support.google.com/edu/classroom/answer/6253304?hl=en&sjid=533248504110682389-EU (last consulted on 2023-09-01).
19. Google. Work Shared from the lesson video page shared work prompt. Available at: https://support.google.com/applieddigitalskills/answer/9798447?hl=en#zippy=%2Cwork-shared-from-the-lesson-video-page-shared-work-prompt (last consulted on 2023-09-01).
20. Microsoft. Track student progress in the Grades tab. Available at: https://support.microsoft.com/en-au/topic/track-student-progress-in-the-grades-tab-bc76ffde-bbf7-4db6-b443-735a07e32de0 (last consulted on 2023-09-01).
21. Microsoft. Education API overview. Available at: https://learn.microsoft.com/en-us/graph/education-concept-overview (last consulted on 2023-09-01).
