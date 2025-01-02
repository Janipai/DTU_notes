yellow box: activities
diamond: forking behaviour (soar gateways?)

circle nodes: places
squared nodes: transitions



## General instructions

The project has to be conducted in teams of 6 persons. The goal of the project is to show that each member of each group has achieved the [learning objectives of the course](https://kurser.dtu.dk/course/02269).

Each group has to choose one of the “project themes” mentioned below and construct their investigations starting from there. The scope of the project is not fixed so there is flexibility as long as the project covers the aspects of process mining discussed in the course. I encourage the involvement of external participants (the company you work on, an association you are part of, etc.) Projects will be associated with a difficulty multiplier that is used to scale the final grade of the project.

There is no limit on which tools can be used or on how to analyze the data. However, I expect that each group will investigate the data using both process mining tools (e.g., ProM, Apromore, Disco, Celonis) as well as more classical tools (e.g., Python scripts, Excel / charts).

In some of the project themes, there are some questions to be investigated and answered; however, this should be taken as a starting point for further explorative analyses. In particular, as discussed in the Process Mining Projects module, it is important that you formulate use cases and then verify them with the tools at your disposal.

Possible project tracks are:

1. Human behavior Analyze event logs referring to human behavior to understand worsening of dementia patients (difficulty multiplier: 1)
    - Dementia patients are typically old persons who are very repetitive in their behavior, therefore their daily tasks can be modeled using process mining-inspired techniques
    - Daily routines over the last period can be discovered (i.e., _control-flow discovery_) and verified against more recent behavior (i.e., _conformance checking_)
    - The project could extend existing methodologies to include new models and new techniques
    - Previous [MSc project on the topic](https://findit.dtu.dk/en/catalog/62df30baf91a1d54e4af4383) and scientific paper _[Do You Behave Always the Same? Let's Find Out](https://andrea.burattin.net/publications/2022-edba)_. The data used in the paper is availble at [https://doi.org/10.5281/zenodo.6632042](https://doi.org/10.5281/zenodo.6632042)
    - Data simulator of IoT-enabled environment here: [http://linac.compute.dtu.dk/](http://linac.compute.dtu.dk/).
2. DTU Analyze data from DTU's students curricula (difficulty multiplier: 1)
    - Recently, DTU prepared a database with data from 22086 students (with 327248 events) for Danmarks Statistik. The dataset is anonymized so it can be shared (dataset available here [https://dtudk-my.sharepoint.com/:x:/g/personal/andbur_dtu_dk/EexamyuXuJNCgnZZZQB1ISYBr5tFx3r9nBNOh7mWlZMueg?e=k1FLY0](https://dtudk-my.sharepoint.com/:x:/g/personal/andbur_dtu_dk/EexamyuXuJNCgnZZZQB1ISYBr5tFx3r9nBNOh7mWlZMueg?e=k1FLY0))
    - Looking at each study plan as a process and doing process mining on it can help reveal where the bottlenecks are, if certain prerequisites are not necessary, whether certain grades correlate with certain curriculum structure, etc
    - Data from the very interesting project DTU Course Analyzer ([https://github.com/SMKIDRaadet/dtu-course-analyzer](https://github.com/SMKIDRaadet/dtu-course-analyzer)) might be integrated too
3. Computer vision Use process mining on data processed from computer vision (difficulty multiplier: 1.1)
    - Many times, the execution of processes is monitored using camera, so events are not recorded in a structured way, but in form of video stream
    - To perform this analisys it is necessary to first process the camera data, to identify the activity/case id, and then give it to a process mining component
    - Ideally the processing of video data should happen in real time, but this is a challenge in itself (cf. [book chapter on the subject](https://andrea.burattin.net/publications/2022-pmh), [tool paper](https://andrea.burattin.net/publications/2023-simpa))
    - Previous [MSc project on the topic](https://findit.dtu.dk/en/catalog/6216242583fe41235e4fb8af) and [paper 1 on the topic](https://link.springer.com/chapter/10.1007/978-3-031-41623-1_12), [paper 2 on the topic](https://ceur-ws.org/Vol-2420/papeDT15.pdf)
4. RPA-Microsoft Real-life project on RPA recommendation with Microsoft (difficulty multiplier: 1.1)
    - Automation of repetitive tasks can be achieved with Robotic Process Automation (RPA) using scripts that encode fine grained interactions with software applications on desktops and the web
    - Several tools for RPA exists, and their leverage some notion of _connector_. Choosing the right connector for suggestion can be a non-trivial task
    - Analyzing the repetitive behavior of a person and how they interact with the system can lead to the recommendation connectors
    - The project has been explored in a [paper](https://andrea.burattin.net/publications/2023-data) and in a [MSc project](https://findit.dtu.dk/en/catalog/630177bde67566132565e3e7) and the idea of the project is to continue it by exploiting novel dimensions and new process modelling paradigms (e.g., DCR)
    - Data is accessible on [Microsoft's GitHub](https://github.com/microsoft/50BusinessAssignmentsLog) and interactions with them might be possible
5. Analysis Analysis of a real event log, to extract some knowledge out of it. In this case, you can decide to analyze a log coming from your own company/organization or you can use a log publicly available. Examples:
    - Analysis of a BPI challenge event log (difficulty multiplier: ~0.8):
        - [https://icpmconference.org/2019/icpm-2019/contests-challenges/bpi-challenge-2019/](https://icpmconference.org/2019/icpm-2019/contests-challenges/bpi-challenge-2019/)
        - [https://www.win.tue.nl/bpi/2018/challenge.html](https://www.win.tue.nl/bpi/2018/challenge.html)
        - [https://www.win.tue.nl/bpi/2017/challenge.html](https://www.win.tue.nl/bpi/2017/challenge.html)
        - [https://www.win.tue.nl/bpi/2016/challenge.html](https://www.win.tue.nl/bpi/2016/challenge.html)
        - [https://www.win.tue.nl/bpi/2015/challenge.html](https://www.win.tue.nl/bpi/2015/challenge.html)
        - Please note that in these cases, you can also have access to the reports that people contributed as solutions. You are very much encouraged to read and study them and therefore you need to explain (in the written report) how your analysis is improving all these solutions
    - Analysis of a set of real event logs (see [https://data.4tu.nl/search?search=%22event+logs%22](https://data.4tu.nl/search?search=%22event+logs%22) or [https://www.tf-pm.org/resources/logs](https://www.tf-pm.org/resources/logs)) like the NASA Crew Exploration Vehicle (CEV) Software Event Log. Note not all of them have business questions associated; therefore, you might need to do some research to understand where the logs are coming from and what is relevant in the specific domains (difficulty multiplier: 0.9-1).
    - Construct and analyze a non-trivial log (i.e., a log not already in the XES form). Example of these could be the MIMIC (Medical Information Mart for Intensive Care, [https://mimic.mit.edu/](https://mimic.mit.edu/), in this case see also [MIMICEL](https://physionet.org/content/mimicel-ed/2.1.0/)) or event logs referring to the edits on a Wikipedia website or the commits on a GitHub repository (difficulty multiplier: 1-1.3).
    - Another example of logs that can be constructed and analyzed are the NASA APOLLO Program missions, see [https://www.nasa.gov/wp-content/uploads/2023/04/sp-4029.pdf](https://www.nasa.gov/wp-content/uploads/2023/04/sp-4029.pdf) (difficulty multiplier: 1-1.3).
6. LLMs Study integration of LLM in the scope of process mining. Examples of projects:
    - Structuring natual language description of activities into event logs. This project has already been explored in a [MSc project](https://findit.dtu.dk/en/catalog/6626fc44d752221afd23fd75) (difficulty multiplier: 0.9-1.1).
    - Refine how LLMs can benefit from process mining research. This project has already been explored in a paper ([working copy of the paper](https://dtudk-my.sharepoint.com/:b:/g/personal/andbur_dtu_dk/EXTha-GP7ZRAhiRrO3AJ3SgBLkqpGkVBcjgnckIYg5PHZA?e=Xfik4A), [report](https://arxiv.org/abs/2409.09191)) that will be presented soon at ICPM (difficulty multiplier: 1.1-1.3).
    - Discretize the NASA APOLLO Program mission timelines, see [https://www.nasa.gov/wp-content/uploads/2023/04/sp-4029.pdf](https://www.nasa.gov/wp-content/uploads/2023/04/sp-4029.pdf) to construct a log and analyze it (difficulty multiplier: 1-1.3).
7. Development Development of a process mining-related software. Examples of projects:
    - An extension of Minecraft to explore an event logs. I started implementing a similar approach just for visualizing process models as BPMN, see [https://github.com/delas/bpmn2minecraft](https://github.com/delas/bpmn2minecraft) (difficulty multiplier: ~1.1)
    - Translation of existing algorithms into online fashion and implement them in [Beamline](https://www.beamline.cloud), see [https://www.beamline.cloud](https://www.beamline.cloud/) (difficulty multiplier: ~1.3)
    - A library to do process mining operations, or an extension of existing libraries (e.g., [https://www.bupar.net](https://www.bupar.net), [http://pm4py.org/](http://pm4py.org/)) (difficulty multiplier: 0.8-1)
    - Go through [Andrea's publications page](https://andrea.burattin.net/publications/), look for something that sounds interesting, and improve it!

**IMPORTANT:** Before starting the work on the project, it is NECESSARY that the teacher approves the project, to ensure that the amount of work is proportionate to the group size. To ensure an even distribution of the project among the groups, please report (and keep updated) the spreadsheet at [https://dtudk-my.sharepoint.com/:x:/g/personal/andbur_dtu_dk/Ef9Qwtz_W_ZDq2mnWkpqDV8BRoK3h1Fg4c04SBYoJFcoCw?e=xIarmM](https://dtudk-my.sharepoint.com/:x:/g/personal/andbur_dtu_dk/Ef9Qwtz_W_ZDq2mnWkpqDV8BRoK3h1Fg4c04SBYoJFcoCw?e=xIarmM).

The deliverable has to include a report where each group describes what they have done in a critical way (i.e., motivate all the decisions and document and explain all results); all the code produced; the slides of the presentation that will be given. Further instruction below.
![[Pasted image 20241010005811.png]]

![[Pasted image 20241010005851.png]]

## What to submit

The final submission comprises a group submission consisting of one `.zip` file containing (please, be precise with the naming of each element):

1. A report in a file called **`report.pdf`** (the report has to be in PDF) which should be structured according to the document `demo-report.pdf` (see [https://learn.inside.dtu.dk/d2l/le/content/215840/viewContent/877257/View](https://learn.inside.dtu.dk/d2l/le/content/215840/viewContent/877257/View)):
    - Has to be **maximum** 8 pages long (only the first 8 pages of the PDF will be printed, so no cover/front page/table of content);
    - Has to provide a complete description of the results, used tools, and why the group chose them. Potential and results have to be commented and discussed in details;
    - Has to provide the work distribution among project members
        - **IMPORTANT:** For each person the workload must be indicated. An even workload of 1 indicates that everyone contributed the same. A workload of 0.5 for one person, while the others have a workload of 1, indicates that the person contributed half. **The workload will be used to weight the final grade for each member.** The workload not necessarily reflects the number of classes/lines of code or pages/algorithms written by the person, the workload is left for your judgement (for example, one person working on a very complicated alorithm can have the same workload of a person working on many simpler algorithms).
2. The final presentation in a file called **`presentation.pdf`** (the presentation has to be exported in PDF).
3. In case the group wrote some software (e.g., processing scripts in Python/R/... or entire software in Java/C#/...), the complete source code should be in a file called **`source.zip`**.

## The intermediate presentation

On 2024-11-13, there will be a first group presentation, where each group will be allotted about 10/15 minutes (exact time will follow, depending on how many groups want to participate) to present the status of their project. The goals of this presentation are:

- Practice with presentation and dealing with time constraints as well as questions (that is why it is important to carefully prepare this presentation);
- Receive feedback from instructors as well as from other students (that is why it is important to carefully prepare this presentation) and the project stakeholders;
- Get inspiration from other groups' work (that is why it is important to attend and be involved in the discussions).

This presentation is not part of the grading (it is up to you get the most out of this opportunity).

## The final presentation

Each group will need to present their project in a ~10 minutes (exact time will follow) long presentation (I will keep the timing). During the presentation, it is required that:

- Each member of the group presents something;
- The presentation has not to be a “slides” version of the report. The focus has to be on the elements that are better explained in person. Still, it has to cover all elements of the project, including:
    - Domain description;
    - Problem description;
    - Method used to solve the problem;
    - Results;
    - Reflections on the project.
- Each member must be able to answer **any** questions about any part of the project (so all members must be 100% familiar with every part of the project);
- The presentation _can_ include a brief live demonstration of the tools if you think this can contribute to the better understanding of the project.

## Assessment

The final assessment is based on the group work grade (multiplied by the difficulty multiplier and the individual workload), the group presentation and the individual part. See the Course Content document for further information.

![[Pasted image 20241010010452.png]]

![[Pasted image 20241010010504.png]]

![[Pasted image 20241010010520.png]]

![[Pasted image 20241010010852.png]]