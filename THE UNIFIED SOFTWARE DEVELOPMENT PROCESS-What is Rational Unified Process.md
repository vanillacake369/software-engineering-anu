# THE UNIFIED SOFTWARE DEVELOPMENT PROCESS :: What is Rational Unified Process

# Contents

---

# Intro

“쉽게 배우는 소프트웨어공학(김치수 저)” 공부 중 UP모델에 관해 이해가 잘 되지 않아 구글링을 하던 중 좋은 자료가 있어 기록해본다.

어떠한 목적으로 나오게 되었는지 궁금했고, 형상(변화)관리,프로젝트 관리, 환경 점검 등 기본 SDLC와 다른 점들이 이해가 되지 않았다.

책에서는 각 Phase마다 다음과 같은 활동을 한다고**”만”** 나와있을 뿐, 하나의 Cycle에서의 활동 및 영역이 무엇인지는 다루지를 않는다.

아래를 보며 Phase에 대한 정확한 이해와 Cycle에서 각 도메인에 대한 이해를 해보자.

---

# What is it?

The Unified Process (UP), or Unified Software Development Process, is a iterative and incremental software development framework from which a customized process can be defined. The framework contains many components and has been modified a number of times to create several variations. The most popular variations include the Rational Unified Process (RUP) and the Open Unified Process (OpenUP). The framework has several key characteristics which seem to carry across all variations (as far as I can tell).

The key characteristics of the Unified Process are: [5]

- It is an iterative and incremental development framework
- It is architecture-centric with major work being done to define and validate an architectural design for most coding is done
- It is risk-focused and emphasizes that highest-risk factors be addressed in the earliest deliverables possible
- It is use-case and UML model driven with nearly all requirements being documented in one of those forms

In general, the Unified Process is built around the idea of incorporating six specific best practices into a configurable process framework. Those best practices are:

1. Develop Software Iteratively
2. Manage Requirements
3. Use Component-based Architectures
4. Visually Model Software
5. Verify Software Quality
6. Control Changes to Software

---

# History

Much of the concepts in the Unified Process began with work Ivar Jacobson did at Ericsson in the 1960's. Jacobson went out on his own in 1987, codified his earlier work into what became the Objectory Process, and started the Objectory AB company to sell the process. After a number of years further developing the Objectory process, Jacobson released the book Object-Oriented Software Engineering in 1995 which described the Objectory Process in detail.

In 1996 Rational Software acquired the Objectory Process and company.[1] Jacobson worked at Rational and teamed up with Grady Booch and Jim Rumbaugh and together they spent the next several years further developing the Objectory Process (now known as the Rational Objectory Process) and the Unified Method (which later became UML). In 1998, Rational changed the name from the Rational Objectory Process to the Rational Unified Process. However, because RUP was the trademarked property of Rational, further work by the software and academic community usually referred to just the Unified Process in order to avoid trademark issues. And by 1999, the first book to describe the generic Unified Process was written by Jacobson, Booch, and Rumbaugh.

IBM acquired Rational Software in 2003, and in 2005 donated the core of the Rational Process to the Eclipse Foundation open-source community. [7]

There were originally just five Disciplines in the Unified Process, but over the years that has been expanded to where there are now up to nine.

---

# The Components of the Unified Process

The Unified Process framework is made up of the following components:

- Cycles
- Phases
- Iterations
- Disciplines (also known as Workflows)
- Activities
- Artifacts
- Workers

The disciplines are:

- Business Modeling
- Requirements
- Analysis and Design
- Implementation
- Testing
- Deployment
- Configuration and Change Management
- Project Management
- Environment

The four phases are:

- Inception phase
- Elaboration phase
- Construction phase
- Transition phase

Each cycle defines a new major version of the software being developed. Each cycle is broken into four different phases, which may have multiple iterations within the phase. Each iteration results in an incremental version of the software. Across the cycles, phases, and iterations; work from different disciplines is undertaken by Workers (think of these as project roles). This work takes the form of specific activities with a discipline that result in specific artifacts (for example, a Create Work Breakdown Structure activity with the Project Management Discipline, which results in a WBS artifact).

Each phase is concluded when a measurable milestone has been reached and is followed by a go / no-go decision by the project team on whether to move forward with the next phase.

**It is important to note that although different amounts of work from each discipline may occur in each phase or iteration, work from all disciplines occurs in every phase.**

The UP framework is commonly visualized in ways such as the graphic below (from the Wikimedia Commons).

![Development-iterative.gif](THE%20UNIFIED%20SOFTWARE%20DEVELOPMENT%20PROCESS%20What%20is%20R%206a247415304144a79af39664e6f7e655/Development-iterative.gif)

---

# The Disciplines

## Business Modeling

The Business Modelling discipline focuses on efforts to understand the organization, its processes, and the problem domain. The discipline focuses on understanding the following factors and how they may impact or relate to the software being considered: [4]

- Enterprise business rules
- Enterprise business process model
- Enterprise domain model
- Enterprise mission statement
- Enterprise vision
- Organization model

## Requirements

The requirements discipline in RUP is like the requirements discipline in pretty much every other software process. The main difference is that RUP requirements are highly focused in the form of UML models and Use Cases (both diagrams and descriptions).

## Analysis and Design

The Analysis and Design discipline would be better named the Solution Analysis and Design discipline in my opinion. This is because the requirements are analyzed from a solution design perspective, rather than a requirements analysis perspective. Specific activities that are part of this discipline include: [4]

- Understanding and analyzing the requirements for the system
- Defining a candidate architecture for a system
- Constructing a proof-of-concept or prototype to validate a candidate architecture
- Design of components, services, and/or modules
- Design of interfaces (network, user, and databases)

## Implementation

The Implementation discipline consists of coding, unit testing, and integration of the software.

## Testing

The Testing discipline is focused on quality assurance of the software being released in that cycle or iteration. It includes such activities as: [4]

- Planning test efforts
- Creating test cases
- Running tests
- Reporting defects

## Deployment

The Deployment discipline is focused on planning the deployment of, and actually deploying, the software that is being completed that cycle, phase or iteration.  It includes such activities as:[4]

- Planning the deployment
- Developing support and operations materials
- Planning alpha, beta, and pilot testing efforts
- Deploying the software
- Training end users
- Managing acceptance testing efforts

## Configuration and Change Management

The Configuration and Change Management discipline is focused on managing change to the project’s work products.  This includes such activities as: [4]

- Managing change requests
- Setting up the Change Management process and environment
- Planning configuration control
- Monitoring and reporting the configuration status
- Managing baselines and releases

## Project Management

The Project Management discipline is focused on standard project management activities such as: [4]

- Managing project staff
- Stakeholder coordination and management
- Managing project risks
- Project estimating, planning, and scheduling
- Iteration planning
- Project initiation and close-out

## Environment

The Environment discipline is focused on supporting the overall project and development efforts through managing environmental factors such as:

- Processes
- Standards
- Tools (hardware, software, etc.)

---

# The Phases

## Inception Phase

The Inception Phase is the part of the framework when the why of the development effort is defined. This includes such activities as:

- Defining the business case
- Creating a vision document with core requirements, features, and constraints
- Creating an initial risk assessment
- Creating early use cases (10-20% complete, mostly use-case models)
- Creating a initial project plan
- And the creation of one or more prototypes (especially architectural prototypes)

The milestones (that together comprise the Lifecycle Objectives Milestone) that show completion of the Inception phase are:

- Stakeholder agreement on business case, scope, and project cost and schedule estimates
- Agreement that the content of the primary use cases is an accurate representation of what the software will deliver (at a high level)
- That the final prototypes are sufficient indications of the correct future development goals

## Elaboration Phase

The Elaboration Phase is the part of the framework when more detailed analysis and planning are undertaken to better understand the problem domain, develop a more concrete project plan, identify and eliminate the high-risk elements of the effort, and to establish a solid architectural foundation for the software to be developed.  The goal is to develop a "mile wide and inch deep" view of the system to be developed. [2]

The specific activities of this phase include:

- The identification of all actors and use cases, with most use cases having been defined to at least 80% completion (use-case descriptions rather than models)
- Supplementary requirements detailing the non-functional requirements and any requirements not related to a use case are completed
- A Software Architecture Description has been completed
- The business case and risk lists have been updated with higher-confidence information
- The project and development plans have been defined to at least a level that shows all iterations and the evaluation criteria for each iteration
- An executable architecture prototype has been created and approved for use (this may involve creating more than one)
- A preliminary user manual has been created (optional)

The milestones (that together comprise  the Lifecycle Architecture Milestone) that show completion of the Elaboration phase are:

- The product vision is stable and approved
- The product architecture is stable and approved
- The executable architecture prototype shows that the major risk elements have been identified and credibly resolved
- The project and development plans sufficiently detailed, accurate, and credible
- All stakeholders agree that the vision can be achieved is the project and development plans are executed with the architecture specified

## Construction Phase

The Construction Phase is the part of the framework where software development, integration, and testing takes place. Because of the emphasis on component-based architectures and the significant attention paid to the architectural plan in the Inception and Elaboration phases, it should be possible to initiate multiple Construction Phases within a single cycle if the software to be developed is complex enough to support multiple discreet components.

The specific activities of this phase include:

- The software is built, integrated, and tested
- The user manuals have been created (or updated)
- The details of the software developed are documented and ready to be provided to end users or support staff (including changes, etc.)

The milestones (that together comprise  the Initial Operational Capability Milestone) that show completion of the Construction phase are:

- The software product is stable and mature enough to be deployed to end users
- All stakeholders are ready to transition to the new / updated software
- Actual versus planned expenditures are still acceptable enough to move forward with the project

The outcome of the construction phase should be a product that is ready to put into the hands of end-users in at least a beta release state.

## Transition Phase

The Transition Phase of the framework is where the software is deployed to end users and is essentially a broad beta test of the application. Users begin to use the new software, issues are identified and potentially corrected, and any features that were delayed are finished and deployed. The transition phase can include multiple iterations of the software, including beta releases, bug fixes, and enhancements.

The specific activities of this phase include:

- beta testing or  by end users to validate the new software against user expectations
    
    user acceptance testing
    
- Parallel operation with legacy systems (if in existence) that will be replaced
- Operational databases are converted (if necessary)
- Users and maintainers of the software are fully trained
- The software is fully rolled-out

The milestones (that together comprise  the Product Release Milestone) that show completion of the Transition phase are:

- Users are satisfied with the software
- Actual versus planned expenditures are still acceptable enough to move forward with the project

---

# Reference

- [http://www.bawiki.com/wiki/Unified-Process.html](http://www.bawiki.com/wiki/Unified-Process.html)