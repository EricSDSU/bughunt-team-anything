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
**V or V:** Validation

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

**Test ID:** EM-03
**Written by:** Eric
**Title:** The system uses postgresql
**Traces to:** store.js
**Test type:** Integration
**Preconditions:** Set up the app
**Test data:** N/A

**Steps:**
1. Clone the repo
2. Look for postgresql

**Expected result:** The code uses postgresql
**Actual result:** The code uses the browser userstore
**Status:** Fail
**Severity:** Minor
**V or V:** Validation

---

**Test ID:** EM-04
**Written by:** Eric
**Title:** Only the hash is stored, never the password itself
**Traces to:** UML_Class.mc diagram: User passwordhash
**Test type:** Security
**Preconditions:** Create a user with a password
**Test data:** Password

**Steps:**
1. Create a user
2. Search in the database for the user's password

**Expected result:** The password does not show up only a hash
**Actual result:** The plaintext password is available
**Status:** Pass
**Severity:** Major
**V or V:** Verification

---

**Test ID:** EM-05
**Written by:** Eric
**Title:** Double voting is not allowed
**Traces to:** app.js:castVote()
**Test type:** Acceptance
**Preconditions:** Signed in user
**Test data:** A user is signed in

**Steps:**
1. Vote for a costume
2. Vote again

**Expected result:** The vote is rejected
**Actual result:** The vote is accepted
**Status:** Fail
**Severity:** Major
**V or V:** Validation
