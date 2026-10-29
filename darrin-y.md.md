# Test Cases: Darrin Y

**Team number:** Anything

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

**Test ID:** DY-10
**Written by:** Darrin Yun
**Title:** VoteWithoutLogin
**Traces to:** CastVote function in app.js 
**Test type:** Security
**Preconditions:** Unregistered
**Test data:** Vote without logging in

**Steps:**
1. Stay logged out
2. Go to vote page
3. Click vote

**Expected result:** Not logged in error
**Actual result:** Enters a vote 
**Status:** Fail
**Severity:** Major
**V or V:** Verification

---

**Test ID:** DY-11
**Written by:** Darrin Yun
**Title:** NegativeOneVotes
**Traces to:** Function VotesRemaining in app.js the return has bad math
**Test type:** Boundary 
**Preconditions:** Used all votes
**Test data:** Use all votes

**Steps:**
1. Go to vote
2. Use all votes
3.

**Expected result:** 0 votes remaining
**Actual result:** -1 votes
**Status:** Fail 
**Severity:** Minor
**V or V:** Verification

**Test ID:** DY12
**Written by:** Darrin Yun
**Title:** CostumeNameLengthBoundaryError
**Traces to:** app.js lines 85 and 86
**Test type:** Boundary
**Preconditions:** Register and login
**Test data:** 51 character costume name

**Steps:**
1. Register and login
2. Submit costume
3. Enter a costume of 51 chars

**Expected result:** Costume name should be less than 50 error
**Actual result:** Costume accepted
**Status:** Fail
**Severity:** Minor
**V or V:** Verification

**Test ID:** DY13
**Written by:** Darrin Yun
**Title:** MultipleCostumeCanBeSubmitted
**Traces to:** Function SubmitCostume in app.js
**Test type:** Acceptance
**Preconditions:** Logged in and have 1 costume submitted
**Test data:** Submitted second costume named "lejfh" after "abc"

**Steps:**
1. Login
2. Submit costume 1
3. Submit costume 2

**Expected result:** "Costume already submitted"
**Actual result:** "Costume submitted. Good luck!"
**Status:** Fail
**Severity:** Major
**V or V:** Validation

---
