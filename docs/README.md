# Genesis 2026: Ideathon
# HAVEN – A Privacy-First Student Well-being Platform

> **Team FixedHacks** | Genesis Ideathon | Domain: Healthcare, Biotechnology & Human Well-being

*Students are already confiding in AI chatbots. HAVEN gives them a safer place to do it: private, campus-based, and backed by real human counsellors.*

---

## 1. Problem Statement

How can colleges identify gradual declines in student well being early, without compromising student privacy, and connect students to appropriate support before the situation worsens?

## 2. The Problem

- Student well-being declines gradually through poor sleep, rising stress, and withdrawal, and nobody sees it because each signal lives in a different place.
- Students rarely ask for help because of stigma and fear of being judged. Campus support starts only when the student walks in.
- Many students now turn to general-purpose AI chatbots to share personal struggles. These tools are not built for mental health: conversations may be stored or used for training, users may not understand the privacy risks, and there is **no human accountability or crisis response**.
- Existing options (counselling centres, helplines, surveys, academic early-warning systems) are reactive, self-initiated, or aggregate only. None is proactive, privacy-first, and linked to real human support.

## 3. Our Solution: HAVEN

HAVEN is a **campus-only mobile app** where students can talk to a real counsellor, track their own well-being privately, and get gentle early support when their patterns drift, all without giving up control of their data.

### Core Features

#### 3.1 Two Ways to Log In
| Mode | How it works | Who it's for |
|---|---|---|
| **Anonymous** | Joins with a college-verified invite code or a one-time college-email verification that is **not stored**. The student gets a random pseudonymous ID, and the college never sees who they are. | Students who fear stigma or judgement |
| **Verified** | Signs in with their official college email. | Students who want direct, named support from their counsellor |

Both modes are **restricted to the student's own college**, so there are no global users, no strangers, and no public feeds. A student can switch from anonymous to verified at any time, and only by their own choice.

#### 3.2 In-App Human Counsellor
- Students can chat with a **real, college-appointed counsellor** inside the app, so they don't have to turn to a chatbot.
- Anonymous students can book sessions or message the counsellor without revealing their identity.
- Conversations are encrypted and **never used to train AI models**.

#### 3.3 Private Well-being Tracking (Early Signals)
- On-device sleep and activity data, plus a **30-second weekly check-in** based on validated tools (PHQ-2, GAD-2, WHO-5).
- HAVEN builds a **personal baseline** for each student and flags **sustained drift over weeks**, not a single bad day.
- Raw data **stays on the phone**. Detection runs on-device (TensorFlow Lite).

#### 3.4 Private Nudges First
- When drift is detected, **only the student** sees a gentle message with self-care tips (sleep routine, breathing exercises, reaching out to a friend).
- Nothing is shared with anyone unless the student chooses.

#### 3.5 Choice of Support
The student picks who to connect with:
- the campus counsellor
- a trained student peer-supporter
- a helpline (Tele-MANAS 14416)

#### 3.6 Crisis Protocol
- Crisis keywords or very high-risk check-in scores trigger an **immediate on-screen prompt** with helpline numbers and a one-tap call to the counsellor or Tele-MANAS 14416.
- **Anonymous users:** the app encourages (never forces) them to share their identity to get urgent help, and always shows emergency resources.
- A human always makes the final call. The app never decides alone.

#### 3.7 Anonymous Campus Insights
- Colleges see only **aggregated, anonymised trends**, shown only for groups of **20 or more students** (e.g. "stress rising in 2nd-year hostel blocks during exam week").
- These insights guide wellness planning, such as workshops, counsellor staffing, and timetable changes.

---

## 4. How It Works

'''
 1. SENSE      →  On-device sleep, activity + 30-sec weekly check-in
 2. DETECT     →  Personal baseline + change detection (3 domains)
 3. NUDGE      →  Private self-care tips, visible only to the student
 4. CONNECT    →  Counsellor / peer / helpline of their choice; crisis escalates
 5. LEARN      →  Anonymous campus-level insights (20+ per group)
'''

## 5. Privacy & Ethics by Design

- **Raw data stays on the device.** Only what the student explicitly allows is shared.
- **Granular, revocable consent.** Students control each data type and can delete their data at any time.
- **No misuse.** Data is never used for grades, discipline, placements, or attendance.
- **Anonymity protection.** Pseudonymous IDs, no storage of emails in anonymous mode, and no cross-linking of identity.
- **Minimum necessary data**, encrypted in transit and at rest, with role-based access.
- **Aggregate privacy.** k-anonymity (min. 20 per group) and differential privacy on campus insights.
- **Legal alignment.** Designed in line with India's DPDP Act 2023, with ethics approval planned before any pilot.
- **Human in the loop.** AI assists with detection only. It is not a replacement for a counsellor.

## 6. How HAVEN Is Different

| | General AI chatbots | Counselling centre | Wellness apps / helplines | **HAVEN** |
|---|---|---|---|---|
| Privacy-first | ❌ | ✅ | ⚠️ | ✅ |
| Anonymous option | ⚠️ | ❌ | ⚠️ | ✅ |
| Real human counsellor | ❌ | ✅ | ⚠️ | ✅ |
| Proactive early detection | ❌ | ❌ | ❌ | ✅ |
| Campus-specific | ❌ | ✅ | ❌ | ✅ |
| Crisis escalation | ❌ | ⚠️ | ⚠️ | ✅ |

## 7. Tech Stack

| Layer | Technology |
|---|---|
| Mobile app | Flutter / React Native with Health Connect (Android) and HealthKit (iOS) |
| On-device ML | TensorFlow Lite (baseline + change detection) |
| Backend | FastAPI + PostgreSQL (encrypted), with a consent ledger |
| Auth | College-email verification + anonymous pseudonymous tokens |
| Counsellor dashboard | Web app for counsellors, showing only consented information |
| Privacy layer | k-anonymity, differential privacy, role-based access control |

## 8. Feasibility & Resources

- **No new hardware.** Students' own smartphones (BYOD).
- A small campus or cloud server and a laptop for the counsellor dashboard.
- A **campus counsellor** as clinical advisor to validate thresholds and escalation rules.
- **Trained student peer-supporters** from the wellness cell.
- Ethics approval, DPDP Act legal review, and an administrative sponsor.

## 9. Implementation Roadmap

| Phase | Goal |
|---|---|
| **Phase 1: Prototype** | Dual login, weekly check-in, personal baseline, private nudges |
| **Phase 2: Human support** | In-app counsellor chat, booking, crisis protocol |
| **Phase 3: Pilot** | 100-200 students at one college, with ethics approval |
| **Phase 4: Scale** | Anonymous campus dashboard, expansion to other colleges |

## 10. Expected Impact & Pilot Targets

| Goal | Target |
|---|---|
| Opt-in rate | 50%+ of students |
| Support acceptance | 60%+ of nudged students accept support |
| Time to help | Drift to first support contact in **under 7 days** |
| False alerts | **Under 10%** |
| Privacy | **Zero** data shared without consent |



**Societal impact:** earlier help, fewer crises and dropouts, reduced stigma, less pressure on counsellors, and fewer preventable tragedies.

## 11. Risks & Mitigation

| Risk | Mitigation |
|---|---|
| Students don't trust the app | Anonymous mode, on-device data, transparent consent screens |
| False alarms or missed cases | Personal baselines, sustained-drift detection, human review, counsellor-validated thresholds |
| Counsellor overload | Triage by risk and trend, plus peer-supporters |
| Anonymous user in crisis | Always-visible emergency resources and optional identity reveal |
| Data misuse | No institutional use for grades or discipline, encryption, audit logs |

## 12. Research Basis



- About 75% of lifetime mental health conditions begin by age 24 (Kessler et al., 2005).
- India records 13,000+ student suicides a year (NCRB data).
- India's National Mental Health Survey (2015-16) found a 70-92% treatment gap.


## 13. Team FixedHacks

| Name | Roll No. |
|------|----------|
| Muppalla Rishvita | CB.SC.U4CSE25731 |
| N Sai Sameera Ram | CB.SC.U4CSE25735 |
| Jiya P | CB.SC.U4CSE25719 |
| Nandhana M. Menon | CB.SC.U4CSE25733 |

---

