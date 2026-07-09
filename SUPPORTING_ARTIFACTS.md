# SIM Project — Supporting Artifacts

This file contains the content for the Ishikawa diagram (to build in draw.io),
the Google Form structure, and the use-case diagram description.

---

## 1. Ishikawa (Fishbone) Diagram — Campus Community Crime

**Effect (head of the fish):** Rising Community/Campus Crime

Build this in draw.io using the built-in "Fishbone Diagram" shape (search
"fishbone" in the shape search). Use the 6 categories below as the bones,
each with 3–4 causes as sub-branches.

**1. People**
- Weak sense of community vigilance among students
- Reluctance to report incidents (fear, stigma, distrust)
- Landlords not screening tenants properly
- Strangers/non-residents blending into student housing areas

**2. Environment**
- Poor street lighting around hostels/off-campus housing
- Isolated or poorly monitored areas (bushes, unfinished buildings)
- High student density with weak access control
- Proximity of campus to high-crime neighborhoods

**3. Process/Method**
- No fast, easy channel to report incidents
- Slow or absent response from security after a report
- No structured record-keeping of past incidents
- Lack of coordination between campus security and local police

**4. Technology**
- No centralized incident-reporting platform (the gap SIM addresses)
- Few or no CCTV cameras in student residential areas
- No early-warning/alert system for the community
- Limited use of data to identify crime hotspots

**5. Policy/Management**
- Inadequate campus security funding/staffing
- Weak enforcement of curfews or access rules in hostels
- No formal landlord-accountability policy
- Lack of regular safety awareness campaigns

**6. Materials/Resources**
- Insufficient security personnel relative to student population
- Lack of patrol vehicles/equipment
- No emergency communication tools (e.g. panic buttons)

> Tip in draw.io: Extension > More Shapes > enable "Engineering" or just
> search "fishbone" — drag the fishbone template, then rename the head and
> the 6 bone labels to match the categories above, adding the causes as
> small text branches off each bone.

---

## 2. Google Form — Questionnaire Structure

Create this as a real Google Form (forms.google.com). Suggested structure:

**Section 1: Respondent Type**
1. What is your role in the community? *(Required, multiple choice)*
   - Student (on-campus)
   - Student (off-campus / villa)
   - University Staff
   - Landlord
   - Other

*(Use Section branching: if "Landlord" is selected, skip to Section 3)*

**Section 2: Students & Staff**
2. Where do you currently reside? *(Short answer)*
3. Have you ever witnessed or experienced a security incident on or around campus? (Yes/No)
4. If yes, what type of incident? *(Checkbox: Theft, Assault, Sexual violence, Stabbing, Murder, Other)*
5. Did you report it to anyone? (Yes/No) — If no, why not? *(Short answer / optional)*
6. How would you prefer to report a security incident? *(Multiple choice: Mobile app, Website, Phone call, In-person, Anonymous online form)*
7. Would you use a web platform like SIM to report incidents anonymously? (Yes/No/Maybe)

**Section 3: Landlords**
8. How many students currently live in your property/properties? *(Short answer)*
9. Have you had any security incidents reported to you by tenants? (Yes/No)
10. Do you currently have any security measures in place (gate, lighting, guard)? *(Checkbox)*
11. Would you support a platform where tenants can report incidents that you'd be notified of? (Yes/No/Maybe)

**Section 4: All Respondents**
12. How important do you think a dedicated incident-reporting platform would be for campus safety? *(Linear scale 1–5)*
13. Any additional comments or suggestions? *(Paragraph, optional)*

---

## 3. Use-Case Diagram — Description

**Actors:**
- Community Member (generalization of Student, Staff, Landlord)
- Visitor (anyone browsing the feed, may overlap with Community Member)

**Use Cases:**
- Submit Incident Report (primary)
  - «include» Validate Report Details
  - «extend» Submit Anonymously
- View Incident Feed

**Relationships:**
- Community Member → Submit Incident Report
- Community Member / Visitor → View Incident Feed
- Submit Incident Report ← «include» ← Validate Report Details
- Submit Anonymously «extend»s Submit Incident Report

**How to sketch in draw.io:**
1. Use UML > Use Case shapes.
2. Draw two stick-figure actors: "Community Member" and "Visitor" (or just one generalized "User" if you want to keep it minimal).
3. Draw two ovals: "Submit Incident Report" and "View Incident Feed".
4. Connect actors to their use cases with plain lines.
5. Add a smaller oval "Validate Report Details" connected to "Submit Incident Report" with a dashed arrow labeled «include».
6. Add a smaller oval "Submit Anonymously" connected to "Submit Incident Report" with a dashed arrow labeled «extend».
