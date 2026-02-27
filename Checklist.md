Below is a **concise, practical GDPR compliance checklist** tailored for using **GitHub Classroom with an LMS**, based directly on GDPR principles and the sourced information about LMS data practices. Citations are included where relevant.

***

# ✅ **GDPR Compliance Checklist for GitHub Classroom + LMS Integrations**

This checklist helps ensure you meet GDPR requirements when processing student data through GitHub Classroom and an LMS (e.g., Canvas, Moodle, Blackboard).

***

## **1. Determine Your Lawful Basis for Processing**

*   Identify why you are collecting student identifiers from the LMS (e.g., delivering coursework, verifying student identity).
*   GDPR requires a lawful basis such as **legitimate interest**, **public task**, or **consent** (depending on your institution’s legal framework).    [\[docebo.com\]](https://www.docebo.com/learning-network/blog/gdpr-lms/)

***

## **2. Minimize the Data Collected**

*   Ensure that only **necessary identifiers** (e.g., LTI student IDs or GitHub usernames) are passed from the LMS to GitHub Classroom.  
    GitHub Classroom imports *“a roster of student identifiers”* only.    [\[docs.github.com\]](https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/connect-a-learning-management-system-course-to-a-classroom)
*   Avoid enabling optional LTI fields that expose unnecessary personal data.

***

## **3. Confirm GDPR Responsibilities With the LMS and GitHub**

*   LMS platforms process personal data such as *names, IP addresses, emails, and other identifiers*, which GDPR regulates.    [\[docebo.com\]](https://www.docebo.com/learning-network/blog/gdpr-lms/)
*   Since GitHub Classroom stores LMS-provided identifiers within GitHub’s infrastructure, document GitHub as a data processor/subprocessor in your DPIA.

***

## **4. Provide Transparent Privacy Information to Students**

*   Inform students:
    *   What identifiers are shared from the LMS to GitHub Classroom
    *   Why they are shared
    *   Where the data is stored (GitHub infrastructure)
    *   How long it is retained
*   GDPR requires clear explanation of **why data is collected and how it will be used**.    [\[docebo.com\]](https://www.docebo.com/learning-network/blog/gdpr-lms/)

***

## **5. Ensure Students Can Exercise Their Rights**

Students must have:

*   **Right of access** — know what data is held about them.
*   **Right to rectification** — correct incorrect identifiers (e.g., GitHub username mismatches).
*   **Right to erasure** — delete personal data.

GitHub users *can request deletion of their data*, though community notes discuss limitations.    [\[github.com\]](https://github.com/orgs/community/discussions/141763)

Ensure your institution has a defined process for handling these rights.

***

## **6. Implement Data Protection by Design & Default**

From GDPR's design principles:

*   Configure LMS ↔ GitHub Classroom integration to **default to the minimum data sharing**.
*   Ensure authentication uses secure protocols—GitHub Classroom uses **OAuth + LTI 1.3**, which is an **industry-standard** security mechanism.    [\[docs.github.com\]](https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/connect-a-learning-management-system-course-to-a-classroom)
*   Ensure GitHub 2FA is required for staff accessing student repositories (security measure).

***

## **7. Maintain Appropriate Technical and Organizational Controls**

*   Restrict GitHub Organization admin privileges.
*   Enforce 2FA for instructors (GitHub requires 2FA for contributors).
*   Maintain secure LMS configuration where LTI keys and settings are stored.
*   LMS providers must implement encryption and secure data handling.    [\[docebo.com\]](https://www.docebo.com/learning-network/blog/gdpr-lms/)

***

## **8. Conduct (or Update) a DPIA – Data Protection Impact Assessment**

Given the involvement of student data across multiple systems:

*   Document the data flows (LMS → GitHub Classroom → GitHub repositories).
*   List the data categories collected (LTI identifiers, GitHub usernames).
*   Identify risks and mitigation steps.  
    GDPR mandates assessments for systems processing educational data at scale.    [\[docebo.com\]](https://www.docebo.com/learning-network/blog/gdpr-lms/)

***

## **9. Ensure Data Retention and Deletion Policies**

*   Define how long student identifiers and GitHub Classroom data are retained.
*   Document how accounts and student repositories are removed after course completion.
*   Ensure deletion workflows are communicated to students.

***

## **10. Verify Third-Party Agreements**

*   Ensure institutional agreements with GitHub (Microsoft) and LMS providers meet GDPR obligations, including:
    *   Subprocessor lists
    *   International data transfer terms (Standard Contractual Clauses)
    *   Security compliance documentation
*   LMS GDPR responsibilities apply even when hosted outside the EU if students are EU residents.    [\[docebo.com\]](https://www.docebo.com/learning-network/blog/gdpr-lms/)

***

# 📄 **Optional: Want a ready-to-download PDF checklist?**

I can generate a formatted PDF version of this checklist for compliance documentation.

Just say **“Generate the PDF”**.
