# SIO West Bengal — Activities Page Wireframe & Section-Wise Content Matrix
> **Document Status**: Production Ready & Fully Aligned with Existing Codebase  

> **Document Status**: Production Ready & Fully Aligned with Official SIO Constitution (Amended Dec 2022) & Biennial Policy & Programme (2025–2026 / 22nd Term)  
> **Target Route**: `/activities`  
> **Source File**: [`src/app/activities/page.tsx`](file:///home/masyud/Development/Masyud/SIO/src/app/activities/page.tsx)  
> **Design Pattern**: Dynamic Student Movement & Social Welfare Hub with 5 Functional Pillars, Sticky Pill Navigation, Real-Time Search, Metrics Badges, and Interactive Participation Modal.
> **Design Pattern**: Dynamic Student Movement & Social Welfare Hub with 5 Functional Pillars, Session 2025–2026 Policy Alignment, Sticky Pill Navigation, Real-Time Search, Impact Metrics, Biennial Calendar, and Interactive Participation Modal.

---

## 1. Executive Summary & Page Architecture

The **Activities Page** (`/activities`) serves as the central showcase of SIO West Bengal's grassroots student activism, statewide advocacy campaigns, flagship conferences, educational talent hunts, and emergency humanitarian relief services.
The **Activities Page** (`/activities`) serves as the central operational hub of SIO West Bengal's grassroots student activism, statewide advocacy campaigns, flagship conferences, higher education admissions desks, and emergency humanitarian relief services in execution of the **Biennial Policy & Programme (January 2025 – December 2026 / 22nd Term)**.

### Core Strategic Pillars:
$$\text{Campaigns (অভিযানসমূহ)} \longleftrightarrow \text{Flagship Events (অনুষ্ঠানসমূহ)} \longleftrightarrow \text{Education (শিক্ষা)} \longleftrightarrow \text{Youth (ছাত্র ও যুব)} \longleftrightarrow \text{Social Welfare (সামাজিক উদ্যোগ)}$$

### Key Technical & Visual Attributes:
- **Sticky Filter Navigation**: Sticky top filter bar featuring 6 dynamic pills with real-time counter badges (`All`, `Campaigns`, `Events`, `Education`, `Youth`, `Social`).
- **Sticky Filter Navigation**: Sticky top filter bar featuring 6 dynamic pills with real-time counter badges (`All [12]`, `Campaigns [3]`, `Events [3]`, `Education [2]`, `Youth [2]`, `Social [2]`).
- **Instant Search Filtering**: Real-time multi-field search engine across titles, descriptions, and locations in both Bengali and English.
- **Unified Activity Card Anatomy**:
  - Top status pill (`Active` / `Upcoming` / `Completed`) with corresponding color palettes (Emerald, Blue, Slate).
  - Prominent verified impact metric tag (e.g., `১,০০,০০০+ শিক্ষার্থী স্বাক্ষর`, `৩৫,০০০+ পরীক্ষার্থী`, `৬,০০০+ ইউনিট রক্তদান`).
  - Prominent verified impact metric tag (e.g., `১,০০,০০০+ শিক্ষার্থী স্বাক্ষর`, `৩৫,০০০+ পরীক্ষার্থী`, `১০,০০০+ রক্তদাতা নেটওয়ার্ক`).
  - Bilingual Title & Description.
  - Geo-location & operational timeframe metadata with Lucide icons (`MapPin`, `Clock`).
  - 3-point Key Highlights checklist with blue check indicators (`CheckCircle2`).
  - Interactive `Participate / Details` modal trigger button and quick `/contact#form` inquiry link.
- **Interactive Participation Modal**: Instant feedback toast/modal acknowledging student engagement and dispatching interest to zonal coordination.
- **Interactive Participation Modal**: Instant feedback modal acknowledging student engagement and dispatching interest to zonal coordination.
- **Volunteer Gateway CTA**: Dark navy banner (`#0F4C81`) routing to `/contact` and `/student-corner`.

---

## 2. Interactive Flowchart & Information Architecture

```mermaid
flowchart TD
    subgraph S0["0. Top Navigation & Header Bar (Sticky)"]
        Nav1["[Official SIO Emblem] SIO WEST BENGAL"] --- Nav2["Desktop Navigation Menu (Active: কার্যক্রম / Activities)"] --- Nav3["Search | Lang Switcher (বাংলা/EN) | Mobile Hamburger"]
    end

    subgraph S1["1. Hero Showcase Section (#EAF6FF)"]
        H1["Eyebrow Badge: 'ছাত্র আন্দোলন ও সমাজকল্যাণ'"]
        H1["Eyebrow Badge: 'সেশন ২০২৫–২৬ • ২২তম টার্ম • ছাত্র আন্দোলন ও সমাজকল্যাণ'"]
        H2["H1: 'আমাদের কার্যক্রম, অভিযান ও সামাজিক উদ্যোগ' (Activities & Campaigns)"]
        H3["Search: [Q অভিযান, সম্মেলন বা উদ্যোগের নাম লিখে খুঁজুন... / Search activities...]"]
        H3["Search: [Q অভিযান, সম্মেলন, ইনকাব বা পরিবেশ উদ্যোগ খুঁজুন... / Search activities...]"]
    end

    subgraph S2["2. Sticky Pillar Navigation Bar (#pillar-nav)"]
        P0["[সকল কার্যক্রম (10)]"] --- P1["[অভিযানসমূহ (2)]"] --- P2["[অনুষ্ঠানসমূহ (2)]"] --- P3["[শিক্ষা কার্যক্রম (2)]"] --- P4["[ছাত্র ও যুব (2)]"] --- P5["[সামাজিক উদ্যোগ (2)]"]
        P0["[সকল কার্যক্রম (12)]"] --- P1["[অভিযানসমূহ (3)]"] --- P2["[অনুষ্ঠানসমূহ (3)]"] --- P3["[শিক্ষা কার্যক্রম (2)]"] --- P4["[ছাত্র ও যুব (2)]"] --- P5["[সামাজিক উদ্যোগ (2)]"]
    end

    subgraph S3["3. Five Strategic Pillars — 2-Column Responsive Card Grid (#F7FAFC)"]
        subgraph C_Camp["1. Campaigns (অভিযানসমূহ)"]
            CC1["Card: রাজ্য শিক্ষা অধিকার ও ক্যাম্পাস গণতন্ত্র রক্ষা অভিযান (১,০০,০০০+ স্বাক্ষর • Active)"]
            CC2["Card: নৈতিক চরিত্র ও মাদকবিরোধী সচেতনতা সপ্তাহ (৫০,০০০+ শপথপত্র • Active)"]
            CC2["Card: চারিত্রিক শালীনতা, যৌন সচেতনতা ও মাদকবিরোধী সপ্তাহ (৫০,০০০+ শপথপত্র • Active)"]
            CC3["Card: জাতীয় তাজকিয়া অভিযান ও কুরআন পাঠ চক্র (৫০০+ ইউনিট সার্কেল • Active)"]
        end

        subgraph C_Evt["2. Flagship Events (অনুষ্ঠানসমূহ)"]
            CE1["Card: পশ্চিমবঙ্গ রাজ্য ছাত্র সম্মেলন ২০২৪ (১৫,০০০+ প্রতিনিধি • Upcoming)"]
            CE2["Card: বার্ষিক অ্যাকাডেমিক রিসার্চ কনক্লেভ CERT (৪০+ গবেষণাপত্র • Upcoming)"]
            CE1["Card: পশ্চিমবঙ্গ রাজ্য ছাত্র সম্মেলন ২০২৫ (১৫,০০০+ প্রতিনিধি • Upcoming)"]
            CE2["Card: হিস্ট্রি সামিট ও আইকেএস কনক্লেভ CERT (৪০+ গবেষণাপত্র • Upcoming)"]
            CE3["Card: আন নূর জাতীয় সাহিত্য উৎসব ২.০ (১,৫০০+ তরুণ লেখক ও শিল্পী • Upcoming)"]
        end

        subgraph C_Edu["3. Educational Programs (শিক্ষা কার্যক্রম)"]
            CD1["Card: রাজ্য বিজ্ঞান মেধা অন্বেষণ পরীক্ষা STSE (৩৫,০০০+ পরীক্ষার্থী • Active)"]
            CD2["Card: ফ্রি লাইব্রেরি ও ডিজিটাল স্টাডি ব্যাংক নেটওয়ার্ক (১২,০০০+ বই • Active)"]
            CD1["Card: উচ্চশিক্ষা ও ভর্তি একাডেমি 'Project InQhab' (৫,০০০+ শিক্ষার্থী • Active)"]
            CD2["Card: রাজ্য বিজ্ঞান মেধা অন্বেষণ পরীক্ষা STSE (৩৫,০০০+ পরীক্ষার্থী • Active)"]
        end

        subgraph C_Yth["4. Youth Activities (ছাত্র ও যুব কার্যক্রম)"]
            CY1["Card: ইয়ুথ লিডারশিপ সামার ক্যাম্প ও ব্যক্তিত্ব উন্নয়ন (১২০০+ গ্র্যাজুয়েট • Active)"]
            CY2["Card: কিশোর উৎসব ও সৃজনশীল মেধা মেলা (৮,০০০+ অংশগ্রহণকারী • Upcoming)"]
            CY1["Card: লিডারশিপ ডেভেলপমেন্ট ও স্টেম ক্যাম্পাস সামিট (১,২০০+ শিক্ষার্থী • Active)"]
            CY2["Card: মানসিক স্বাস্থ্য ফোরাম ও ২৪/৭ যুব হেল্পলাইন (৩,৫০০+ কাউন্সেলিং • Active)"]
        end

        subgraph C_Soc["5. Social Welfare (সামাজিক উদ্যোগ ও ত্রাণ)"]
            CS1["Card: রাজ্যব্যাপী জরুরি রক্তদাতা নেটওয়ার্ক Life Line (৬,০০০+ ইউনিট/বছর • Active)"]
            CS2["Card: দুর্যোগে জরুরি ত্রাণ ও পুনর্বাসন কর্মসূচি (৫০,০০০+ পরিবার ত্রাণ • Active)"]
        subgraph C_Soc["5. Social Welfare & Environment (সামাজিক উদ্যোগ ও পরিবেশ)"]
            CS1["Card: পরিসর সংবাদ — ক্যাম্পাস পরিবেশ ও ইকোলজি ফোরাম (১০০+ ক্যাম্পাস ফোরাম • Active)"]
            CS2["Card: রাজ্যব্যাপী জরুরি রক্তদাতা নেটওয়ার্ক Life Line (১০,০০০+ রক্তদাতা • Active)"]
        end
    end

    subgraph S4["4. Interactive Participation & Volunteer Feedback"]
        MD1["Modal / Toast: '[কার্যক্রমের নাম]' আগ্রহ গ্রহণ করা হয়েছে! আমাদের প্রতিনিধি যোগাযোগ করবেন।"]
        MD2["Inquire Action: সরাসরি যোগাযোগ ও তথ্য ডেস্ক (/contact#form)"]
    end

    subgraph S5["5. Student Movement & Volunteer CTA Banner (#0F4C81)"]
        CTA1["Badge: 'দেশ ও সমাজের সেবায় চার দশক' + H2: 'আপনার এলাকায় আমাদের কার্যক্রমে যুক্ত হতে চান?'"]
        CTA1["Badge: 'দ্বীনি নির্দেশনার আলোয় সমাজ পুনর্গঠন' + H2: 'আপনার এলাকায় আমাদের কার্যক্রমে যুক্ত হতে চান?'"]
        CTA2["Dual Actions: [যোগাযোগ করুন →] (Linked to /contact) & [শিক্ষার্থী কর্নার দেখুন] (/student-corner)"]
    end

    subgraph S6["6. Master Black Footer (#0F172A)"]
        FT1["Helpline 24/7 (+91 12345 67890) + Socials + Quick Links + Alimuddin St Map + Copyright"]
    end

    S0 --> S1 --> S2 --> S3 --> S4 --> S5 --> S6
```

---

## 3. Visual Wireframes (ASCII Schematics)
## 3. Section-Wise Detailed Content Matrix

### 3.1 Activities Directory (`/activities`) — Desktop Layout (1280px+)
### Section 1: Hero Showcase & Real-Time Search Bar
- **Section ID**: `#top`
- **Background**: Light Sky Blue (`#EAF6FF`)
- **Name-Wise Content**:
  - **Eyebrow Badge**: `সেশন ২০২৫–২৬ • ২২তম টার্ম • ছাত্র আন্দোলন ও সমাজকল্যাণ` / `Session 2025–26 • 22nd Term • Student Movement & Social Action`
  - **Main H1 Title**: `আমাদের কার্যক্রম, অভিযান ও সামাজিক উদ্যোগ` / `Statewide Activities, Campaigns & Social Initiatives`
  - **Description**: `এসআইও সংবিধানের লক্ষ্য এবং 'পলিসি অ্যান্ড প্রোগ্রাম ২০২৫–২৬'-এর নির্দেশনায় শিক্ষাঙ্গনের গণতান্ত্রিক অধিকার রক্ষা, আত্মশুদ্ধি, মেধা বিকাশ এবং মানবিক সেবায় আমাদের চার দশকেরও বেশি সময়ের ধারাবাহিক পথচলা।`
  - **Search Input**: `[Q অভিযান, সম্মেলন, ইনকাব বা পরিবেশ উদ্যোগ খুঁজুন... / Search activities...]` with clear reset trigger.

```
+--------------------------------------------------------------------------------------------------+
| [LOGO] SIO West Bengal        [Home]  [About]  [Leadership]  [ACTIVITIES*]  [Contact]  [BN/EN]   |
+--------------------------------------------------------------------------------------------------+
| HERO SHOWCASE & SEARCH BAR (#EAF6FF)                                                             |
|                                                                                                  |
|   (•) STUDENT MOVEMENTS & SOCIAL ACTION / ছাত্র আন্দোলন ও সমাজকল্যাণ                                 |
|   STATEWIDE ACTIVITIES, CAMPAIGNS & SOCIAL WELFARE                                               |
|   আমাদের কার্যক্রম, অভিযান ও সামাজিক উদ্যোগ                                                          |
|   Advocating educational equity, campus democracy, moral character development, and active       |
|   emergency relief across West Bengal for over four decades.                                     |
|                                                                                                  |
|   +-------------------------------------------------------------------------+                    |
|   | [Q] Search campaigns, conferences, relief programs, or districts...   [X]|                    |
|   +-------------------------------------------------------------------------+                    |
+--------------------------------------------------------------------------------------------------+
| STICKY PILLAR NAVIGATION BAR (Sticky top-16 md:top-[72px])                                       |
| [All Activities (10)] [Campaigns (2)] [Events (2)] [Education (2)] [Youth (2)] [Social (2)]      |
+--------------------------------------------------------------------------------------------------+
| MAIN CONTENT AREA (2-Column Grid / #F7FAFC)                                                      |
|                                                                                                  |
|   +----------------------------------------+  +----------------------------------------+         |
|   | [Active]        [১,০০,০০০+ স্বাক্ষর]   |  | [Active]          [৫০,০০০+ শপথপত্র]    |         |
|   | Statewide Right to Education & Campus  |  | Moral Character & Anti-Substance       |         |
|   | Democracy Campaign                     |  | Abuse Awareness Drive                  |         |
|   | রাজ্য শিক্ষা অধিকার ও ক্যাম্পাস গণতন্ত্র |  | নৈতিক চরিত্র ও মাদকবিরোধী সচেতনতা     |         |
|   |                                        |  |                                        |         |
|   | Description: Statewide student drive   |  | Description: Extensive campaign        |         |
|   | against fee hikes, equitable access... |  | educating students against addiction...|         |
|   |                                        |  |                                        |         |
|   | [Pin] All Universities & Districts WB  |  | [Pin] 23 Districts & 500+ Campuses     |         |
|   | [Clock] Ongoing Campaign               |  | [Clock] Annual State Campaign          |         |
|   |                                        |  |                                        |         |
|   | Key Highlights:                        |  | Key Highlights:                        |         |
|   |  [v] Signature drive & memorandum      |  |  [v] Street plays, posters & counseling|         |
|   |  [v] Marches for education budget      |  |  [v] Anti-addiction helpline desk      |         |
|   |  [v] Campus democracy conventions      |  |  [v] Youth marathon & moral pledges    |         |
|   |                                        |  |                                        |         |
|   | [Participate / Details ->] [Inquire ->]|  | [Participate / Details ->] [Inquire ->]|         |
|   +----------------------------------------+  +----------------------------------------+         |
|                                                                                                  |
|   +----------------------------------------+  +----------------------------------------+         |
|   | [Upcoming]         [১৫,০০০+ প্রতিনিধি] |  | [Upcoming]         [৪০+ গবেষণাপত্র]   |         |
|   | West Bengal State Student Conf 2024    |  | Annual Academic Research Conclave CERT |         |
|   | পশ্চিমবঙ্গ রাজ্য ছাত্র সম্মেলন ২০২৪      |  | বার্ষিক অ্যাকাডেমিক রিসার্চ কনক্লেভ    |         |
|   |                                        |  |                                        |         |
|   | Description: Flagship biennial summit  |  | Description: Research symposium on     |         |
|   | gathering thousands of delegates...    |  | minority education, pedagogy...        |         |
|   |                                        |  |                                        |         |
|   | [Pin] Kolkata Convention Centre        |  | [Pin] Jadavpur Campus & Auditorium     |         |
|   | [Clock] Upcoming Event                 |  | [Clock] October 2024                   |         |
|   |                                        |  |                                        |         |
|   | Key Highlights:                        |  | Key Highlights:                        |         |
|   |  [v] National academic scholar talks   |  |  [v] Peer-reviewed journal publications|         |
|   |  [v] Academic panels & seminars        |  |  [v] Policy roundtable dialogues       |         |
|   |  [v] Student talent awards & cultural  |  |  [v] Research grant announcements      |         |
|   |                                        |  |                                        |         |
|   | [Participate / Details ->] [Inquire ->]|  | [Participate / Details ->] [Inquire ->]|         |
|   +----------------------------------------+  +----------------------------------------+         |
|                                                                                                  |
|   +----------------------------------------+  +----------------------------------------+         |
|   | [Active]           [৩৫,০০০+ পরীক্ষার্থী]|  | [Active]             [১২,০০০+ বই]      |         |
|   | State Talent Search Exam (STSE)        |  | Free Public Library & Book Bank        |         |
|   | রাজ্য বিজ্ঞান মেধা অন্বেষণ পরীক্ষা (STSE)|  | ফ্রি লাইব্রেরি ও ডিজিটাল স্টাডি ব্যাংক|         |
|   |                                        |  |                                        |         |
|   | [Pin] 250+ Centers Across Bengal       |  | [Pin] 85+ Local Study Centers          |         |
|   | [Clock] Annually in December           |  | [Clock] Round-the-Year Access          |         |
|   | [Participate / Details ->] [Inquire ->]|  | [Participate / Details ->] [Inquire ->]|         |
|   +----------------------------------------+  +----------------------------------------+         |
|                                                                                                  |
|   +----------------------------------------+  +----------------------------------------+         |
|   | [Active]            [১২০০+ গ্র্যাজুয়েট]|  | [Upcoming]         [৮,০০০+ অংশগ্রহণকারী]|        |
|   | Youth Leadership Summer Retreat        |  | Junior Fest & Creative Talent Expo     |         |
|   | ইয়ুথ লিডারশিপ সামার ক্যাম্প            |  | কিশোর উৎসব ও সৃজনশীল মেধা মেলা        |         |
|   |                                        |  |                                        |         |
|   | [Pin] Darjeeling & Bankura Centers     |  | [Pin] All District Headquarters        |         |
|   | [Clock] May & June                     |  | [Clock] November 2024                  |         |
|   | [Participate / Details ->] [Inquire ->]|  | [Participate / Details ->] [Inquire ->]|         |
|   +----------------------------------------+  +----------------------------------------+         |
|                                                                                                  |
|   +----------------------------------------+  +----------------------------------------+         |
|   | [Active]             [৬,০০০+ ইউনিট রক্ত]|  | [Active]           [৫০,০০০+ পরিবার ত্রাণ|        |
|   | Emergency Blood Donors (Life Line)     |  | Disaster Emergency Relief & Rehab      |         |
|   | জরুরি রক্তদাতা নেটওয়ার্ক (Life Line)   |  | দুর্যোগে জরুরি ত্রাণ ও পুনর্বাসন       |         |
|   |                                        |  |                                        |         |
|   | [Pin] All Govt Medical Colleges & Hosps|  | [Pin] Sundarbans, North Bengal Belts   |         |
|   | [Clock] 24/7 Emergency Service         |  | [Clock] Rapid Emergency Deployment     |         |
|   | [Participate / Details ->] [Inquire ->]|  | [Participate / Details ->] [Inquire ->]|         |
|   +----------------------------------------+  +----------------------------------------+         |
+--------------------------------------------------------------------------------------------------+
| STUDENT MOVEMENT CTA BANNER (#0F4C81 Navy)                                                       |
|   (•) FOUR DECADES OF STUDENT LEADERSHIP / দেশ ও সমাজের সেবায় চার দশক                            |
|   Want to Organize or Participate in SIO Initiatives?                                            |
|   আপনার এলাকায় বা ক্যাম্পাসে আমাদের কার্যক্রমে যুক্ত হতে চান?                                       |
|                                                                                                  |
|   [Get in Touch / যোগাযোগ করুন ->]              [Visit Student Corner / শিক্ষার্থী কর্নার]        |
+--------------------------------------------------------------------------------------------------+
| MASTER BLACK FOOTER (#0F172A)                                                                    |
|   24/7 Emergency Helpline | Quick Navigation | Social Channels | Google Maps HQ Location         |
+--------------------------------------------------------------------------------------------------+
```

---

### 3.2 Mobile Visual Layout (375px–430px Responsive View)
### Section 2: Sticky 5-Pillar Navigation Bar
- **Section ID**: `#pillar-nav`
- **Positioning**: Sticky `top-16 md:top-[72px] z-40 bg-white border-b border-[#E5E7EB] shadow-2xs`
- **Filter Pills**:
  1. `সকল কার্যক্রম (12)` (`category: "all"`)
  2. `অভিযানসমূহ (3)` (`category: "campaigns"`)
  3. `অনুষ্ঠানসমূহ (3)` (`category: "events"`)
  4. `শিক্ষা কার্যক্রম (2)` (`category: "education"`)
  5. `ছাত্র ও যুব (2)` (`category: "youth"`)
  6. `সামাজিক উদ্যোগ (2)` (`category: "social"`)

```
+-----------------------------------+
| [=] SIO WB Logo          [BN/EN]  |
+-----------------------------------+
| HERO SECTION                      |
| (•) STUDENT ACTION & WELFARE      |
| Activities, Campaigns & Welfare   |
| কার্যক্রম, অভিযান ও সামাজিক উদ্যোগ|
|                                   |
| [Q Search activities or dist...]  |
+-----------------------------------+
| HORIZONTAL SCROLL PILL NAV        |
| [All(10)] [Camp(2)] [Evt(2)] [Edu]|
+-----------------------------------+
| 1-COLUMN ACTIVITY CARDS           |
|                                   |
| +-------------------------------+ |
| | [Active]   [১,০০,০০০+ স্বাক্ষর] | |
| | Right to Education Campaign   | |
| | রাজ্য শিক্ষা অধিকার অভিযান   | |
| |                               | |
| | Campus democracy, fee hike    | |
| | reforms across Bengal...      | |
| |                               | |
| | [Pin] All WB Universities     | |
| | [Clock] Ongoing Campaign      | |
| |                               | |
| | Key Highlights:               | |
| |  [v] Mass signatures          | |
| |  [v] Education budget rallies | |
| |  [v] Campus open dialogue     | |
| |                               | |
| | [Participate / Details ->]    | |
| | Inquire →                     | |
| +-------------------------------+ |
|                                   |
| +-------------------------------+ |
| | [Upcoming]  [১৫,০০০+ প্রতিনিধি]| |
| | WB State Student Conf 2024    | |
| | পশ্চিমবঙ্গ রাজ্য ছাত্র সম্মেলন| |
| |                               | |
| | [Pin] Kolkata Conv. Centre    | |
| | [Clock] Upcoming Event        | |
| |                               | |
| | [Participate / Details ->]    | |
| | Inquire →                     | |
| +-------------------------------+ |
|                                   |
| +-------------------------------+ |
| | [Active]     [৬,০০০+ ইউনিট রক্ত]| |
| | Statewide Blood Donors Network| |
| | জরুরি রক্তদাতা নেটওয়ার্ক      | |
| |                               | |
| | [Pin] All Govt Hospitals      | |
| | [Clock] 24/7 Emergency        | |
| |                               | |
| | [Participate / Details ->]    | |
| | Inquire →                     | |
| +-------------------------------+ |
+-----------------------------------+
| CTA: CONNECT WITH SIO WB          |
| [Get in Touch] [Student Corner]   |
+-----------------------------------+
| MASTER FOOTER                     |
+-----------------------------------+
```

---

## 4. Section-by-Section Name-Wise Content Matrix

### Section 0: Sticky Navigation Header
- **Component File**: [`src/components/layout/header.tsx`](file:///home/masyud/Development/Masyud/SIO/src/components/layout/header.tsx)
- **Position**: Sticky (`top-0 z-50 bg-white/95 backdrop-blur-md border-b border-[#E5E7EB]`)
- **Active Navigation Link**: `কার্যক্রম (Activities)`
- **Actions**: Language switch (`বাংলা` / `English`), Search toggle, CTA button (`যুক্ত হোন / Join Us`).

---

### Section 1: Hero Showcase & Real-Time Search Bar (`#top`)
- **Component File**: Native Section in [`src/app/activities/page.tsx`](file:///home/masyud/Development/Masyud/SIO/src/app/activities/page.tsx)
- **Styling**: Light Sky Blue backdrop (`#EAF6FF`) with radial gradient glow orbs.

| Content Field | Bengali Translation (`bn`) | English Translation (`en`) |
| :--- | :--- | :--- |
| **Top Eyebrow Pill** | `ছাত্র আন্দোলন ও সমাজকল্যাণ` | `Student Movements & Social Action` |
| **Main Title** | `আমাদের কার্যক্রম, অভিযান ও সামাজিক উদ্যোগ` | `Statewide Activities, Campaigns & Social Welfare` |
| **Subtitle Description** | `ক্যাম্পাস অধিকার রক্ষা থেকে শুরু করে নৈতিক চরিত্র গঠন, মেধা অন্বেষণ পরীক্ষা এবং প্রাকৃতিক দুর্যোগে ত্রাণ বিতরণ—চার দশক ধরে SIO পশ্চিমবঙ্গ ছাত্র ও যুব সমাজের কল্যাণে অবিচল।` | `Advocating educational equity, student rights, moral character development, and active emergency relief across West Bengal for over four decades.` |
| **Search Placeholder** | `অভিযান, সম্মেলন বা উদ্যোগের নাম লিখে খুঁজুন...` | `Search campaigns, conferences, or relief programs...` |
| **Search Clear Glyph** | `✕ (অনুসন্ধান মুছুন)` | `✕ (Clear)` |

---

### Section 2: Sticky Pillar Navigation Bar (`#pillar-nav`)
- **Component**: Sticky Header Strip (`sticky top-16 md:top-[72px] z-40 bg-white border-b border-[#E5E7EB] shadow-2xs`)
- **Pills**: Responsive horizontal scroll pills with count badges and Lucide SVG icons.

| Tab ID | Bengali Label | English Label | Icon | Count | Filter Target |
| :--- | :--- | :--- | :--- | :--- | :--- |
| `all` | `সকল কার্যক্রম` | `All Activities` | `Sparkles` | **10** | Shows entire collection |
| `campaigns` | `অভিযানসমূহ` | `Campaigns` | `Megaphone` | **2** | Educational rights & moral drives |
| `events` | `অনুষ্ঠানসমূহ` | `Events` | `Calendar` | **2** | State conferences & research conclaves |
| `education`| `শিক্ষা কার্যক্রম` | `Educational Programs` | `GraduationCap` | **2** | Talent searches & book banks |
| `youth` | `ছাত্র ও যুব` | `Youth Activities` | `Users` | **2** | Leadership camps & creative fests |
| `social` | `সামাজিক উদ্যোগ` | `Social Welfare` | `HeartHandshake` | **2** | Blood network & disaster relief |

---

### Section 3: Campaigns Pillar Grid (`category: "campaigns"`)
- **Focus**: Statewide student rights, higher education governance, and ethical public campaigns.

#### Card 3.1: Right to Education & Campus Democracy Campaign
#### Card 3.1: Statewide Right to Education & Campus Democracy Drive
- **ID**: `camp-1`
- **Status**: `active` (`চলমান`) | **Style**: `bg-emerald-50 text-emerald-700 border-emerald-200`
- **Verified Impact Metric**: `১,০০,০০০+ শিক্ষার্থী স্বাক্ষর` (100,000+ Student Signatures)
- **Title (BN)**: `রাজ্য শিক্ষা অধিকার ও ক্যাম্পাসে গণতন্ত্র রক্ষা অভিযান`
- **Title (EN)**: `Statewide Right to Education & Campus Democracy Campaign`
- **Description (BN)**: `উচ্চশিক্ষায় ফি বৃদ্ধি প্রতিরোধ, মেধাভিত্তিক ও স্বচ্ছ ভর্তি প্রক্রিয়া, এবং বিশ্ববিদ্যালয় ক্যাম্পাসসমূহে অবাধ গণতান্ত্রিক পরিবেশ নিশ্চিত করার দাবিতে রাজ্যব্যাপী ছাত্র আন্দোলন।`
- **Description (EN)**: `Statewide campaign against fee hikes, demanding equitable admissions, campus democracy, and fair representation for all students.`
- **Location (BN/EN)**: `পশ্চিমবঙ্গের সকল বিশ্ববিদ্যালয় ও জেলা` / `All Universities & Districts across WB`
- **Timeframe (BN/EN)**: `চলমান অভিযান` / `Ongoing Campaign`
- **Status**: `active` (`চলমান`)
- **Verified Metric**: `১,০০,০০০+ শিক্ষার্থী স্বাক্ষর` (1,00,000+ Student Signatures)
- **Title (BN)**: `রাজ্য শিক্ষা অধিকার, ক্যাম্পাস গণতন্ত্র ও ছাত্র সংসদ পুনর্বহাল অভিযান`
- **Title (EN)**: `Statewide Right to Education, Campus Democracy & Student Union Restoration Campaign`
- **Policy Alignment**: পলিসি পৃষ্ঠা ১৭-১৮ (ক্যাম্পাস সংস্কৃতি ও নিষিদ্ধ ছাত্র সংসদ সচল করার আন্দোলন)।
- **Description (BN)**: `পশ্চিমবঙ্গের বিশ্ববিদ্যালয় ও কলেজগুলোতে গণতান্ত্রিক পরিবেশ ফিরিয়ে আনা, নিষিদ্ধ ছাত্র সংসদ নির্বাচন পুনর্বহাল, অন্যায্য ফি বৃদ্ধি প্রতিরোধ এবং সংখ্যালঘু শিক্ষার্থীদের জন্য শিক্ষা বাজেটের দাবিতে রাজ্যব্যাপী ঐতিহাসিক আন্দোলন।`
- **Location**: সকল বিশ্ববিদ্যালয়, কলেজ ও জেলা সদর
- **Timeframe**: চলমান সেশন ২০২৫–২৬
- **Key Highlights**:
  1. `কলেজ ও বিশ্ববিদ্যালয় স্তরে গণস্বাক্ষর সংগ্রহ ও মেমোরেন্ডাম পেশ` (Mass signature collection & memorandum submission)
  2. `শিক্ষা বাজেট বৃদ্ধি ও স্কলারশিপ বরাদ্দের দাবিতে রাজপথে পদযাত্রা` (Public rallies demanding educational budget hikes)
  3. `ক্যাম্পাস গণতন্ত্র কনভেনশন ও ওপেন ডায়ালগ ফোরাম` (Campus democracy conventions & open dialogue forums)
  1. `শিক্ষামন্ত্রীর নিকট গণস্বাক্ষর সম্বলিত স্মারকলিপি পেশ`
  2. `ক্যাম্পাসে গণতান্ত্রিক ছাত্র সংসদ নির্বাচনের দাবিতে কনভেনশন`
  3. `মাতৃভাষায় শিক্ষা নিশ্চিতকরণ ও ড্রপ-আউট প্রতিরোধ সমাবেশ`.

#### Card 3.2: Moral Character & Anti-Substance Abuse Awareness Drive
#### Card 3.2: Moral Character, Sexual Morality & Anti-Addiction Week
- **ID**: `camp-2`
- **Status**: `active` (`চলমান`)
- **Verified Impact Metric**: `৫০,০০০+ শপথপত্র পূরণ` (50,000+ Youth Pledges)
- **Title (BN)**: `নৈতিক চরিত্র ও মাদকবিরোধী সচেতনতা সপ্তাহ`
- **Title (EN)**: `Moral Character & Anti-Substance Abuse Awareness Drive`
- **Description (BN)**: `ক্যাম্পাস ও শহর-গ্রামাঞ্চলের তরুণদের মাঝে মাদক ও সামাজিক অবক্ষয়ের বিরুদ্ধে সচেতনতা সৃষ্টি এবং সুস্থ নৈতিক মূল্যবোধ জাগিয়ে তোলার আন্দোলন।`
- **Description (EN)**: `Extensive campaign educating students against drug addiction, substance abuse, and moral erosion through street plays, posters, and counseling.`
- **Location (BN/EN)**: `২৩ টি জেলা ও ৫০০+ ক্যাম্পাস` / `23 Districts & 500+ Campuses`
- **Timeframe (BN/EN)**: `বার্ষিক রাজ্য অভিযান` / `Annual State Campaign`
- **Verified Metric**: `৫০,০০০+ শিক্ষার্থী শপথপত্র` (50,000+ Pledges Taken)
- **Title (BN)**: `চারিত্রিক শালীনতা, যৌন সচেতনতা ও মাদকবিরোধী সপ্তাহ`
- **Title (EN)**: `Moral Character, Sexual Morality & Anti-Substance Abuse Awareness Drive`
- **Policy Alignment**: পলিসি পৃষ্ঠা ১১ ও ২৪ (হায়া, যৌন সচেতনতা ও ডিজিটাল আসক্তি নিরসন)।
- **Description (BN)**: `তরুণ প্রজন্মের মাঝে ইসলামি শালীনতা (হায়া) ও চারিত্রিক পবিত্রতা বৃদ্ধি, ডিজিটাল পর্নোগ্রাফি ও মাদকাসক্তি প্রতিরোধ এবং প্রাক-বিবাহ নৈতিক কাউন্সেলিং পরিচালনা।`
- **Location**: ২৩ জেলা ও ৫০০+ শিক্ষাপ্রতিষ্ঠান
- **Timeframe**: বার্ষিক রাজ্য ক্যাম্পেইন
- **Key Highlights**:
  1. `ক্যাম্পাসে পথনাটিকা, ডকুমেন্টারি প্রদর্শন ও পোস্টারিং` (Street theatre, documentary screenings & poster drives)
  2. `মাদকাসক্তি নিরাময় কাউন্সেলিং ডেস্ক ও হেল্পলাইন` (Addiction recovery counseling desks & helplines)
  3. `ম্যারাথন দৌড় ও যুব নৈতিক শপথ গ্রহণ` (Youth marathons and collective ethical pledges)
  1. `মাদক ও পর্নোগ্রাফিমুক্ত জীবনের জন্য শপথ গ্রহণ`
  2. `প্রাক-বিবাহ সচেতনতা ও পারিবারিক মূল্যবোধ কর্মশালা`
  3. `২৪/৭ যুব মানসিক স্বাস্থ্য ও কাউন্সেলিং ডেস্ক`.

#### Card 3.3: National Tazkiyah Campaign & Unit Quran Reading Circles
- **ID**: `camp-3`
- **Status**: `active` (`চলমান`)
- **Verified Metric**: `৫০০+ ইউনিট সার্কেল ও ইনফাক সপ্তাহ` (500+ Active Reading Circles)
- **Title (BN)**: `জাতীয় তাজকিয়া অভিযান ও ইউনিট কুরআন পাঠ চক্র`
- **Title (EN)**: `National Tazkiyah Campaign, Unit Quran Circles & Infaaq Drive`
- **Policy Alignment**: পলিসি পৃষ্ঠা ১০ ও ২৪ (আত্মশুদ্ধি, ফরজ সালাত, তাজকিয়া গাইড ও ইনফাক সপ্তাহ)।
- **Description (BN)**: `প্রতিটি ইউনিটে বাধ্যতামূলক কুরআন অধ্যয়ন সার্কেল পরিচালনা, আখেরাতের চিন্তা (Fikr-e-aakhirat) জাগ্রতকরণ, মুদাররিস-ই-কুরআন প্রশিক্ষণ এবং সদস্যদের জন্য ব্যক্তিগত আত্মমূল্যায়ন (মুহাসাবা)।`
- **Location**: সমগ্র পশ্চিমবঙ্গ জোন (তৃণমূল ইউনিট স্তর)
- **Timeframe**: সেশন ২০২৫–২৬ নিয়মিত কার্যক্রম
- **Key Highlights**:
  1. `প্রতিটি স্থানীয় ইউনিটে সাপ্তাহিক কুরআন পাঠ চক্র বাধ্যতামূলক`
  2. `বার্ষিক জাতীয় ইনফাক সপ্তাহ ও দানশীলতার বিকাশ`
  3. `মুদাররিস-ই-কুরআন প্রশিক্ষণ ও তাজকিয়া গাইডবুক বিতরণ`.

---

### Section 4: Flagship Events Pillar Grid (`category: "events"`)
- **Focus**: Academic symposia, research conventions, and biennial student summits.
### Section 4: Flagship Events & Summits Grid (`category: "events"`)

#### Card 4.1: West Bengal State Student Conference
#### Card 4.1: West Bengal State Students Conference 2025
- **ID**: `evt-1`
- **Status**: `upcoming` (`আসন্ন`) | **Style**: `bg-[#EAF6FF] text-[#168BD4] border-[#63BDFF]/30`
- **Verified Impact Metric**: `১৫,০০০+ প্রতিনিধি` (15,000+ Delegates)
- **Title (BN)**: `পশ্চিমবঙ্গ রাজ্য ছাত্র সম্মেলন ২০২৪`
- **Title (EN)**: `West Bengal State Student Conference 2024`
- **Description (BN)**: `জ্ঞান, চরিত্র ও কর্মের মাধ্যমে সমাজ পুনর্গঠনের আহ্বানে রাজ্যের বিভিন্ন জেলা থেকে হাজার হাজার শিক্ষার্থী ও শিক্ষাবিদদের মিলনমেলা।`
- **Description (EN)**: `Flagship biennial student convention gathering thousands of delegates, academic thinkers, and student leaders in Kolkata.`
- **Location (BN/EN)**: `কলকাতা কনভেনশন সেন্টার` / `Kolkata Convention Centre`
- **Timeframe (BN/EN)**: `আসন্ন অনুষ্ঠান` / `Upcoming Event`
- **Status**: `upcoming` (`আসন্ন`)
- **Verified Metric**: `১৫,০০০+ প্রতিনিধি ও ছাত্র নেতৃত্ব` (15,000+ Student Delegates)
- **Title (BN)**: `পশ্চিমবঙ্গ রাজ্য ছাত্র সম্মেলন ২০২৫`
- **Title (EN)**: `West Bengal State Student Conference 2025`
- **Description (BN)**: `রাজ্যের সকল কলেজ, বিশ্ববিদ্যালয় ও মাদরাসা শিক্ষার্থীদের অংশগ্রহণে দ্বিভাষিক শিক্ষা সনদ পেশ, ইনসাফ ও ভ্রাতৃত্বের সমাজ বিনির্মাণের ঐতিহাসিক মহাসম্মেলন।`
- **Location**: মিলন মেলা প্রাঙ্গণ / কনভেনশন সেন্টার, কলকাতা
- **Timeframe**: নভেম্বর ২০২৫
- **Key Highlights**:
  1. `জাতীয় স্তরের শীর্ষস্থানীয় স্কলার ও শিক্ষাবিদদের বক্তব্য` (Keynotes from national scholars and educators)
  2. `বিশেষ অ্যাকাডেমিক সেমিনার ও প্যানেল ডিসকাশন` (Specialized academic panel discussions)
  3. `ছাত্র মেধা সংবর্ধনা ও সাংস্কৃতিক পরিবেশনা` (Academic felicitations and cultural exhibitions)
  1. `৪ দফা ঐতিহাসিক ছাত্র শিক্ষা সনদ ঘোষণা`
  2. `জাতীয় ও আন্তর্জাতিক বুদ্ধিজীবীদের উন্মুক্ত অ্যাকাডেমিক প্যানেল`
  3. `কৃতি শিক্ষার্থী ও সমাজসেবীদের বিশেষ সম্মাননা স্মারক`.

#### Card 4.2: Annual Academic Research Conclave (CERT WB)
#### Card 4.2: History Summit, Indian Knowledge System & CERT Conclave
- **ID**: `evt-2`
- **Status**: `upcoming` (`আসন্ন`)
- **Verified Impact Metric**: `৪০+ গবেষণাপত্র উপস্থাপন` (40+ Research Papers Presented)
- **Title (BN)**: `বার্ষিক অ্যাকাডেমিক রিসার্চ কনক্লেভ (CERT)`
- **Title (EN)**: `Annual Academic Research Conclave (CERT)`
- **Description (BN)**: `উচ্চশিক্ষা গবেষক ও শিক্ষকদের অংশগ্রহণে শিক্ষানীতি, ড্রপআউট পরিসংখ্যান ও আধুনিক শিখন পদ্ধতির ওপর জাতীয় কনফারেন্স।`
- **Description (EN)**: `Annual research presentation summit featuring empirical research papers on minority education and school pedagogy.`
- **Location (BN/EN)**: `যাদবপুর ক্যাম্পাস ও অডিটোরিয়াম` / `Jadavpur Campus & Auditorium`
- **Timeframe (BN/EN)**: `অক্টোবর ২০২৪` / `October 2024`
- **Verified Metric**: `৪০+ গবেষণাপত্র ও মনোগ্রাফ প্রকাশ` (40+ Peer-Reviewed Papers)
- **Title (BN)**: `হিস্ট্রি সামিট ও ভারতীয় জ্ঞানব্যবস্থা (IKS) অ্যাকাডেমিক কনক্লেভ`
- **Title (EN)**: `History Summit, Indian Knowledge System (IKS) & CERT Academic Conclave`
- **Policy Alignment**: পলিসি পৃষ্ঠা ১৭ ও ২৬ (পাঠ্যপুস্তকে ইতিহাস বিকৃতি রোধ ও অ্যাকাডেমিক গবেষণা)।
- **Description (BN)**: `উপমহাদেশের ইতিহাস বিকৃতি প্রতিরোধ, মুসলিম ঐতিহ্যের বস্তুনিষ্ঠ মূল্যায়ন এবং শিক্ষানীতি পর্যালোচনায় শীর্ষ গবেষক ও অধ্যাপকদের অংশগ্রহণে অ্যাকাডেমিক সিম্পোজিয়াম।`
- **Location**: যাদবপুর বিশ্ববিদ্যালয় ও আলিয়া বিশ্ববিদ্যালয়
- **Timeframe**: অক্টোবর ২০২৫
- **Key Highlights**:
  1. `পিয়ার-রিভিউড জার্নাল প্রকাশনা ও পুরস্কার` (Peer-reviewed journal publishing & research awards)
  2. `নীতিমালা নির্ধারক ও গবেষকদের গোলটেবিল বৈঠক` (Roundtables between policymakers and scholars)
  3. `স্টুডেন্ট রিসার্চ গ্রান্ট ঘোষণা` (Announcement of competitive student research grants)
  1. `পাঠ্যপুস্তকে বিকৃতি ও ইতিহাস পুনর্লিখনের ওপর বৈজ্ঞানিক পর্যালোচনা`
  2. `সিইআরটি বার্ষিক শিক্ষা সমীক্ষা ও ড্রপ-আউট রিপোর্ট প্রকাশ`
  3. `তরুণ ইতিহাস গবেষকদের জন্য সেরা পেপার অ্যাওয়ার্ড`.

#### Card 4.3: An Noor Literature & Cultural Festival 2.0
- **ID**: `evt-3`
- **Status**: `upcoming` (`আসন্ন`)
- **Verified Metric**: `১,৫০০+ তরুণ লেখক, কবি ও শিল্পী` (1,500+ Young Creators)
- **Title (BN)**: `আন নূর জাতীয় সাহিত্য ও সংস্কৃতি উৎসব ২.০`
- **Title (EN)**: `An Noor Literature & Cultural Festival 2.0`
- **Policy Alignment**: পলিসি পৃষ্ঠা ২০-২১ ও ২৭ ('আল-জামিল' দর্শন, সুস্থ সংস্কৃতি ও বঙ্গীয় সাহিত্য চর্চা)।
- **Description (BN)**: `ইসলামি নন্দনতত্ত্বের আলোকে সাহিত্য, কবিতা, সাংবাদিকতা, ক্যালিগ্রাফি এবং চারুকলায় মুসলিম তরুণদের সৃজনশীল প্রতিভার বিকাশ সম্মেলন।`
- **Location**: কলকাতা ও জেলা শিল্প একাডেমি
- **Timeframe**: জানুয়ারি ২০২৬
- **Key Highlights**:
  1. `বাংলা কবিতা আবৃত্তি, ছোটগল্প ও চিত্রাঙ্কন প্রতিযোগিতা`
  2. `ইসলামিক ক্যালিগ্রাফি ও ভিজ্যুয়াল আর্ট এক্সিবিশন`
  3. `বঙ্গীয় মুসলিম সাহিত্যের ঐতিহাসিক অবদান বিষয়ক সিম্পোজিয়াম`.

---

### Section 5: Educational Programs Pillar Grid (`category: "education"`)
- **Focus**: Academic empowerment, competitive talent identification, and inclusive study resources.
### Section 5: Educational Programs Grid (`category: "education"`)

#### Card 5.1: State Talent Search Examination (STSE)
#### Card 5.1: Project InQhab — University Admissions & Higher Ed Academy
- **ID**: `edu-1`
- **Status**: `active` (`চলমান`)
- **Verified Impact Metric**: `৩৫,০০০+ পরীক্ষার্থী` (35,000+ Examinees Annually)
- **Title (BN)**: `রাজ্য বিজ্ঞান মেধা অন্বেষণ পরীক্ষা (STSE)`
- **Title (EN)**: `State Talent Search Examination (STSE)`
- **Description (BN)**: `অষ্টম থেকে দশম শ্রেণির ছাত্র-ছাত্রীদের বিজ্ঞান ও গণিত প্রতিভা যাচাই, ক্যারিয়ার গাইডেন্স এবং নগদ শিক্ষাবৃত্তি প্রদান।`
- **Description (EN)**: `Prestigious talent hunt examination assessing science, mathematics, and logical reasoning among school students across Bengal.`
- **Location (BN/EN)**: `রাজ্যের ২৫০+ পরীক্ষা কেন্দ্র` / `250+ Centers Across Bengal`
- **Timeframe (BN/EN)**: `প্রতি বছর ডিসেম্বর` / `Annually in December`
- **Verified Metric**: `৫,০০০+ শিক্ষার্থী ভর্তি প্রশিক্ষণ` (5,000+ Students Mentored)
- **Title (BN)**: `প্রজেক্ট ইনকাব (InQhab) — বিশ্ববিদ্যালয় ভর্তি ও উচ্চশিক্ষা একাডেমি`
- **Title (EN)**: `Project InQhab — University Admissions & Higher Education Academy`
- **Policy Alignment**: পলিসি পৃষ্ঠা ১৫ ও ২৫ (বিশ্ববিদ্যালয় ভর্তি সহায়তা ও ফ্রেমওয়ার্ক)।
- **Description (BN)**: `কেন্দ্রীয় ও রাজ্য বিশ্ববিদ্যালয়সমূহে (JNU, AMU, Jamia, DU, Presidency, Jadavpur, Aliah) অনগ্রসর শিক্ষার্থীদের ভর্তির প্রবেশিকা পরীক্ষার প্রস্তুতি, ফ্রি কোচিং এবং স্কলারশিপ সহায়তা।`
- **Location**: অনলাইন পোর্টাল ও ১২টি অফলাইন লার্নিং সেন্টার
- **Timeframe**: সারা বছর চলমান
- **Key Highlights**:
  1. `শীর্ষ ১০০ মেধাবী শিক্ষার্থীর জন্য নগদ মেধা বৃত্তি` (Cash scholarships for top 100 meritorious students)
  2. `সায়েন্স এক্সিবিশন ও মডেল মেকিং প্রতিযোগিতা` (Science project exhibitions & model-making tournaments)
  3. `ক্যারিয়ার কাউন্সেলিং ও মেন্টরশিপ সাপোর্ট` (Personalized career counseling & ongoing mentorship)
  1. `CUET ও বিশ্ববিদ্যালয় প্রবেশিকা পরীক্ষার ফ্রি মক টেস্ট`
  2. `প্রখ্যাত বিশ্ববিদ্যালয়ের সাবেক গবেষকদের মেন্টরশিপ`
  3. `হস্টেল ও স্কলারশিপ আবেদন সহায়তা ডেস্ক`.

#### Card 5.2: Free Public Library & Digital Book Bank Network
#### Card 5.2: State Talent Search Examination (STSE)
- **ID**: `edu-2`
- **Status**: `active` (`চলমান`)
- **Verified Impact Metric**: `১২,০০০+ বই সংরক্ষিত` (12,000+ Books in Circulation)
- **Title (BN)**: `ফ্রি লাইব্রেরি ও ডিজিটাল স্টাডি ব্যাংক নেটওয়ার্ক`
- **Title (EN)**: `Free Public Library & Digital Book Bank Network`
- **Description (BN)**: `আর্থিকভাবে অনগ্রসর শিক্ষার্থীদের জন্য পাঠ্যপুস্তক, প্রতিযোগিতামূলক পরীক্ষার বই ও ডিজিটাল স্টাডি মেটেরিয়ালের উন্মুক্ত লাইব্রেরি।`
- **Description (EN)**: `Community reading rooms and central book lending banks supporting college and school aspirants with costly textbooks.`
- **Location (BN/EN)**: `৮৫+ স্থানীয় স্টাডি সেন্টার` / `85+ Local Study Centers`
- **Timeframe (BN/EN)**: `সারা বছর উন্মুক্ত` / `Round-the-Year Access`
- **Verified Metric**: `৩৫,০০০+ পরীক্ষার্থী প্রতি বছর` (35,000+ Examinees Annually)
- **Title (BN)**: `রাজ্য বিজ্ঞান মেধা অন্বেষণ পরীক্ষা (STSE)`
- **Title (EN)**: `Statewide Science & Talent Search Examination (STSE)`
- **Description (BN)**: `পশ্চিমবঙ্গের ৭ম থেকে ১০ম শ্রেণির ছাত্রছাত্রীদের মাঝে বিজ্ঞান মনস্কতা, গণিত দক্ষতা ও নৈতিক শিক্ষার বিকাশে চার দশক ধরে পরিচালিত ঐতিহাসিক মেধা বৃত্তি পরীক্ষা।`
- **Location**: ২৫০+ পরীক্ষা কেন্দ্র (সমগ্র পশ্চিমবঙ্গ)
- **Timeframe**: প্রতি বছর অক্টোবর–ডিসেম্বর
- **Key Highlights**:
  1. `সেমিস্টারভিত্তিক রেফারেন্স বই ইস্যু সুবিধা` (Semester-long reference textbook lending)
  2. `ডিজিটাল ই-বুক রিডিং ট্যাব ও কম্পিউটার হাব` (Digital tablets & e-resource computer stations)
  3. `সাপ্তাহিক গ্রুপ স্টাডি ও ক্লিয়ারিং ক্লাসেস` (Weekly peer group studies & doubt-clearing clinics)
  1. `রাজ্য ও জেলা স্তরে মেধা বৃত্তি ও ল্যাপটপ পুরস্কার`
  2. `উচ্চশিক্ষার জন্য বিশেষ বিজ্ঞান কাউন্সেলিং শিবির`
  3. `প্রত্যন্ত গ্রামের অনগ্রসর স্কুলের শিক্ষার্থীদের বিশেষ প্রশিক্ষণ`.

---

### Section 6: Youth Activities Pillar Grid (`category: "youth"`)
- **Focus**: Moral character, leadership bootcamp retreats, sports, and creative cultural expression.
### Section 6: Youth Activities Grid (`category: "youth"`)

#### Card 6.1: Youth Leadership Summer Retreat & Personality Camp
#### Card 6.1: Youth Leadership Development & STEM Campuses Summit
- **ID**: `yth-1`
- **Status**: `active` (`চলমান`)
- **Verified Impact Metric**: `১২০০+ ক্যাম্প গ্র্যাজুয়েট` (1,200+ Trained Graduates)
- **Title (BN)**: `ইয়ুথ লিডারশিপ সামার ক্যাম্প ও ব্যক্তিত্ব উন্নয়ন`
- **Title (EN)**: `Youth Leadership Summer Retreat & Personality Camp`
- **Description (BN)**: `ছাত্রদের আত্মবিশ্বাস, পাবলিক স্পিকিং, টিমওয়ার্ক, সংগঠন পরিচালনা ও নৈতিক মূল্যবোধ বিকাশের ৩ দিনব্যাপী আবাসিক কর্মশালা।`
- **Description (EN)**: `Residential leadership training bootcamp cultivating public speaking, event management, and spiritual mindfulness.`
- **Location (BN/EN)**: `দার্জিলিং ও বাঁকুড়া রিট্রিট সেন্টার` / `Darjeeling & Bankura Retreat Centers`
- **Timeframe (BN/EN)**: `মে ও জুন মাস` / `May & June`
- **Verified Metric**: `১,২০০+ ইঞ্জিনিয়ার ও চিকিৎসক প্রশিক্ষণার্থী` (1,200+ STEM Professionals)
- **Title (BN)**: `ইয়ুথ লিডারশিপ ডেভেলপমেন্ট ও স্টেম ক্যাম্পাস সামিট`
- **Title (EN)**: `Youth Leadership Development & STEM Campuses Summit`
- **Policy Alignment**: পলিসি পৃষ্ঠা ১৮ ও ২৮ (প্রফেশনাল ও স্টেম ক্যাম্পাস নেটওয়ার্ক)।
- **Description (BN)**: `মেডিক্যাল, ইঞ্জিনিয়ারিং ও পলিটেকনিক ক্যাম্পাসের শিক্ষার্থীদের প্রযুক্তিগত উৎকর্ষ, উদ্যোক্তা হওয়ার অনুপ্রেরণা এবং সামাজিক দায়িত্ববোধে উদ্বুদ্ধকরণ।`
- **Location**: আইআইটি খড়গপুর ও সল্টলেক আইটি হাব
- **Timeframe**: সেপ্টেম্বর ২০২৫
- **Key Highlights**:
  1. `বিশেষজ্ঞ মেন্টরদের মাধ্যমে লাইফ স্কিলস ও ডিসিশন মেকিং ট্রেনিং` (Life skills and decision-making modules by expert mentors)
  2. `বিতর্ক, তাৎক্ষণিক বক্তৃতা ও লিডারশিপ সিমুলেশন` (Debates, extempore speech & organizational simulations)
  3. `আউটডোর ট্র্যাকিং ও টিম বিল্ডিং অ্যাক্টিভিটিস` (Outdoor tracking & team synergy exercises)
  1. `এআই, ডেটা সায়েন্স ও নৈতিক টেকনোলজি সেমিনার`
  2. `স্টার্টআপ ইনকিউবেশন ও বিজনেস মডেল কর্মশালা`
  3. `টেক প্রফেশনালদের সাথে ক্যারিয়ার নেটওয়ার্কিং সার্কেল`.

#### Card 6.2: Junior Fest & Creative Talent Exhibition
#### Card 6.2: Mental Wellness Forum & 24/7 Youth Helpline
- **ID**: `yth-2`
- **Status**: `upcoming` (`আসন্ন`)
- **Verified Impact Metric**: `৮,০০০+ অংশগ্রহণকারী` (8,000+ Participants)
- **Title (BN)**: `কিশোর উৎসব ও সৃজনশীল মেধা মেলা`
- **Title (EN)**: `Junior Fest & Creative Talent Exhibition`
- **Description (BN)**: `স্কুল ও কিশোর শিক্ষার্থীদের চিত্রাঙ্কন, ক্যালিগ্রাফি, প্রবন্ধ রচনা, কুইজ এবং রোবোটিক্স মডেল প্রদর্শনের মেগা উৎসব।`
- **Description (EN)**: `Vibrant creative carnival celebrating calligraphy, essay writing, quiz tournaments, and junior science projects.`
- **Location (BN/EN)**: `প্রতিটি সাংগঠনিক জেলা সদর` / `All District Headquarters`
- **Timeframe (BN/EN)**: `নভেম্বর ২০২৪` / `November 2024`
- **Status**: `active` (`চলমান`)
- **Verified Metric**: `৩,৫০০+ গোপনীয় কাউন্সেলিং সেশন` (3,500+ Confidential Sessions)
- **Title (BN)**: `যুব মানসিক স্বাস্থ্য ফোরাম ও ২৪/৭ হেল্পলাইন`
- **Title (EN)**: `Mental Wellness Forum & 24/7 Youth Helpline`
- **Policy Alignment**: পলিসি পৃষ্ঠা ১১ ও ২৫ (মানসিক সুস্থতা ও যুব মানসিক স্বাস্থ্য সাপোর্ট)।
- **Description (BN)**: `পড়াশোনার চাপ, ক্যারিয়ার হতাশা, সোশ্যাল মিডিয়া আসক্তি এবং পারিবারিক জটিলতায় ভোগা তরুণদের জন্য পেশাদার সাইকোলজিস্ট ও মেন্টরদের সার্বক্ষণিক বিনামূল্যে কাউন্সেলিং।`
- **Location**: অনলাইন পোর্টাল ও কলকাতা ওয়েলনেস সেন্টার
- **Timeframe**: ২৪/৭ সার্বক্ষণিক সেবা
- **Key Highlights**:
  1. `ইসলামি ক্যালিগ্রাফি ও পেইন্টিং প্রতিযোগিতা` (Islamic calligraphy & fine arts competition)
  2. `সাধারণ জ্ঞান ও বিজ্ঞান কুইজ টুর্নামেন্ট` (General knowledge and scientific quiz tournaments)
  3. `পুরস্কার বিতরণ ও সার্টিফিকেট প্রদান` (Merit trophy distribution & commemorative certificates)
  1. `সম্পূর্ণ গোপনীয় টেলিফোনিক কাউন্সেলিং সাপোর্ট`
  2. `ক্যাম্পাসে ডিপ্রেশন ও স্ট্রেস ম্যানেজমেন্ট কর্মশালা`
  3. `আত্মহত্যার প্রবণতা নিরসনে পিয়ার মেন্টরশিপ সেল`.

---

### Section 7: Social Welfare Pillar Grid (`category: "social"`)
- **Focus**: Humanitarian relief, 24/7 student voluntary blood donation, and natural disaster rehabilitation.
### Section 7: Social Welfare & Environment Grid (`category: "social"`)

#### Card 7.1: Statewide Emergency Blood Donors Network (Life Line)
#### Card 7.1: Parisar Samvad — Campus Eco-Dialogue & 'Imaratul Ardh'
- **ID**: `soc-1`
- **Status**: `active` (`চলমান`)
- **Verified Impact Metric**: `৬,০০০+ ইউনিট রক্তদান প্রতি বছর` (6,000+ Blood Units Donated Annually)
- **Title (BN)**: `রাজ্যব্যাপী জরুরি রক্তদাতা নেটওয়ার্ক (Life Line)`
- **Title (EN)**: `Statewide Emergency Blood Donors Network (Life Line)`
- **Description (BN)**: `পশ্চিমবঙ্গের সরকারি ও বেসরকারি হাসপাতালে মুমূর্ষু রোগীদের জরুরি রক্তের প্রয়োজনে ২৪ ঘণ্টার স্বেচ্ছাসেবী ছাত্র রক্তদাতা সেবা।`
- **Description (EN)**: `Active 24/7 student-driven voluntary blood donor registry serving critical patients across state blood banks and hospitals.`
- **Location (BN/EN)**: `সকল সরকারি মেডিক্যাল কলেজ ও হাসপাতাল` / `All Govt Medical Colleges & Hospitals`
- **Timeframe (BN/EN)**: `২৪/৭ জরুরি সেবা` / `24/7 Emergency Service`
- **Verified Metric**: `১০০+ ক্যাম্পাস ফোরাম ও ২৫,০০০+ বৃক্ষরোপণ` (100+ Campus Eco-Chapters)
- **Title (BN)**: `পরিসর সংবাদ — ক্যাম্পাস পরিবেশ ও ইকোলজি আন্দোলন ('ইমারাতুল আরদ')`
- **Title (EN)**: `Parisar Samvad — Campus Eco-Dialogue & 'Imaratul Ardh' Movement`
- **Policy Alignment**: পলিসি পৃষ্ঠা ২০ ও ২৭ (ইসলামি পরিবেশ দর্শন ও প্যারিসার সংবাদ ফোরাম)।
- **Description (BN)**: `পৃথিবীকে সুরক্ষা ও আবাদ করার ইসলামি দায়িত্ববোধ (ইমারাতুল আরদ) থেকে শিক্ষাপ্রতিষ্ঠানে পরিবেশ দূষণ, জলবায়ু সংকট ও প্লাস্টিক বর্জ্য ব্যবস্থাপনায় শিক্ষার্থীদের পরিবেশ সচেতনতা আন্দোলন।`
- **Location**: পশ্চিমবঙ্গের ৫০০+ কলেজ ও স্কুল ক্যাম্পাস
- **Timeframe**: বছরব্যাপী কর্মসূচি
- **Key Highlights**:
  1. `জেলা ও মহকুমা স্তরে তাৎক্ষণিক ভলান্টিয়ার কোঅর্ডিনেশন` (Instant district-level volunteer coordination desk)
  2. `বিশ্ব রক্তদাতা দিবসে মেগা রক্তদান শিবির` (Mega blood donation drives on World Blood Donor Day)
  3. `অনলাইন ব্লাড রিকোয়েস্ট ট্র্যাকিং ডিরেক্টরি` (Live online blood requirement registry)
  1. `ক্যাম্পাসে প্লাস্টিকমুক্ত পরিবেশ গড়ার যৌথ কর্মসূচি`
  2. `বিশ্ব পরিবেশ দিবসে রাজ্যব্যাপী ২৫,০০০ বৃক্ষরোপণ`
  3. `জল অপচয় রোধ ও বৃষ্টির জল সংরক্ষণে স্টুডেন্টস ক্যাম্পেইন`.

#### Card 7.2: Disaster Emergency Relief & Rehabilitation Mission
#### Card 7.2: Statewide Emergency Blood Donors Network (Life Line) & Disaster Relief
- **ID**: `soc-2`
- **Status**: `active` (`চলমান`)
- **Verified Impact Metric**: `৫০,০০০+ পরিবারে খাদ্য ও বস্ত্র সহায়তা` (50,000+ Families Aided)
- **Title (BN)**: `দুর্যোগে জরুরি ত্রাণ ও পুনর্বাসন কর্মসূচি`
- **Title (EN)**: `Disaster Emergency Relief & Rehabilitation Mission`
- **Description (BN)**: `ঘূর্ণিঝড়, বন্যা ও প্রাকৃতিক দুর্যোগের সময় প্রত্যন্ত অঞ্চলে শুকনা খাদ্য, বিশুদ্ধ পানি, চিকিৎসা সহায়তা এবং ঘরবাড়ি মেরামত সেবা।`
- **Description (EN)**: `Rapid humanitarian relief teams deployed during floods and cyclones delivering rations, medical aid, and shelter rehabilitation.`
- **Location (BN/EN)**: `সুন্দরবন, উত্তরবঙ্গ ও নদী তীরবর্তী এলাকা` / `Sundarbans, North Bengal & Riverine Belts`
- **Timeframe (BN/EN)**: `জরুরি সময় মোতায়েন` / `Emergency Rapid Deployment`
- **Verified Metric**: `১০,০০০+ নিবন্ধিত রক্তদাতা নেটওয়ার্ক` (10,000+ Voluntary Donors)
- **Title (BN)**: `রাজ্যব্যাপী জরুরি রক্তদাতা নেটওয়ার্ক (Life Line) ও দুর্যোগ ত্রাণ সেল`
- **Title (EN)**: `Statewide Emergency Blood Donors Network (Life Line) & Disaster Relief`
- **Description (BN)**: `পশ্চিমবঙ্গের সরকারি ও বেসরকারি হাসপাতালে মুমূর্ষু রোগীদের জন্য ২৪ ঘণ্টা স্বেচ্ছাসেবী রক্তদাতা সেবা এবং ঘূর্ণিঝড় ও বন্যায় সুন্দরবন ও উত্তরবঙ্গে জরুরি খাদ্য ও চিকিৎসা সহায়তা।`
- **Location**: সকল মেডিক্যাল কলেজ ও দুর্যোগপ্রবণ উপকূলীয় এলাকা
- **Timeframe**: ২৪/৭ সার্বক্ষণিক সেবা
- **Key Highlights**:
  1. `বোট ও ফিল্ড টিম দ্বারা দুর্গত এলাকায় ত্রাণ সরবরাহ` (Boat fleets & field dispatch into inundated river islands)
  2. `বন্যা পরবর্তী বিনামূল্যে চিকিৎসা ও ওষুধ বিতরণ ক্যাম্প` (Post-flood medical relief and prescription camps)
  3. `বার্ষিক রাজ্যব্যাপী শীতবস্ত্র বিতরণ কর্মসূচি` (Annual statewide winter clothing drives)
  1. `অনলাইন ব্লাড রিকোয়েস্ট ট্র্যাকিং ডিরেক্টরি`
  2. `ঘূর্ণিঝড়-পরবর্তী বোট ও মেডিকেল টিম দ্বারা ত্রাণ সরবরাহ`
  3. `বার্ষিক শীতবস্ত্র ও শিশু সুরক্ষা সামগ্রী বিতরণ কর্মসূচি`.

---

### Section 8: Interactive Participation & Registration Trigger
- **Component**: Client State Modal / Toast Feedback in [`src/app/activities/page.tsx`](file:///home/masyud/Development/Masyud/SIO/src/app/activities/page.tsx)
- **Interaction**:
  - Clicking `Participate / Details (অংশগ্রহণ করুন / বিস্তারিত)` opens top banner confirmation:
    - *Bengali*: `"[কার্যক্রমের নাম]" কার্যক্রমে আপনার আগ্রহ গ্রহণ করা হয়েছে! আমাদের প্রতিনিধি শীঘ্রই আপনার সাথে যোগাযোগ করবেন।`
    - *English*: `Your participation interest for "[Activity Name]" has been noted. Our team will reach out soon.`
  - Clicking `Inquire (প্রশ্ন করুন →)` smoothly routes to `/contact#form` with context.
## 4. Master Activities Reference Table (12 Flagship Initiatives)

---

### Section 9: Student Movement & Volunteer CTA Banner
- **Component**: High-Impact Call to Action Banner
- **Background**: Solid Deep Blue (`#0F4C81`) with White Typography

| Element | Bengali (`bn`) | English (`en`) |
| :--- | :--- | :--- |
| **Eyebrow Badge** | `দেশ ও সমাজের সেবায় চার দশক` | `Four Decades of Student Leadership` |
| **Heading** | `আপনার এলাকায় বা ক্যাম্পাসে আমাদের কার্যক্রমে যুক্ত হতে চান?` | `Want to Organize or Participate in SIO Initiatives?` |
| **Description** | `শিক্ষা সংস্কার, রক্তদান ক্যাম্প কিংবা চরিত্র গঠন শিবিরে স্বেচ্ছাসেবক হিসেবে কাজ করতে আমাদের রাজ্য বা জেলা প্রতিনিধির সাথে যোগাযোগ করুন।` | `Connect with our state and district representatives to volunteer in educational, humanitarian, and youth development programs.` |
| **Primary Button** | `যোগাযোগ করুন →` (`/contact`) | `Get in Touch →` (`/contact`) |
| **Secondary Button** | `শিক্ষার্থী কর্নার দেখুন` (`/student-corner`) | `Visit Student Corner` (`/student-corner`) |

---

### Section 10: Master Black Footer
- **Component File**: [`src/components/layout/footer.tsx`](file:///home/masyud/Development/Masyud/SIO/src/components/layout/footer.tsx)
- **Background**: `#0F172A`
- **Key Features**: 24/7 Student Helpline (`+91 12345 67890`), State Headquarters location (Kolkata), Social feeds, Quick links, and Google Maps location embed.

---

## 5. Master Activities Reference Table (10 Core Initiatives)

| ID | Category | Title (Bengali & English) | Verified Metric | Status | Location | Timeframe |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `camp-1` | `campaigns` | **রাজ্য শিক্ষা অধিকার ও ক্যাম্পাস গণতন্ত্র রক্ষা অভিযান**<br>`Statewide Right to Education Campaign` | ১,০০,০০০+ স্বাক্ষর | Active | সকল বিশ্ববিদ্যালয় ও জেলা | চলমান অভিযান |
| `camp-2` | `campaigns` | **নৈতিক চরিত্র ও মাদকবিরোধী সচেতনতা সপ্তাহ**<br>`Moral Character & Anti-Drug Drive` | ৫০,০০০+ শপথপত্র | Active | ২৩ জেলা ও ৫০০+ ক্যাম্পাস | বার্ষিক অভিযান |
| `evt-1` | `events` | **পশ্চিমবঙ্গ রাজ্য ছাত্র সম্মেলন ২০২৪**<br>`WB State Student Conference 2024` | ১৫,০০০+ প্রতিনিধি | Upcoming | কলকাতা কনভেনশন সেন্টার | আসন্ন অনুষ্ঠান |
| `evt-2` | `events` | **বার্ষিক অ্যাকাডেমিক রিসার্চ কনক্লেভ (CERT)**<br>`Annual Academic Research Conclave` | ৪০+ গবেষণাপত্র | Upcoming | যাদবপুর বিশ্ববিদ্যালয় | অক্টোবর ২০২৪ |
| `edu-1` | `education` | **রাজ্য বিজ্ঞান মেধা অন্বেষণ পরীক্ষা (STSE)**<br>`State Talent Search Exam (STSE)` | ৩৫,০০০+ পরীক্ষার্থী | Active | ২৫০+ পরীক্ষা কেন্দ্র | প্রতি বছর ডিসেম্বর |
| `edu-2` | `education` | **ফ্রি লাইব্রেরি ও ডিজিটাল স্টাডি ব্যাংক নেটওয়ার্ক**<br>`Free Public Library & Book Bank` | ১২,০০০+ বই | Active | ৮৫+ স্টাডি সেন্টার | সারা বছর উন্মুক্ত |
| `yth-1` | `youth` | **ইয়ুথ লিডারশিপ সামার ক্যাম্প ও ব্যক্তিত্ব উন্নয়ন**<br>`Youth Leadership Summer Retreat` | ১২০০+ গ্র্যাজুয়েট | Active | দার্জিলিং ও বাঁকুড়া | মে ও জুন মাস |
| `yth-2` | `youth` | **কিশোর উৎসব ও সৃজনশীল মেধা মেলা**<br>`Junior Fest & Creative Talent Expo` | ৮,০০০+ অংশগ্রহণকারী | Upcoming | প্রতিটি জেলা সদর | নভেম্বর ২০২৪ |
| `soc-1` | `social` | **রাজ্যব্যাপী জরুরি রক্তদাতা নেটওয়ার্ক (Life Line)**<br>`Statewide Emergency Blood Donors Network` | ৬,০০০+ ইউনিট/বছর | Active | সকল মেডিক্যাল কলেজ | ২৪/৭ জরুরি সেবা |
| `soc-2` | `social` | **দুর্যোগে জরুরি ত্রাণ ও পুনর্বাসন কর্মসূচি**<br>`Disaster Relief & Rehabilitation Mission` | ৫০,০০০+ পরিবার | Active | সুন্দরবন ও উত্তরবঙ্গ | জরুরি সময় মোতায়েন |
| ID | Category | Title (Bengali & English) | Verified Metric | Status | Location | Timeframe | Policy Reference |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| `camp-1` | `campaigns` | **শিক্ষা অধিকার ও ছাত্র সংসদ পুনর্বহাল অভিযান**<br>`Campus Democracy & Student Union Campaign` | ১,০০,০০০+ স্বাক্ষর | Active | সকল বিশ্ববিদ্যালয় | সেশন ২০২৫–২৬ | পলিসি পৃষ্ঠা ১৮ |
| `camp-2` | `campaigns` | **চারিত্রিক শালীনতা ও মাদকবিরোধী সপ্তাহ**<br>`Sexual Morality & Anti-Addiction Week` | ৫০,০০০+ শপথপত্র | Active | ২৩ জেলা ও ক্যাম্পাস | বার্ষিক অভিযান | পলিসি পৃষ্ঠা ১১, ২৪ |
| `camp-3` | `campaigns` | **জাতীয় তাজকিয়া অভিযান ও কুরআন পাঠ চক্র**<br>`National Tazkiyah & Quran Circles` | ৫০০+ ইউনিট সার্কেল | Active | রাজ্য ইউনিট স্তর | নিয়মিত কার্যক্রম | পলিসি পৃষ্ঠা ১০, ২৪ |
| `evt-1` | `events` | **পশ্চিমবঙ্গ রাজ্য ছাত্র সম্মেলন ২০২৫**<br>`WB State Student Conference 2025` | ১৫,০০০+ প্রতিনিধি | Upcoming | মিলন মেলা, কলকাতা | নভেম্বর ২০২৫ | দ্বিবার্ষিক সেশন |
| `evt-2` | `events` | **হিস্ট্রি সামিট ও আইকেএস কনক্লেভ (CERT)**<br>`History Summit & IKS Conclave` | ৪০+ গবেষণাপত্র | Upcoming | যাদবপুর বিশ্ববিদ্যালয় | অক্টোবর ২০২৫ | পলিসি পৃষ্ঠা ১৭, ২৬ |
| `evt-3` | `events` | **আন নূর জাতীয় সাহিত্য উৎসব ২.০**<br>`An Noor Literature Festival 2.0` | ১,৫০০+ তরুণ লেখক | Upcoming | কলকাতা আর্ট গ্যালারি | জানুয়ারি ২০২৬ | পলিসি পৃষ্ঠা ২০, ২৭ |
| `edu-1` | `education` | **উচ্চশিক্ষা একাডেমি 'Project InQhab'**<br>`Project InQhab Admissions Academy` | ৫,০০০+ শিক্ষার্থী | Active | অনলাইন ও ১২ কেন্দ্র | সারা বছর | পলিসি পৃষ্ঠা ১৫, ২৫ |
| `edu-2` | `education` | **রাজ্য বিজ্ঞান মেধা অন্বেষণ পরীক্ষা (STSE)**<br>`State Talent Search Exam (STSE)` | ৩৫,০০০+ পরীক্ষার্থী | Active | ২৫০+ কেন্দ্র | অক্টোবর–ডিসেম্বর | বার্ষিক ফ্ল্যাগশিপ |
| `yth-1` | `youth` | **লিডারশিপ ডেভেলপমেন্ট ও স্টেম সামিট**<br>`Leadership Dev. & STEM Campuses` | ১,২০০+ গ্র্যাজুয়েট | Active | আইআইটি খড়গপুর | সেপ্টেম্বর ২০২৫ | পলিসি পৃষ্ঠা ১৮, ২৮ |
| `yth-2` | `youth` | **মানসিক স্বাস্থ্য ফোরাম ও ২৪/৭ হেল্পলাইন**<br>`Mental Wellness Forum & Helpline` | ৩,৫০০+ কাউন্সেলিং | Active | সার্বক্ষণিক অনলাইন | ২৪/৭ লাইভ | পলিসি পৃষ্ঠা ১১, ২৫ |
| `soc-1` | `social` | **পরিসর সংবাদ — ক্যাম্পাস পরিবেশ আন্দোলন**<br>`Parisar Samvad Eco-Dialogue Movement` | ১০০+ ক্যাম্পাস ফোরাম | Active | রাজ্য ক্যাম্পাসসমূহ | বছরব্যাপী | পলিসি পৃষ্ঠা ২০, ২৭ |
| `soc-2` | `social` | **জরুরি রক্তদাতা নেটওয়ার্ক Life Line ও ত্রাণ**<br>`Statewide Blood Donors & Relief Cell` | ১০,০০০+ রক্তদাতা | Active | সকল মেডিক্যাল কলেজ | ২৪/৭ জরুরি সেবা | মানবসেবা সেল |
