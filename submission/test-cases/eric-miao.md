# Test Cases: Eric M

**Team number:** [anything]

<!--
HOW TO USE THIS FILE
1. Copy this file. Name the copy with your first name and last initial, like  maria-g.md
2. Leave TEMPLATE.md untouched for your teammates.
3. Write at least ONE failing test case. More is better.
4. Copy the block between the lines for each new test case.
5. Test IDs: use your initials plus a number, like  MG-01, MG-02. This keeps IDs unique across your team.
6. See docs/TESTING_FIELD_GUIDE.md for the sample test case TC-00.
-->

---

**Test ID:** EM-1
**Written by:** Eric
**Title:** Only the owner of a costume can delete it.
**Traces to:** app.js:function deleteCostume(id)
**Test type:** Acceptance
**Preconditions:** Deletion requires the requester be the owner of the costume.
**Test data:** User A: has costume

**Steps:**
1. Create a new user user b
2. Log in as user b
3. Attempt to delete user a's costume

**Expected result:** user b can't delete the costume
**Actual result:** user b can delete the costume
**Status:** fail
**Severity:** Major
**V or V:** Verification

---

**Test ID:** EM-2
**Written by:** Eric
**Title:** Secrets 
**Traces to:** https://github.com/EricSDSU/bughunt-team-anything/blob/main/app/config.js
**Test type:** Security
**Preconditions:** Secrets should be hidden in .env or another gitignored file
**Test data:** "sk_live_fr1ght_n1ght_8f3a9c2e7b1d4f6a0c5e" and other secure api keys

**Steps:**
1. Clone the repository
2. rg . "API_KEY|ADMIN"

**Expected result:** Keys do not appear in terminal
**Actual result:** 12:  API_KEY: "sk_live_fr1ght_n1ght_8f3a9c2e7b1d4f6a0c5e",
**Status:** Fail
**Severity:** Critical
**V or V:** Verification

---

**Test ID:**
**Written by:**
**Title:**
**Traces to:**
**Test type:** (Unit / Integration / System / Acceptance / Boundary Value / Negative / Security)
**Preconditions:**
**Test data:**

**Steps:**
1.
2.
3.

**Expected result:**
**Actual result:**
**Status:** (Pass / Fail)
**Severity:** (Critical / Major / Minor, Fail only)
**V or V:** (Verification / Validation, Fail only)

---

**Test ID:**
**Written by:**
**Title:**
**Traces to:**
**Test type:** (Unit / Integration / System / Acceptance / Boundary Value / Negative / Security)
**Preconditions:**
**Test data:**

**Steps:**
1.
2.
3.

**Expected result:**
**Actual result:**
**Status:** (Pass / Fail)
**Severity:** (Critical / Major / Minor, Fail only)
**V or V:** (Verification / Validation, Fail only)
