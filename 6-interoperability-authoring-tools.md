[Interoperability of Learning Records: State-of-the-Art in 2023](/)

## 6\. Interoperability of Authoring tools

Authoring tools are used by training organisations to create a wide range of interactive learning content while leveraging the advantages of learning standards like xAPI, SCORM, and cmi5.

In this part, we have analysed the various authoring tools available on the market. For each authoring tools, we have gathered as much information as possible about their compatibility with the major Learning Records standards (xAPi, SCORM, IMS Caliper, cmi5) from their website, support center (forum, knoledge base) or dvelopper documentation when available.

The compatibility of the authoring tools with the main learning records standards are available in the table below.

**Table 6.1. Compatiblity of authoring tools with Learning Records standards**

| Name | Link | Free | xAPI | IMS Caliper | SCORM | cmi5 |
|------|------|------|------|-------------|-------|------|
| Articulate Storyline 360 | [Link](https://articulate.com/360/storyline) | No (Free Trial) | [Yes](https://articulate.com/support/article/articulate-storyline-is-scorm-conformant) | No | [Yes](https://articulate.com/support/article/articulate-storyline-is-scorm-conformant) | [Yes](https://articulate.com/support/article/articulate-storyline-is-scorm-conformant) |
| Adobe Captivate | [Link](https://www.adobe.com/products/captivate.html) | No (Free Trial) | [Yes](https://helpx.adobe.com/captivate/classic/learning-management-system-lms.html#:~:text=Adobe%20Captivate%20Classic%20provides%20you,published%20package%20to%20an%20LMS) | No | [Yes](https://helpx.adobe.com/captivate/classic/learning-management-system-lms.html#:~:text=Adobe%20Captivate%20Classic%20provides%20you,published%20package%20to%20an%20LMS) | [Possible](https://community.adobe.com/t5/captivate-discussions/adobe-captivate-support-for-cmi5/m-p/8599029) |
| H5P | [Link](https://h5p.org/) | Yes | [Yes](https://h5p.org/documentation/x-api) | No | No, but can be [converted](https://translate-h5p.tk/scorm-h5p/) | No |
| hihaho | [Link](https://hihaho.com/) | No (Free Trial) | [Yes](https://support.hihaho.com/en/articles/5695482-xapi-tin-can-api-guide) | No | [Yes](https://support.hihaho.com/en/articles/5694732-exporting-your-video-as-a-scorm-package) | No |
| iSpring | [Link](https://www.ispringsolutions.com/) | No (Free Trial) | [Yes](https://www.ispringsolutions.com/blog/what-is-xapi) | No | [Yes](https://www.ispringsolutions.com/blog/scorm-course) | [Yes](https://www.ispringsolutions.com/blog/ispring-now-supports-cmi5-the-next-generation-of-scorm) |
| Lectora authoring tool | [Link](https://www.lectoraonline.com/) | No (Free Trial) | [Yes](https://blog.elblearning.com/drive-better-learning-outcomes-using-xapi-data) | No | [Yes](https://www.elblearning.com/create-learning/lectora-features) | [Yes](https://www.elblearning.com/create-learning/lectora-features) |
| Alchemer (formerly SurveyGizmo) | [Link](https://www.alchemer.com/) | No (Free trial) | [Yes](https://help.alchemer.com/help/lmslrs-integration) | No | No | No |
| Lumi | [Link](https://app.lumi.education/) | Yes | [Yes](https://docs.lumi.education/advanced-usage/completion-tracking) | No | [Yes](https://wiki.ubc.ca/images/f/f6/Lumi_Guide_-_H5P_SCORM_Object.pdf) | No |

### 6\.1 Articulate Storyline 360

[Articulate Storyline 360](https://articulate.com/360/storyline) is a powerful software tool which allows users to create interactive, engaging e-learning courses. It is widely recognized for its user-friendly interface and its ability to create highly customized learning experiences. It is an industry standard and highly suitable for corporate training. While it isn't available for free, it does support xAPI, SCORM, and cmi5, making it compatible with most LMS.

Articulate Storyline 360 is compatible with xAPI. This allows the software to track and store a wide range of eLearning experiences. This means that Storyline 360 can capture data about learner activities, both online and offline, and store this data in a LRS.

Articulate Storyline 360 is [SCORM conformant](https://articulate.com/support/article/articulate-storyline-is-scorm-conformant), supporting SCORM 1.2 through SCORM 2004 4th Edition. Thus, it can communicate with SCORM-compliant LMS to record and track learners' progress and completion of online learning activities.

Articulate Storyline 360 does not support IMS Caliper.

Articulate Storyline 360 also conforms to the cmi5 specification.

### 6\.2 Adobe Captivate

[Adobe Captivate](https://www.adobe.com/products/captivate.html) is a versatile tool for creating interactive eLearning and HTML content. It supports VR and responsive eLearning projects and quizzes. It doesn't have a free version, but it is compatible with xAPI, and SCORM, and possibly with cmi5.

Adobe Captivate supports [xAPI](https://helpx.adobe.com/captivate/classic/learning-management-system-lms.html#:~:text=Adobe%20Captivate%20Classic%20provides%20you,published%20package%20to%20an%20LMS), allowing users to track and store comprehensive learning data from multiple learning activities across various platforms. The xAPI data can be sent to a LRS for further processing and analysis, making it a flexible and powerful tool for capturing learning data.

The software also conforms to SCORM standards. As a SCORM-compliant tool, Adobe Captivate can communicate with SCORM-friendly LMS, recording completion, time, and pass/fail results. It can also track both online and offline learning activities.

Adobe Captivate does not support IMS Caliper.

There's possible support for [cmi5](https://community.adobe.com/t5/captivate-discussions/adobe-captivate-support-for-cmi5/m-p/8599029) in Adobe Captivate. While not explicitly documented, community discussion indicates that it might be possible to adapt output for compatibility with the cmi5 standard.

### 6\.3 H5P

[H5P](https://h5p.org/) is an open-source framework that allows users to create, share, and reuse rich interactive HTML5 content in their web browsers. It provides an easy-to-use interface where no coding experience is required to build and design a variety of engaging learning activities such as presentations, videos, and quizzes. It's free and supports xAPI, but not SCORM nor cmi5.

H5P is compatible with xAPI, which allows to track and guide individual learners' experiences. When learners interact with H5P content, their actions (like responses to questions, scores, and video playback progress) can be captured and formatted as xAPI statements. These statements conform to the "Actor-Verb-Object" structure (as you mentioned in previous queries), which can also include additional information about the resulting activity or its context. H5P itself does not store learning records. However, with the integration of xAPI, these learning records (in the form of xAPI statements) can be sent to and stored in an external LRS. This requires H5P being configured with the LRS endpoints and authentication information. Once correctly set up, H5P can send learner interaction information as xAPI messages to the LRS where these records are stored for analytics and reporting.

[H5P's approach](https://h5p.org/documentation/x-api) is to generate xAPI statements and make them available through events in JavaScript.

To listen for xAPI events a developer adds:

```js
H5P.externalDispatcher.on('xAPI', eventHandler);
```

Where the xAPI statement is to be found in event.data.statement. The event will be an XAPIEvent with many functions that makes working with it easier - see the API reference.
Example
To try this out type the following in your browser's console when using an H5P object on a website:

```js
H5P.externalDispatcher.on('xAPI', function (event) {
    console.log(event.data.statement);
});
```

You should now see xAPI statements in your console.
If you, for instance, need to do something if the user gets full score you may do something like this:

```js
H5P.externalDispatcher.on('xAPI', function (event) {
    if (event.getScore() === event.getMaxScore() && event.getMaxScore() > 0) {
        console.log('do something useful here');
    }
});
```

Since H5P is a plugin for publishing tools H5P does not include its own LRS integration. Instead, H5P generates the statements and makes them available for the publishing platform so that the publishing platform may use its own LRS integration to send H5P's statements to an LRS.

Although H5P does not natively support SCORM, it is still possible to convert H5P content into SCORM packages using external tools or platforms. This means that H5P interactive content can still be packaged and used on SCORM-compliant LMS albeit through conversion.

The [scorm-h5p-wrapper](https://github.com/sr258/scorm-h5p-wrapper)github project is a tool that enables users to package H5P files into SCORM format. This utility essentially acts as a bridge to make H5P content compatible with any Learning Management System (LMS) that supports SCORM, even if the LMS lacks a built-in H5P module.

The tool can also send scores from the H5P content to the LMS through SCORM, facilitating the tracking of learner progress. Other benefits of packaging H5P content into SCORM include reduced reliance on external sites (addressing both privacy concerns and availability issues), the ability to use H5P content types not available on your LMS, and the assurance that your content remains unchanged, immune to any updates in H5P core or libraries.

However, there are also a few drawbacks while using scorm-h5p-wrapper. These include lack of caching H5P library files across content, inability to use the H5P Editor for quick changes, no automatic updates from H5P libraries or the core, and slightly larger packages due to the inclusion of the h5p-standalone library.

Therefore, using the scorm-h5p-wrapper will be beneficial only under the right circumstances. It is suggested that if the LMS has a built-in H5P plugin, it is better to stick with the traditional upload process unless compelling reasons exist to package H5P content into SCORM.

H5P does not support IMS Caliper.

H5P also does not natively support the cmi5 specification.

### 6\.4 Lumi

[Lumi](https://app.lumi.education/) is an open-source software platform for interactive lesson delivery, formative assessment and analytics. It focuses on building interactive instructional materials, particularly with the use of H5P content and quizzes. Lumi is free, supports xAPI, and learning object created with Lumi (in H5P) can be exported as SCORM object.

Unlike all other H5P systems, Lumi doesn't require you to have access to a Learning Management System (LMS) like Moodle or a Content Management System (CMS) like WordPress or Drupal. You can simply create interactive content in your desktop environment and share it with your students by exporting it as a HTML file.

Lumi is compatible with the [xAPI](https://docs.lumi.education/advanced-usage/completion-tracking) standard. This standard enables Lumi to record and track a broad range of learning experiences. Lumi H5P client is capable of sending a message to the server when the user has completed a content object. This includes the time when this occured, how long the content was open, the achieved score and the maximum score. While technically this message is derived from a xAPI statement generated by the content types, it is not the same as xAPI and is a completely separate system that co-exists with xAPI and a potential LRS. You can enable completion tracking and xAPI tracking indepedently. To capture all xAPI statements, Lumi users either have to inject their own xAPI capturing JavaScript or use the xAPI capabilities of the H5PPlayerComponent in the webcomponent package (or the corresponding functionality in the React package).

Lumi can create [SCORM](https://wiki.ubc.ca/images/f/f6/Lumi_Guide_-_H5P_SCORM_Object.pdf) package.

Lumi does not explicitly support IMS Caliper.

There is no evidence to suggest that cmi5 is supported by Lumi.

### 6\.5 hihaho

[Hihaho](https://hihaho.com) is a universal interactive video creation platform enabling users to create engaging learning experiences. It's known for simple yet effective video editing tools, which require no special technical skills. It doesn't have a free version.

Hihaho is compatible with the [xAPI](https://support.hihaho.com/en/articles/5695482-xapi-tin-can-api-guide) standard. The video will send several commands through xAPI to the LRS. Hihaho uses the ‘course’ and ‘video’ xAPI recipes. Here are a few ecamples of statements generated by Hihaho video:

| Command | Description | Recipe | Verb |
|---------|-------------|--------|------|
| I attempted a session for an eLearning course | When the video plays for the first time, this xAPI command will be sent. | course | http://adlnet.gov/expapi/verbs/attempted |
| I answered an eLearning course question | When an answer is given to a question, an xAPI command will be sent. | course | http://adlnet.gov/expapi/verbs/answered |
| I completed a session for an eLearning course | When the viewer has viewed the entire video, this xAPI command will be sent. | course | http://adlnet.gov/expapi/verbs/completed |
| I passed an eLearning course | When the viewer has scored more than the minimum percentage he needs to pass the video, this will be sent. You will find these settings next to the xAPI settings under the 'Reporting' tab. | course | http://adlnet.gov/expapi/verbs/passed |
| I failed an eLearning course | When the viewer has not met the minimum percentage needed to succeed, this will be sent. | course | http://adlnet.gov/expapi/verbs/failed |

The software also supports the [SCORM](https://support.hihaho.com/en/articles/5694732-exporting-your-video-as-a-scorm-package) standard, allowing it to interoperate with SCORM-compliant LMS. Hihaho's SCORM file includes the following data of each viewer session:

* Started / Not started
* Finished / Not finished
* Scores of each question
* Total score of the video

Hihaho does not currently support the IMS Caliper standard.

Hihaho does not support cmi5.

### 6\.6 iSpring

[iSpring](https://www.ispringsolutions.com/) is a suite of eLearning authoring tools that enable the creation of interactive courses, quizzes, dialog simulations, screencasts, and more. The software is recognized for its seamless PowerPoint integration and for allowing comprehensive SCORM packaging for LMS.

iSpring allows tracking of a wide range of learning experiences with [xAPI](https://www.ispringsolutions.com/blog/what-is-xapi).

iSpring is fully compatible with [SCORM](https://www.ispringsolutions.com/blog/scorm-course). This allows learning content from iSpring to be uploaded to any SCORM-compliant LMS. The SCORM compatibility ensures that learning progress, completion statuses, and other learning analytics are tracked and stored systematically.

iSpring does not offer support for the IMS Caliper standard.

iSpring has full support for the [cmi5](https://www.ispringsolutions.com/blog/ispring-now-supports-cmi5-the-next-generation-of-scorm) standard.

### 6\.7 Lectora authoring tool

[Lectora authoring tool](https://www.lectoraonline.com/)is a leading authoring software that provides an intuitive, collaborative environment for creating interactive, SCORM-conformant content. Well-known for its wide range of functionality and ease-of-use, Lectora empowers users to create compelling, engaging eLearning content.

Lectora is compatible with [xAPI](https://blog.elblearning.com/drive-better-learning-outcomes-using-xapi-data).

Lectora also supports SCORM, ensuring that courses built using the tool can communicate effectively with SCORM-compliant LMS.

Lectora does not support IMS Caliper.

Lectora is compatible with the [cmi5](https://www.elblearning.com/create-learning/lectora-features) standard.

### 6\.8 Alchemer

[Alchemer](https://www.alchemer.com/, formerly known as SurveyGizmo, is a comprehensive survey platform enabling businesses to gather, analyze, and act on data. It provides tools for building, distributing, and analyzing survey results.

Alchemer offers compatibility with [xAPI](https://help.alchemer.com/help/lmslrs-integration). This feature facilitates the exchange of data about learner activity and experiences between Alchemer and learning management systems (LMSs). This supports the collection, storage, and retrieval of learning records, irrespective of where and how learning has happened.

Alchemer does not support the SCORM standard.

Alchemer does not support IMS Caliper.

Alchemer does not support the cmi5 standard.

### 6\.9 References

 1. Articulate Support. Articulate Storyline 360 is SCORM Conformant. Available at: https://articulate.com/support/article/articulate-storyline-is-scorm-conformant (last consulted on 2023-09-08).
 2. Adobe Help Center. Learning Management System (LMS). Available at: https://helpx.adobe.com/captivate/classic/learning-management-system-lms.html (last consulted on 2023-09-08).
 3. Adobe Community. Adobe Captivate support for cmi5. Available at: https://community.adobe.com/t5/captivate-discussions/adobe-captivate-support-for-cmi5/m-p/8599029 (last consulted on 2023-09-08).
 4. H5P. Documentation xAPI. Available at: https://h5p.org/documentation/x-api (last consulted on 2023-09-08).
 5. H5P. xAPI support in H5P. Available at: https://h5p.org/documentation/x-api (last consulted on 2023-09-08).
 6. H5P. H5P to SCORM. Available at: https://translate-h5p.tk/scorm-h5p/ (last consulted on 2023-09-08).
 7. H5P. Website. Available at: https://h5p.org/ (last consulted on 2023-09-08).
 8. H5P. Node discussion. Available at: https://h5p.org/node/1086708 (last consulted on 2023-09-08).
 9. Github. Scorm H5P Wrapper. Available at: https://github.com/sr258/scorm-h5p-wrapper (last consulted on 2023-09-08).
10. Lumi Education. Completion Tracking. Available at: https://docs.lumi.education/advanced-usage/completion-tracking (last consulted on 2023-09-08).
11. UBC Learning Design. Lumi Guide - H5P SCORM Object. Available at: https://wiki.ubc.ca/images/f/f6/Lumi_Guide\_-\_H5P_SCORM_Object.pdf (last consulted on 2023-09-08).
12. Github. Lumi project. Available at: https://github.com/Lumieducation/Lumi (last consulted on 2023-09-08).
13. HiHaHo Support. xAPI (Tin Can API) guide. Available at: https://support.hihaho.com/en/articles/5695482-xapi-tin-can-api-guide (last consulted on 2023-09-08).
14. HiHaHo Support. Testing a SCORM package in a LMS. Available at: https://support.hihaho.com/en/articles/5833550-testing-a-scorm-package-in-a-lms (last consulted on 2023-09-08).
15. HiHaHo Support. Exporting your video as a SCORM package. Available at: https://support.hihaho.com/en/articles/5694732-exporting-your-video-as-a-scorm-package (last consulted on 2023-09-08).
16. iSpring. What is xAPI. Available at: https://www.ispringsolutions.com/blog/what-is-xapi (last consulted on 2023-09-08).
17. iSpring. What is a SCORM course. Available at: https://www.ispringsolutions.com/blog/scorm-course (last consulted on 2023-09-08).
18. iSpring. iSpring now supports cmi5, the next generation of SCORM. Available at: https://www.ispringsolutions.com/blog/ispring-now-supports-cmi5-the-next-generation-of-scorm (last consulted on 2023-09-08).
19. ELB Learning. Drive Better Learning Outcomes Using xAPI Data. Available at: https://blog.elblearning.com/drive-better-learning-outcomes-using-xapi-data (last consulted on 2023-09-08).
20. ELB Learning. Lectora Features. Available at: https://www.elblearning.com/create-learning/lectora-features (last consulted on 2023-09-08).
21. ELB Learning. Lectora product. Available at: https://www.elblearning.com/create-learning/lectora (last consulted on 2023-09-08).
22. Alchemer Support. LMS/LRS Integration. Available at: https://help.alchemer.com/help/lmslrs-integration (last consulted on 2023-09-08).
