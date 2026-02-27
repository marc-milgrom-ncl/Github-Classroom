Below is a clear, citation‑supported explanation of **what information GitHub Classroom stores when integrated with an LMS** and **where it is stored** for GDPR considerations.

***

# ✅ **What information does GitHub Classroom store from an LMS integration?**

GitHub Classroom supports LMS integrations via **LTI 1.3**, which allows the LMS to pass limited roster‑related information into GitHub Classroom.

### **1. Student Identifiers (Roster Data)**

When an LMS course is connected, GitHub Classroom can **import a roster of student identifiers** from the LMS.

*   GitHub’s official documentation states that connecting an LMS allows teachers to *“import a roster of student identifiers from the LMS.”* [\[docs.github.com\]](https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/connect-a-learning-management-system-course-to-a-classroom)

This typically includes:

*   LMS **student ID tokens** (LTI identifiers, not full personal profiles)
*   User‑mapping that links an LMS identity to a student’s GitHub account
*   In some setups, only the **GitHub username** is required for identifying learners (as noted in user discussions). [\[github.com\]](https://github.com/orgs/community/discussions/141763)

GitHub Classroom does **not** import grades, assignments, or sensitive LMS profile data unless explicitly provided through LTI fields (which most faculty do not enable).

### **2. OAuth / LTI Authentication Metadata**

When an LMS is registered, the system performs an **OAuth handshake** to authorize the connection.

*   LMS administrators must *“register your LMS with GitHub Classroom to initiate the OAuth handshake.”* [\[docs.github.com\]](https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/connect-a-learning-management-system-course-to-a-classroom), [\[docs.github.com\]](https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/register-a-learning-management-system-with-github-classroom)

This process stores:

*   LMS platform identifiers
*   LTI configuration keys needed for future authentication
*   No student personal data is included in this handshake other than what the LMS sends through permitted LTI claims.

***

# ✅ **Where is this information stored (for GDPR purposes)?**

### **1. Stored Within GitHub’s Infrastructure**

All roster identifiers and LMS‑related data passed to GitHub Classroom are stored **inside GitHub’s standard service infrastructure**, the same platform where GitHub organizations, repositories, and user data reside.

Although GitHub’s documentation does not publish a separate storage location for Classroom data, the LMS integration documentation shows that:

*   GitHub Classroom uses **GitHub’s own API and data models** to manage user accounts, organizations, teams, and associated metadata. [\[deepwiki.com\]](https://deepwiki.com/github-education-resources/classroom/4-external-integrations)
*   Thus, LMS‑provided identifiers become part of the **GitHub Classroom instance** associated with the teacher’s GitHub Organization.

In other words:  
▶️ **All LMS‑imported identifiers are stored on GitHub’s servers alongside standard GitHub account and organization data.**

### **2. Protected via LTI Security Standards**

GitHub emphasizes that LTI 1.3 is used because it *“helps keep your information safe and secure,”* and the integration is **IMS Global certified**. [\[docs.github.com\]](https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/connect-a-learning-management-system-course-to-a-classroom)

This means data is stored and transferred in compliance with the LTI protocol’s security requirements.

***

# 🛡️ **GDPR Considerations**

While GitHub does not provide a Classroom‑specific GDPR statement, the following points apply:

### **1. Student Data Minimization**

LTI integrations pass only the identifiers needed for roster syncing—typically **opaque, system‑generated LTI identifiers** rather than names or emails—helping reduce GDPR exposure.

### **2. Right to Information and Erasure**

GitHub users can request data deletion (as highlighted in community GDPR discussions), although some users note limitations on fully automated deletion flows. [\[github.com\]](https://github.com/orgs/community/discussions/141763)

### **3. GitHub’s General GDPR Compliance**

GitHub, as a Microsoft company, is GDPR‑compliant at the platform level. LMS‑related data inherited by GitHub Classroom follows the same global privacy framework.

***

# 📌 **Summary**

**GitHub Classroom stores the following LMS‑transferred information:**

*   ✔️ Student roster identifiers (LTI user IDs or GitHub usernames) [\[docs.github.com\]](https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/connect-a-learning-management-system-course-to-a-classroom), [\[github.com\]](https://github.com/orgs/community/discussions/141763)
*   ✔️ LMS configuration and authentication metadata (OAuth / LTI keys) [\[docs.github.com\]](https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/connect-a-learning-management-system-course-to-a-classroom), [\[docs.github.com\]](https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/register-a-learning-management-system-with-github-classroom)

**This information is stored:**

*   ✔️ Within GitHub’s standard infrastructure supporting Classroom organizations and repositories
*   ✔️ Under LTI 1.3 security and IMS Global certification requirements [\[docs.github.com\]](https://docs.github.com/en/education/manage-coursework-with-github-classroom/teach-with-github-classroom/connect-a-learning-management-system-course-to-a-classroom)

If you'd like, I can also provide a **GDPR-compliance checklist for using GitHub Classroom**, or a **data‑flow diagram** showing exactly how information moves between the LMS and GitHub Classroom.
