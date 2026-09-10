# SIO West Bengal — About Page Wireframe & Name-Wise Content Blueprint

This document specifies the complete architectural wireframe, layout blueprints, and section-by-section name-wise content matrix for the official **SIO West Bengal About Page** ([`src/app/about/page.tsx`](file:///home/masyud/Development/Masyud/SIO/src/app/about/page.tsx)).
> **Document Status**: Production Ready & Fully Aligned with Official SIO Constitution (Amended Dec 2022) & Policy & Programme (2025–2026 / 22nd Term)  
> **Target Route**: `/about`  
> **Source File**: [`src/app/about/page.tsx`](file:///home/masyud/Development/Masyud/SIO/src/app/about/page.tsx)  
> **Design Pattern**: Comprehensive Institutional Showcase, Constitutional Philosophy & Preamble, Mission & Six Core Objectives, Tri-Modal Methodology, 2025–2026 Session Vision, Four-Decade Milestone Timeline, Four-Tier Governance, and Membership Pathway Gateway.

---

## 1. High-Level Architectural Flow & Wireframe Diagram

```mermaid
flowchart TD
    subgraph S0["0. Top Navigation & Header Bar (Sticky)"]
        A0["[Official SIO Emblem] SIO WEST BENGAL | Students Islamic Org of India"] --- B0["Desktop Navigation Menu (About highlighted)"] --- C0["Search | Lang Switcher (বাংলা/EN) | Mobile Hamburger"]
    end

    subgraph S1["1. Hero Showcase Section (White)"]
        H1A["H1: 'আমাদের সম্পর্কে' (About Us) + Blue Accent Line"]
        H1B["Intro Narrative: Student leadership in the light of Divine Guidance for 4+ decades"]
        H1C["Right Col Graphic: Architectural Islamic Arch Motif + SIO West Bengal Badge"]
        H1A["H1: 'আমাদের সম্পর্কে' (About Us) + Blue Accent Line (#168BD4)"]
        H1B["Pill: 'প্রতিষ্ঠিত ১৯৮২ • ১লা মুহাররম ১৪০৩ হিজরি • সেশন ২০২৫–২৬ (২২তম টার্ম)'"]
        H1C["Session Theme: 'Illuminating Society with the Light of Divine Guidance'"]
        H1D["Right Col Graphic: Architectural Islamic Arch Motif + SIO West Bengal Landmark Seal"]
    end

    subgraph S2["2. Our Mission & Objectives (#F7FAFC)"]
    subgraph S2["2. Constitutional Philosophy & Preamble Callout (#EAF6FF)"]
        CP1["Philosophical Premise: আল্লাহর সার্বভৌমত্ব, মানুষের বিবেক ও স্বাধিকার, এবং সার্বজনীন নববী নির্দেশনা"]
        CP2["Ultimate Driving Motivation: 'The sole motivating factor is the pleasure of Allah in the Hereafter'"]
    end

    subgraph S3["3. Mission & Six Constitutional Objectives (#F7FAFC)"]
        M2A["Card 1: 'আমাদের মিশন' (Our Mission) — Article 4(A)"]
        M2B["Card 2: 'আমাদের উদ্দেশ্য' (Our Objectives) — Article 4(B)"]
        M2C["Interactive CTA: [বিস্তারিত দেখুন →] (Opens Constitutional Detail Modal)"]
        M2B["Card 2: '৬টি সাংবিধানিক উদ্দেশ্য' (6 Core Objectives) — Article 4(B)"]
        M2C["Interactive CTA: [সংবিধানের বিস্তারিত পাঠ দেখুন →] (Opens Full Constitutional Modal)"]
    end

    subgraph S3["3. Our Ideals & Methodology (White)"]
        ID1["1. কুরআন ও সুন্নাহ<br/>(Qur'an & Sunnah)"]
        ID2["2. সৎ, শান্তিপূর্ণ ও গঠনমূলক<br/>(Peaceful & Constructive)"]
        ID3["3. ছাত্র ও যুব কেন্দ্রিক<br/>(Student Centered)"]
        ID4["4. চরিত্র গঠন<br/>(Character Building)"]
        ID5["5. ব্যক্তি-সমাজ-জাতির উন্নয়ন<br/>(Societal Elevation)"]
    subgraph S4["4. Tri-Modal Constitutional Methodology & Ethical Bounds (White)"]
        ID1["১. কুরআন ও সুন্নাহর দিকনির্দেশনা<br/>(ধারা ৫.১: সকল কাজের মূল ভিত্তি)"]
        ID2["২. কঠোর নৈতিকতার অনুশাসন<br/>(ধারা ৫.২: সততা ও আত্মশুদ্ধি)"]
        ID3["৩. শান্তিপূর্ণ ও গঠনমূলক পন্থা<br/>(ধারা ৫.৩: যুক্তি, সম্প্রীতি ও বিভেদহীনতা)"]
    end

    subgraph S4["4. Our Journey — Aceternity Milestone Timeline (#F7FAFC)"]
    subgraph S5["5. Our Journey — Aceternity Milestone Timeline (#F7FAFC)"]
        TJ0["Header Badge: '১৯৮২ — ২০২৬ • চার দশকেরও বেশি ছাত্র নেতৃত্ব'"]
        TJ1["Milestone 1: ১৯৮২ (The Genesis & Foundation) + 2 Image Cards"]
        TJ2["Milestone 2: ১৯৯০ — ২০০০ (Campus Expansion & Movement) + 2 Image Cards"]
        TJ3["Milestone 3: ২০১০ — ২০২০ (Research & Mega Conferences) + 2 Image Cards"]
        TJ4["Milestone 4: ২০২৬ ও আগামী দিন (Present Stature & Future Horizon) + 2 Image Cards"]
        TJ1["Milestone 1: ১৯৮২ (The Genesis & Foundation) + 2 Archival Photo Cards"]
        TJ2["Milestone 2: ১৯৯০ — ২০০০ (Campus Expansion & Democratic Rights) + 2 Image Cards"]
        TJ3["Milestone 3: ২০১০ — ২০২০ (CERT Research, BTF & State Conferences) + 2 Image Cards"]
        TJ4["Milestone 4: ২০২৫ — ২০২৬ ও আগামী দিন (22nd Term, Policy Planks & Digital Ethics) + 2 Image Cards"]
    end

    subgraph S5["5. Organizational Structure & Leadership Link (White)"]
        OS1["Tier 1: কেন্দ্রীয় কাঠামো (Central CAC)"]
        OS2["Tier 2: জোনাল কাঠামো (West Bengal ZAC)"]
        OS3["Tier 3: স্থানীয় ইউনিট (23 Districts)"]
        OS4["Tier 4: শাখা/প্রকল্প (Campus & Units)"]
        OS5["High-Impact Banner: 'রাজ্য সভাপতি, সম্পাদকমণ্ডলী ও জেলা নেতৃত্ব দেখুন' → [নেতৃত্ব পৃষ্ঠা দেখুন]"]
    subgraph S6["6. Four-Tier Democratic Governance & Institutional Integrity (White)"]
        OS1["Tier 1: কেন্দ্রীয় কাঠামো (National CAC - 15 Members & President)"]
        OS2["Tier 2: জোনাল কাঠামো (West Bengal ZAC & Secretariat)"]
        OS3["Tier 3: জেলা ও বিভাগীয় স্তর (23 Districts Leadership)"]
        OS4["Tier 4: স্থানীয় ও ক্যাম্পাস ইউনিট (Articles 38-41: Institutional Cells)"]
        OS5["Constitutional Hallmarks: দ্বিবার্ষিক সেশন (ধারা ৮) • পদলিপ্সাহীন নেতৃত্ব (ধারা ৭) • অডিটকৃত বায়তুলমাল (ধারা ৪২-৪৭)"]
        OS6["Leadership Banner: '২০২৫–২৬ সেশনের রাজ্য নেতৃত্ব দেখুন' → [নেতৃত্ব ডিরেক্টরি]"]
    end

    subgraph S6["6. Join Movement Banner (#EAF6FF)"]
        JM1["Silhouette Background Graphic + H2: 'আপনিও যুক্ত হন'"]
        JM2["Narrative: 'আদর্শ সমাজ গঠনের এই মহান কাজে আপনিও অংশ নিন...'"]
        JM3["Action CTA: [যোগ দিন এখনই →] (Linked to /contact)"]
    subgraph S7["7. Constitutional Membership Criteria & Youth Gateway (#EAF6FF)"]
        JM1["Badge: 'সদস্যপদ শর্তাবলি • ধারা ৬'"]
        JM2["4 Pillars: ভারতীয় নাগরিক (অনূর্ধ্ব ৩০ বছর) • সংবিধানের আনুগত্য • নিয়মিত সালাত ও ফরজ পালন • কবিরা গুনাহ বর্জন"]
        JM3["Action CTA: [আন্দোলনে যুক্ত হোন এখনই →] (Linked to /contact)"]
    end

    subgraph S7["7. Newsletter Strip (#0F4C81) & 8. Master Black Footer (#0B0F17)"]
    subgraph S8["8. Newsletter Strip (#0F4C81) & 9. Master Black Footer (#0B0F17)"]
        NL1["ইমেইল ইনপুট + [সাবস্ক্রাইব করুন] বাটন"]
        FT1["Brand Info + Socials + 24/7 Availability Pill + Sitemap + 14 Alimuddin St Map + Copyright"]
        FT1["কেন্দ্রীয় দফতর (নয়া দিল্লি) + রাজ্য দফতর (কলকাতা) + ২৪/৭ হেল্পলাইন + সোশ্যাল মিডিয়া + কপিরাইট"]
    end

    subgraph SM["[Interactive Modal] Constitutional Detail Modal (Article 4)"]
    subgraph SM["[Interactive Modal] Constitutional Detail Modal (Articles 4, 5 & 6)"]
        MD1["Article 4(A) Mission Statement"]
        MD2["Article 4(B) 6-Point Constitutional Objectives List"]
        MD3["Dec 2022 Amendment Citation + Close Button"]
        MD2["Article 4(B) Complete 6-Point Constitutional Objectives"]
        MD3["Article 5 Methodology & Article 6 Membership Conditions"]
    end

    S0 --> S1 --> S2 --> S3 --> S4 --> S5 --> S6 --> S7
    S0 --> S1 --> S2 --> S3 --> S4 --> S5 --> S6 --> S7 --> S8
    M2C -.-> SM
```

---

## 2. Name-Wise Content Matrix & Layout Blueprint

### Section 0: Sticky Navigation Header (`Header`)
- **Container / Height**: `w-full h-[74px] md:h-[84px] bg-white/95 backdrop-blur-md border-b border-[#E5E7EB]`
- **Container / Height**: `w-full h-[74px] md:h-[84px] bg-white/95 backdrop-blur-md border-b border-[#E5E7EB] sticky top-0 z-50`
- **Active Navigation Pill**: "আমাদের সম্পর্কে" (`/about`) highlighted in `#168BD4` with blue baseline accent indicator.
- **Brand Identity**: Authentic official SIO circular watercolor emblem (56px) + `SIO WEST BENGAL` + `Students Islamic Organisation of India`.

---

### Section 1: Hero Showcase (`/about#top`)
### Section 1: Hero Showcase & Institutional Heritage (`/about#top`)
- **Visual Wireframe**:
  ```
  +-----------------------------------------------------------------------------------+
  | Left Column:                                | Right Column:                       |
  | [Badge: পশ্চিমবঙ্গ জোন • প্রতিষ্ঠিত ১৯৮২ • সেশন ২০২৫–২৬ (২২তম টার্ম)]               |
  | H1: আমাদের সম্পর্কে (About Us)               | [ Architectural Arch Motif Card:    |
  | [ Blue Accent Line: w-14 h-1 ]              |   - Building2 Icon in Circle        |
  | [ Blue Accent Line: w-14 h-1 ]              |   - Building2 Icon & SIO Emblem     |
  |                                             |   - 'স্টুডেন্টস ইসলামিক অর্গানাইজেশন  |
  | Body: ইসলামের আলোকে ছাত্র ও যুব সমাজকে গড়ে  |     অব ইন্ডিয়া'                     |
  | তোলা এবং ব্যক্তি, সমাজ ও জাতির পুনর্গঠনের   |   - 'পশ্চিমবঙ্গ জোন • প্রতিষ্ঠিত ১৯৮২'|
  | লক্ষ্য অর্জন করে যাওয়া SIO-র মূল লক্ষ্য...  | ]                                   |
  | Theme: "দ্বীনি নির্দেশনার আলোয় সমাজ পুনর্গঠন"   |     অব ইন্ডিয়া'                     |
  |                                             |   - 'প্রতিষ্ঠিত: ১লা মুহাররম ১৪০৩ হিজরি'|
  | Body: ইসলামের পূর্ণাঙ্গ নির্দেশনার আলোকে ছাত্র ও   |   - 'জাতীয় সভাপতি: মোঃ আব্দুল হাফিজ'|
  | যুব সমাজকে গড়ে তোলা এবং চার দশক ধরে সত্য,    | ]                                   |
  | ন্যায় ও ইনসাফভিত্তিক সমাজ বিনির্মাণে নিবেদিত...|                                     |
  +-----------------------------------------------------------------------------------+
  ```
- **Name-Wise Content**:
  - **Section Name (BN)**: সূচনা ও সারসংক্ষেপ
  - **Section Name (EN)**: Hero Overview & Introduction
  - **Section Name (BN)**: সূচনা, ঐতিহ্য ও সেশন পরিচিতি
  - **Section Name (EN)**: Hero Overview, Heritage & Session Stature
  - **Heading 1**: 
    - *Bengali*: `আমাদের সম্পর্কে`
    - *English*: `About Us`
    - *English*: `About SIO West Bengal`
  - **Accent Divider**: `w-14 h-1 bg-[#168BD4] rounded-full`
  - **Session Pill**: `পশ্চিমবঙ্গ জোন • প্রতিষ্ঠিত ১৯৮২ (১লা মুহাররম ১৪০৩ হিজরি) • সেশন ২০২৫–২৬ (২২তম টার্ম)`
  - **Session Moto**: *"Illuminating Society with the Light of Divine Guidance"* (দ্বীনি নির্দেশনার আলোয় সমাজ পুনর্গঠন) — জাতীয় সভাপতি ব্রাদার মোহাম্মদ আব্দুল হাফিজ।
  - **Body Description**: 
    - *Bengali*: `ইসলামের আলোকে ছাত্র ও যুব সমাজকে গড়ে তোলা এবং ব্যক্তি, সমাজ ও জাতির পুনর্গঠনের লক্ষ্য অর্জন করে যাওয়া SIO-র মূল লক্ষ্য। কুরআন-সুন্নাহর নির্দেশনা ও আদর্শকে জীবনের সকল ক্ষেত্রে প্রতিষ্ঠা করতে আমরা প্রতিজ্ঞাবদ্ধ।`
    - *English*: `The core aim of SIO is to nurture students and youth in the light of Divine Guidance, actively participating in the moral and intellectual reconstruction of the individual, society, and the nation.`
  - **Visual Asset**: Architectural geometric arch SVG illustration with `Building2` icon and zonal badge.
    - *Bengali*: `স্টুডেন্টস ইসলামিক অর্গানাইজেশন অব ইন্ডিয়া (SIO) ভারতের ছাত্র ও যুব সমাজের মাঝে নৈতিক চেতনা, চারিত্রিক সততা ও অ্যাকাডেমিক উৎকর্ষ সৃষ্টিতে নিবেদিত এক আদর্শিক ছাত্র আন্দোলন। ১৯৮২ সালের ১৯শে অক্টোবর (১লা মুহাররম ১৪০৩ হিজরি) প্রতিষ্ঠিত হয়ে চার দশকেরও বেশি সময় ধরে সংগঠনটি শিক্ষার্থীদের অধিকার রক্ষা, বৌদ্ধিক বিকাশ এবং শান্তি ও সৌহার্দ্যের সমাজ বিনির্মাণে পথপ্রদর্শকের ভূমিকা পালন করে আসছে।`
    - *English*: `Students Islamic Organisation of India (SIO) is an ideological student movement committed to nurturing moral consciousness, academic brilliance, and societal responsibility. Founded on 19th October 1982 (1st Muharram 1403 A.H.), SIO has stood for over four decades as a vanguard of students' democratic rights, intellectual depth, and ethical social transformation.`
  - **Visual Asset**: Architectural geometric arch SVG illustration with `Building2` icon, official 1982 founding seal, and national/state headquarters attribution.

---

### Section 2: Mission & Objectives (`#mission`)
- **Visual Wireframe**: 2-column card grid on `#F7FAFC` with central action button opening the constitutional modal.
### Section 2: Constitutional Philosophy & Preamble Callout (`#preamble`)
- **Visual Wireframe**: Centered container with left blue border accent (`border-l-4 border-[#168BD4]`), light sky-blue background (`#EAF6FF`), and prominent quote block.
- **Name-Wise Content**:
  - **Section Name (BN)**: আমাদের মিশন ও উদ্দেশ্য
  - **Section Name (EN)**: Our Mission & Objectives
  - **Section Name (BN)**: সংবিধানের ভূমিকা ও মূল দর্শন
  - **Section Name (EN)**: Constitutional Philosophy & Preamble
  - **Preamble Text**:
    - *Divine Sovereignty*: `“আল্লাহ সমগ্র বিশ্বজগতের স্রষ্টা, প্রতিপালক ও একমাত্র শাসক। তিনি প্রকৃতিতে নিজ অমোঘ নিয়ম জারি রেখেছেন। তিনি মানুষকে পৃথিবীতে এক বিশেষ মর্যাদা দান করেছেন—বিবেক, বুদ্ধি, ভালো ও মন্দের পার্থক্য করার স্বাধীনতা দিয়ে তাকে পরীক্ষার মুখে ফেলেছেন। মানুষ যখন অর্পিত স্বাধীনতার সুযোগ নিয়ে আল্লাহর নির্দেশিত সত্য ও ন্যায়ের পথে অবিচল থাকে, তখন সে উভয় জাহানে সাফল্য লাভ করে।”`
    - *Prophetic Universal Mission*: `“মানবজাতির নৈতিক, বৌদ্ধিক, সামাজিক ও অর্থনৈতিক সংকট নিরসনে বিশ্বপ্রতিপালক যুগে যুগে নবী-রাসূলগণের মাধ্যমে সঠিক জীবনবিধান প্রেরণ করেছেন। মহানবী হযরত মুহাম্মদ (সা.)-এর প্রদর্শিত ইসলামের এই সার্বজনীন জীবনব্যবস্থাই পারে বর্ণ, ধর্ম, জাতি ও ভাষার বৈষম্যহীন একটি শান্তিময় ও ইনসাফপূর্ণ বিশ্ব বিনির্মাণ করতে।”`
    - *Sole Motivation*: `“The sole motivating factor in all these efforts should be the pleasure of our Cherisher and His benevolence in the Hereafter.”` (আমাদের সকল চেষ্টার একমাত্র অনুপ্রেরণা মহান প্রতিপালকের সন্তুষ্টি অর্জন ও পরকালীন মুক্তি)।

---

### Section 3: Mission & Six Constitutional Objectives (`#mission`)
- **Visual Wireframe**: 2-column card grid on `#F7FAFC` with central action button opening the constitutional detail modal.
- **Name-Wise Content**:
  - **Section Name (BN)**: আমাদের মিশন ও ৬টি সাংবিধানিক উদ্দেশ্য
  - **Section Name (EN)**: Our Mission & Six Constitutional Objectives
  - **Section Subtitle**: `সংবিধানের ধারা ৪(ক) ও ৪(খ)-এর প্রাতিষ্ঠানিক রূপরেখা`

| # | Card Name (BN / EN) | Icon | Core Content & Constitutional Mandate |
|---|---|---|---|
| **1** | **আমাদের মিশন**<br/>*(Our Mission)* | `Target` | **ধারা ৪(ক)**: ইসলামের পূর্ণাঙ্গ নির্দেশনার আলোকে ছাত্র ও যুব সমাজকে প্রস্তুত করা, যাতে তারা ব্যক্তি, সমাজ এবং জাতির পুনর্গঠনে সক্রিয় ভূমিকা পালন করতে পারে। *(To prepare the students and youth for the reconstruction of the society in the light of Divine Guidance).* |
| **2** | **আমাদের উদ্দেশ্য**<br/>*(Our Objectives)* | `Flag` | **ধারা ৪(খ)**: ছাত্র ও যুবসমাজকে ইসলামের দিকে আহবান জানানো, ইসলামের সঠিক উপলব্ধি গড়ে তোলা, কুরআন-সুন্নাহ অনুযায়ী জীবন গড়ে তোলা, নৈতিক চরিত্র গঠন, সাম্য ও ন্যায়ের পক্ষে কাজ করা এবং সর্বাত্মক বিকাশ সাধন। |
| **1** | **আমাদের মিশন**<br/>*(Our Mission)* | `Target` | **ধারা ৪(ক)**: ছাত্র ও যুব সমাজকে দ্বীনি নির্দেশনার আলোকে সমাজ পুনর্গঠনের জন্য প্রস্তুত করা। *(The mission of the Organisation shall be to prepare the students and youth for the reconstruction of the society in the light of Divine Guidance).* |
| **2** | **৬টি সাংবিধানিক উদ্দেশ্য**<br/>*(Six Core Objectives)* | `Flag` | **ধারা ৪(খ)**:<br/>১. ইসলামের প্রতি আহ্বান জানানো (Calling to Islam)।<br/>২. ইসলামি জ্ঞান ও উপলব্ধি বিস্তার (Cultivating Knowledge)।<br/>৩. কুরআন-সুন্নাহ মোতাবেক চরিত্র গঠন (Character Building)।<br/>৪. মারুফ প্রতিষ্ঠা ও মুনকার প্রতিরোধ (Promoting Virtue & Uprooting Evil)।<br/>৫. শিক্ষাব্যবস্থায় নৈতিক মূল্যবোধ ও সুস্থ পরিবেশ রক্ষা (Educational Reforms)।<br/>৬. সার্বিক মানবসম্পদ ও সুপ্ত মেধা বিকাশ (Holistic Development)। |

- **Modal Trigger Button**: `[বিস্তারিত দেখুন →]` / `[View Full Constitution Details →]`
- **Modal Trigger Button**: `[সংবিধানের বিস্তারিত পাঠ দেখুন →]` / `[View Full Constitutional Text →]`

---

### Section 3: Ideals & Methodology (`#methodology`)
- **Visual Wireframe**: 5-column responsive grid on pure white background featuring circular icon badges and hover accents.
### Section 4: Tri-Modal Constitutional Methodology (`#methodology`)
- **Visual Wireframe**: 3-column responsive grid on pure white background featuring circular icon badges and hover accents.
- **Section Heading**: 
  - *Title*: `আমাদের আদর্শ ও কাজের পদ্ধতি` / `Our Ideals & Methodology`
  - *Divider*: `w-12 h-1 bg-[#168BD4] rounded-full`
  - *Title*: `আমাদের কাজের কর্মপদ্ধতি ও চারিত্রিক মানদণ্ড` / `Our Constitutional Methodology (Article 5)`
  - *Subtitle*: `সংগঠনের যাবতীয় কর্মসূচি বাস্তবায়নে বাধ্যতামূলক ৩টি মূলনীতি।`
- **Name-Wise Methodology Cards**:

| # | Method Pillar (BN / EN) | Icon | Description |
| # | Methodology Pillar (BN / EN) | Article Citation | Description & Practical Application |
|---|---|---|---|
| **1** | **কুরআন ও সুন্নাহ**<br/>*(Qur'an & Sunnah)* | `BookOpen` | আমাদের সকল কার্যক্রমের মূল নির্দেশনা ও ভিত্তি হচ্ছে কুরআন ও সুন্নাহ। |
| **2** | **সৎ, শান্তিপূর্ণ ও গঠনমূলক**<br/>*(Peaceful & Constructive)* | `Handshake` | আমরা শান্তিপূর্ণ, গঠনমূলক ও আইনসম্মত পন্থায় সামাজিক পরিবর্তনে বিশ্বাস করি। |
| **3** | **ছাত্র ও যুব কেন্দ্রিক**<br/>*(Student Centered)* | `Users` | ছাত্র ও যুব সমাজকে নেতৃত্বের জন্য প্রস্তুত করাই আমাদের প্রধান লক্ষ্য। |
| **4** | **চরিত্র গঠন**<br/>*(Character Building)* | `Heart` | ইসলামী চরিত্র, নৈতিকতা ও মূল্যবোধ গঠনে আমরা আপসহীন। |
| **5** | **ব্যক্তি-সমাজ-জাতির উন্নয়ন**<br/>*(Societal Elevation)* | `TrendingUp` | ব্যক্তির উন্নয়নের মাধ্যমে সমাজ ও জাতির সামগ্রিক পুনর্গঠন। |
| **১** | **কুরআন ও সুন্নাহর ভিত্তি**<br/>*(Qur'an & Sunnah)* | **ধারা ৫.১** | সংগঠনের সকল বৌদ্ধিক, নৈতিক ও সাংগঠনিক কার্যক্রমের প্রধান দিকনির্দেশক ও ভিত্তি হবে পবিত্র কুরআন ও সুন্নাহ। |
| **২** | **নৈতিকতার সার্বক্ষণিক অনুশাসন**<br/>*(Strict Moral Bounds)* | **ধারা ৫.২** | সংগঠন সর্বাবস্থায় এবং সকল পদক্ষেপে কঠোরভাবে নৈতিকতার অনুশাসন ও শরিয়াহর সীমা মেনে চলবে। অনৈতিক কৌশল কঠোরভাবে নিষিদ্ধ। |
| **৩** | **শান্তিপূর্ণ ও গঠনমূলক পন্থা**<br/>*(Peaceful & Constructive Means)* | **ধারা ৫.৩** | শিক্ষা, যুক্তি, অনুপ্রেরণা ও সত্য প্রচারের আইনসম্মত মাধ্যমে লক্ষ্য অর্জন করা; এবং মিথ্যা, অসততা, সাম্প্রদায়িক বিদ্বেষ, বিভেদ ও বিশৃঙ্খলা সম্পূর্ণ পরিহার করা। |

---

### Section 4: Our Journey — Aceternity Milestone Timeline (`#history`)
- **Visual Wireframe**: Full-width interactive timeline featuring a dynamic vertical line with an animated glowing blue progress beam (`#168BD4` to `#63BDFF`), sticky milestone nodes, and two-column dummy photo cards.
### Section 5: Our Journey — Aceternity Milestone Timeline (`#history`)
- **Visual Wireframe**: Full-width interactive timeline featuring a dynamic vertical line with an animated glowing blue progress beam (`#168BD4` to `#63BDFF`), sticky milestone nodes, and two-column archival photo cards.
- **Section Heading**:
  - *Pill Badge*: `১৯৮২ — ২০২৬ • চার দশকেরও বেশি ছাত্র নেতৃত্ব` (with pulsing indicator)
  - *Title*: `আমাদের পথচলা` / `Our Journey`
  - *Subtitle*: `১৯৮২ সালের ১৯শে অক্টোবর (১লা মহররম ১৪০৩ হিজরি) প্রতিষ্ঠিত হয়ে আজ চার দশকেরও বেশি সময় ধরে সত্য, শিক্ষা ও সমাজ সংস্কারের অবিচল ছাত্র আন্দোলন।`
  - *Title*: `আমাদের পথচলা` / `Our Four-Decade Journey`
  - *Subtitle*: `১৯৮২ সালের ১৯শে অক্টোবর (১লা মুহাররম ১৪০৩ হিজরি) প্রতিষ্ঠিত হয়ে আজ চার দশকেরও বেশি সময় ধরে সত্য, শিক্ষা ও সমাজ সংস্কারের অবিচল ঐতিহাসিক ছাত্র কাফেলা।`
- **Name-Wise Timeline Milestones**:

#### Milestone 1: ১৯৮২ (1982) — The Genesis & Foundation
- **Title**: `১৯৮২`
- **Subtitle**: `শুরু থেকে • The Genesis`
- **Narrative**: ১৯৮২ সালের ১৯শে অক্টোবর (১লা মহররম ১৪০৩ হিজরি) কয়েকজন দূরদর্শী ছাত্রের হাত ধরে প্রতিষ্ঠিত হয় স্টুডেন্টস ইসলামিক অর্গানাইজেশন অব ইন্ডিয়া (SIO)। জ্ঞান, চরিত্র ও কর্মের সমন্বয়ে একটি ন্যায়ভিত্তিক সমাজ বিনির্মাণের প্রত্যয়ে শুরু হয় এই ঐতিহাসিক অভিযাত্রা।
- **Badges**:
  - `১৯ অক্টোবর ১৯৮২ প্রতিষ্ঠা`
  - `১লা মহররম ১৪০৩ হিজরি`
  - `সত্য ও ন্যায়ের আদর্শ`
- **Subtitle**: `শুরু থেকে • The Genesis & Foundation`
- **Narrative**: ১৯৮২ সালের ১৯শে অক্টোবর (১লা মুহাররম ১৪০৩ হিজরি) কয়েকজন দূরদর্শী ছাত্রের হাত ধরে প্রতিষ্ঠিত হয় স্টুডেন্টস ইসলামিক অর্গানাইজেশন অব ইন্ডিয়া (SIO)। জ্ঞান, চরিত্র ও কর্মের সমন্বয়ে একটি ন্যায়ভিত্তিক সমাজ বিনির্মাণের প্রত্যয়ে শুরু হয় এই ঐতিহাসিক অভিযাত্রা।
- **Badges**: `১৯ অক্টোবর ১৯৮২ প্রতিষ্ঠা` • `১লা মুহাররম ১৪০৩ হিজরি` • `সংবিধান কার্যকর (ধারা ৩)`
- **Dummy Images Grid (2 Columns)**:
  1. `https://images.unsplash.com/photo-1523240795612-9a054b0db644?q=80&w=800&auto=format&fit=crop`
     - *Caption*: প্রতিষ্ঠাতা ছাত্র প্রতিনিধিদের প্রাথমিক সমাবেশ (১৯৮২)
     - *Sub-caption*: পশ্চিমবঙ্গে ছাত্র আন্দোলনের সূত্রপাত
  2. `https://images.unsplash.com/photo-1517486808906-6ca8b3f04846?q=80&w=800&auto=format&fit=crop`
     - *Caption*: নৈতিক পাঠচক্র ও ছাত্র কল্যাণ কর্মসূচি
     - *Sub-caption*: ক্যাম্পাসভিত্তিক প্রাথমিক ইউনিট গঠন
  1. Founder Student Representatives Assembly (1982)
  2. Moral Study Circles & First Campus Units in Bengal.

#### Milestone 2: ১৯৯০ — ২০০০ (1990s — 2000s) — Organic Growth & Campus Outreach
#### Milestone 2: ১৯৯০ — ২০০০ (1990s — 2000s) — Organic Growth & Campus Rights
- **Title**: `১৯৯০ — ২০০০`
- **Subtitle**: `ক্রমবিকাশ • Campus Expansion`
- **Narrative**: সময়ের সাথে সাথে স্কুল, মাদ্রাসা এবং বিশ্ববিদ্যালয় ক্যাম্পাসে সংগঠনের বিকাশ ঘটে। কলকাতা বিশ্ববিদ্যালয়, যাদবপুর, আলিয়া, উত্তরবঙ্গ এবং বর্ধমান বিশ্ববিদ্যালয়ে ছাত্র অধিকার রক্ষা, ক্যারিয়ার গাইডেন্স এবং রক্তদান কর্মসূচির মতো মানবিক সেবার সূচনা।
- **Badges**:
  - `ক্যাম্পাস অধিকার আন্দোলন`
  - `ক্যারিয়ার ও স্কলারশিপ গাইডেন্স`
  - `জরুরি মানবসেবা ও রক্তদান`
- **Dummy Images Grid (2 Columns)**:
  1. `https://images.unsplash.com/photo-1524178232363-1fb2b075b655?q=80&w=800&auto=format&fit=crop`
     - *Caption*: বিশ্ববিদ্যালয় ক্যাম্পাসে শিক্ষা অধিকার সেমিনার
     - *Sub-caption*: গণতান্ত্রিক ছাত্র সংসদ ও ক্যাম্পাস রাজনীতি সংস্কার
  2. `https://images.unsplash.com/photo-1427504494785-3a9ca7044f45?q=80&w=800&auto=format&fit=crop`
     - *Caption*: মেধাবী শিক্ষার্থীদের জন্য স্টাডি সার্কেল ও লাইব্রেরি
     - *Sub-caption*: উচ্চশিক্ষায় অনগ্রসরদের সহযোগিতা
- **Subtitle**: `ক্যাম্পাস বিকাশ • Campus Expansion & Movement`
- **Narrative**: কলকাতা বিশ্ববিদ্যালয়, যাদবপুর, আলিয়া, উত্তরবঙ্গ এবং বর্ধমান বিশ্ববিদ্যালয়ে ছাত্র অধিকার রক্ষা, গণতান্ত্রিক ছাত্র সংসদ নির্বাচন, ক্যারিয়ার গাইডেন্স এবং রক্তদান কর্মসূচির মতো মানবিক সেবার প্রাতিষ্ঠানিক বিস্তার।
- **Badges**: `ক্যাম্পাস অধিকার আন্দোলন` • `ক্যারিয়ার ও স্কলারশিপ ডেস্ক` • `জরুরি মানবসেবা নেটওয়ার্ক`.

#### Milestone 3: ২০১০ — ২০২০ (2010s — 2020s) — Research, Academic Forums & Mega Conferences
- **Title**: `২০১০ — ২০২০`
- **Subtitle**: `মেধা বিকাশ ও সম্মেলন • Research & Mega Conferences`
- **Narrative**: শিক্ষা সংস্কার ও বুদ্ধিবৃত্তিক গবেষণায় সূচনা হয় CERT (Centre for Educational Research & Training) এবং সাংস্কৃতিক জাগরণে BTF (বঙ্গীয় প্রতিভা ফোরাম)। রাজ্যজুড়ে ঐতিহাসিক ছাত্র সমাবেশ, শিক্ষানীতি সমীক্ষা ও গ্রন্থ প্রকাশনার নতুন দিগন্ত উন্মোচিত হয়।
- **Badges**:
  - `CERT শিক্ষা গবেষণা শাখা`
  - `BTF সাহিত্য ও প্রতিভা বিকাশ`
  - `ঐতিহাসিক রাজ্য ছাত্র সমাবেশ`
- **Dummy Images Grid (2 Columns)**:
  1. `https://images.unsplash.com/photo-1577495508048-b635879837f1?q=80&w=800&auto=format&fit=crop`
     - *Caption*: কলকাতা নজরুল মঞ্চে রাজ্য ছাত্র সম্মেলন
     - *Sub-caption*: হাজার হাজার প্রতিনিধির ঐতিহাসিক সমাগম
  2. `https://images.unsplash.com/photo-1541339907198-e08756dedf3f?q=80&w=800&auto=format&fit=crop`
     - *Caption*: শিক্ষা সমীক্ষা ও গবেষণা প্রকাশনা উদ্বোধন
     - *Sub-caption*: পশ্চিমবঙ্গের শিক্ষা সংকট নিয়ে বিশ্লেষণ
- **Narrative**: শিক্ষা সংস্কার ও গবেষণায় CERT (Centre for Educational Research & Training) এবং সাংস্কৃতিক জাগরণে BTF (বঙ্গীয় প্রতিভা ফোরাম)-এর প্রতিষ্ঠা। কলকাতা নজরুল মঞ্চে ঐতিহাসিক ছাত্র সমাবেশ এবং শিক্ষানীতি সমীক্ষা প্রকাশ।
- **Badges**: `CERT শিক্ষা গবেষণা কেন্দ্র` • `BTF সাহিত্য ও মেধা বিকাশ` • `ঐতিহাসিক রাজ্য ছাত্র সমাবেশ`.

#### Milestone 4: ২০২৬ ও আগামী দিন (2026 & Beyond) — Transforming Bengal's Future
- **Title**: `২০২৬ ও আগামী দিন`
- **Subtitle**: `আজ ও আগামী দিন • Present & Future Horizon`
- **Narrative**: বর্তমানে পশ্চিমবঙ্গের ২৩টি জেলা এবং শত শত প্রতিষ্ঠানে সক্রিয় SIO। শিক্ষার্থীদের ডিজিটাল সহায়তা, লিগ্যাল এইড সেল, স্কলারশিপ ডেস্ক এবং নেতৃত্ব বিকাশ শিবিরের মাধ্যমে এক মানবিক, বৈষম্যহীন ও সমৃদ্ধ বাংলা গঠনে আমরা অঙ্গীকারবদ্ধ।
- **Badges**:
  - `২৩টি জেলায় তৃণমূল নেটওয়ার্ক`
  - `ডিজিটাল লার্নিং ও লিগ্যাল এইড`
  - `নৈতিক সমাজ ও আগামীর নেতৃত্ব`
- **Dummy Images Grid (2 Columns)**:
  1. `https://images.unsplash.com/photo-1531482615713-2afd69097998?q=80&w=800&auto=format&fit=crop`
     - *Caption*: রাজ্য যুব নেতৃত্ব ও স্কিল ডেভেলপমেন্ট সামিট
     - *Sub-caption*: একবিংশ শতাব্দীর চ্যালেঞ্জ মোকাবেলায় তরুণরা
  2. `https://images.unsplash.com/photo-1522202176988-66273c2fd55f?q=80&w=800&auto=format&fit=crop`
     - *Caption*: ক্যাম্পাস অধিকার ও সার্বজনীন ছাত্র সহায়তা নেটওয়ার্ক
     - *Sub-caption*: ২৪/৭ শিক্ষার্থী সহায়তায় নিবেদিত
#### Milestone 4: ২০২৫ — ২০২৬ ও আগামী দিন (2025–2026 / 22nd Term & Beyond)
- **Title**: `২০২৫ — ২০২৬ ও আগামী দিন`
- **Subtitle**: `সেশন ২০২৫–২৬ • 22nd Term & Future Horizon`
- **Narrative**: জাতীয় সভাপতি ব্রাদার মোহাম্মদ আব্দুল হাফিজের নেতৃত্বে বর্তমান ২২তম টার্মে গৃহীত হয়েছে ১২ দফা 'পলিসি অ্যান্ড প্রোগ্রাম ২০২৫–২৬'। আত্মশুদ্ধি (তাজকিয়া), ডিজিটাল নীতিশাস্ত্র, প্রজেক্ট ইনকাব (InQhab), ফ্রেমিং অ্যাকাডেমিয়া, প্যারিসার সংবাদ (পরিবেশ ফোরাম) এবং ওয়াকফ ও মানবাধিকার সুরক্ষায় পশ্চিমবঙ্গজুড়ে নতুন অগ্রযাত্রা।
- **Badges**: `২২তম টার্ম (সেশন ২০২৫-২৬)` • `১২ কৌশলগত পলিসি প্লাংক` • `প্রজেক্ট ইনকাব ও ফ্রেমিং অ্যাকাডেমিয়া` • `ডিজিটাল নীতিশাস্ত্র ও পরিবেশ`.

---

### Section 5: Organizational Structure & Leadership Gateway (`#structure`)
### Section 6: Four-Tier Democratic Governance & Institutional Hierarchy (`#structure`)
- **Visual Wireframe**: 4-Tier horizontal structure cards followed by a high-impact horizontal banner directing users to the Leadership Directory (`/about/leadership`).
- **Section Heading**: 
  - *Title*: `আমাদের সাংগঠনিক কাঠামো` / `Our Organizational Structure`
  - *Title*: `আমাদের সাংগঠনিক শাসনতন্ত্র ও স্তরবিন্যাস` / `Four-Tier Democratic Governance`
  - *Subtitle*: `কেন্দ্রীয় মজলিসে শুরা (CAC) থেকে স্থানীয় ক্যাম্পাস ইউনিট পর্যন্ত শুরাভিত্তিক পরামর্শমূলক কাঠামো।`
- **Name-Wise Structural Tiers**:

| Tier # | Tier Name (BN / EN) | Icon | Scope & Responsibilities |
| Tier # | Tier Name (BN / EN) | Constitutional Basis | Scope & Responsibilities |
|---|---|---|---|
| **Tier 1** | **কেন্দ্রীয় কাঠামো**<br/>*(Central Structure)* | `Building2` | সারাদেশের জন্য দিকনির্দেশনা ও নীতি নির্ধারণ (National CAC & HQ)। |
| **Tier 2** | **জোনাল কাঠামো**<br/>*(Zonal Structure)* | `MapPin` | রাজ্য/অঞ্চল ভিত্তিক সংগঠন ও কার্যক্রম পরিচালনা (West Bengal ZAC & Secretariat)। |
| **Tier 3** | **স্থানীয় ইউনিট**<br/>*(Local Units)* | `Users2` | জেলা ও উপজেলা পর্যায়ে বাস্তব কার্যক্রম বাস্তবায়ন (23 Districts)। |
| **Tier 4** | **শাখা/প্রকল্প**<br/>*(Branches & Projects)* | `GitFork` | কলেজ, বিশ্ববিদ্যালয়, মাদ্রাসা ও পাড়া-মহল্লা পর্যায়ে শিক্ষার্থীদের সংগঠিত করা। |
| **Tier 1** | **কেন্দ্রীয় স্তর (Markaz)** | **ধারা ৯–২৪** | প্রধান অভিভাবক (Chief Patron - আমিরে জামায়াত), কেন্দ্রীয় সভাপতি (National President) এবং ১৫ সদস্যের নির্বাচিত মজলিসে শুরা (CAC)। |
| **Tier 2** | **জোনাল স্তর (State Zone)** | **ধারা ২৫–৩৭** | জোনাল প্যাট্রন (Ameer-e-Halqa), নির্বাচিত জোন সভাপতি (Zonal President), জোনাল শুরা (ZAC) ও প্রশাসনিক সচিবালয়। |
| **Tier 3** | **জেলা ও বিভাগীয় স্তর** | **সাংগঠনিক জেলা** | পশ্চিমবঙ্গের ২৩টি প্রশাসনিক জেলায় জেলা সভাপতি ও কার্যকরী সমন্বয়কদের আঞ্চলিক মনিটরিং নেটওয়ার্ক। |
| **Tier 4** | **স্থানীয় ও ক্যাম্পাস ইউনিট** | **ধারা ৩৮–৪১** | যেখানে ২ বা ততোধিক সদস্য সক্রিয়, সেখানেই প্রাতিষ্ঠানিক ইউনিট গঠিত। স্থানীয় সভাপতি ও লোকাল শুরা (LAC) দ্বারা ক্যাম্পাস সেল পরিচালিত। |

- **Constitutional Hallmarks Bar**:
  - **দ্বিবার্ষিক সেশন (Biennial Term — ধারা ৮)**: কেন্দ্র ও জোন পর্যায়ে দুই বছর মেয়াদি গণতান্ত্রিক কার্যকাল।
  - **পদলিপ্সাহীন আত্মনিবেদিত নেতৃত্ব (Non-Aspiring Leadership — ধারা ৭)**: কোনো পদের জন্য নিজে আকাঙ্ক্ষা প্রকাশ বা লবিং করা সম্পূর্ণ নিষিদ্ধ। তাকওয়া, জ্ঞান ও আমানতদারিতাই দায়িত্ব অর্পণের মানদণ্ড।
  - **কঠোর আর্থিক স্বচ্ছতা ও অডিটকৃত বায়তুলমাল (Audited Baitulmal — ধারা ৪২–৪৭)**: তহবিল কেবল ধারা ৪-এর উদ্দেশ্যেই ব্যয় হতে পারে (ধারা ৪৩), নিজস্ব সদস্য চাঁদা ও অনুদানে পরিচালিত, প্রতি বছর বাধ্যতামূলক সরকারি অডিট।
- **Leadership Gateway Banner**:
  - *Headline*: `রাজ্য সভাপতি, সম্পাদকমণ্ডলী ও জেলা নেতৃত্ব দেখুন`
  - *Subtext*: `২০২৫–২৬ সেশনের নির্বাচিত রাজ্য পরামর্শদাতা পরিষদ এবং ঐতিহাসিক নেতৃত্ব আর্কাইভ।`
  - *Subtext*: `২০২৫–২৬ সেশনের নির্বাচিত রাজ্য পরামর্শদাতা পরিষদ (ZAC) এবং ঐতিহাসিক নেতৃত্ব আর্কাইভ।`
  - *CTA Button*: `[নেতৃত্ব পৃষ্ঠা দেখুন →]` (Linked to `/about/leadership`)

---

### Section 6: Join Movement Call to Action (`#join`)
- **Visual Wireframe**: Full-width light blue container (`#EAF6FF`) with subtle student silhouette graphic and prominent centered CTA.
### Section 7: Constitutional Membership Criteria & Youth CTA (`#join`)
- **Visual Wireframe**: Full-width light blue container (`#EAF6FF`) highlighting the 4 eligibility conditions from Article 6 and enrollment gateway.
- **Name-Wise Content**:
  - **Heading**: `আপনিও যুক্ত হন` / `Join the Movement`
  - **Description**: `আদর্শ সমাজ গঠনের এই মহান কাজে আপনিও অংশ নিন। আসুন, একসাথে গড়ে তুলি আলোকিত আগামী।`
  - **Action Button**: `[যোগ দিন এখনই →]` (Linked to `/contact`)
  - **Badge**: `সাংবিধানিক সদস্যপদ মানদণ্ড • ধারা ৬` / `Membership Standards • Article 6`
  - **Heading**: `সত্য, চরিত্র ও সমাজ বিনির্মাণের এই কাফেলায় আপনিও অংশ নিন` / `Join the Movement for Societal Reconstruction`
  - **Description**: `ভারতের যেকোনো শিক্ষার্থী বা যুবক (সর্বোচ্চ ৩০ বছর বয়স পর্যন্ত) যিনি নৈতিক সততা বজায় রেখে দ্বীনি নির্দেশনার আলোকে সমাজ বিনির্মাণে বিশ্বাসী—তিনি SIO-তে যুক্ত হতে পারেন।`
  - **4 Pillars of Eligibility**:
    1. **নাগরিকত্ব ও বয়স (Article 6.3, 6.4)**: ভারতীয় নাগরিক, ছাত্র বা যুবক, সর্বোচ্চ ৩০ বছর বয়স।
    2. **সংবিধানের শপথ (Article 6.1)**: সংগঠনের সংবিধান বোঝা এবং তার শৃঙ্খলা ও আনুগত্যের অঙ্গীকার করা।
    3. **ফরজ বিধান পালন (Article 6.2)**: সালাত, সাওমসহ সমস্ত ধর্মীয় ফরজ নিয়মিত একনিষ্ঠভাবে পালন করা।
    4. **কবিরা গুনাহ বর্জন (Article 6.2)**: সমস্ত বড় পাপ থেকে নিজেকে পবিত্র রাখা ও চারিত্রিক সততা বজায় রাখা।
  - **Action Button**: `[সদস্যপদ আবেদন করুন এখনই →]` (Linked to `/contact`)

---

### Section 7: Newsletter Subscription Strip
### Section 8: Newsletter Subscription Strip
- **Visual Wireframe**: Full-width `#0F4C81` Navy strip with Mail icon, description, input field, and black submit button.
- **Name-Wise Content**:
  - **Heading**: `আমাদের সাথে থাকুন` / `Stay Connected with Us`
  - **Description**: `নতুন খবর, অনুষ্ঠান ও প্রকাশনার আপডেট পেতে আমাদের নিউজলেটারে সাবস্ক্রাইব করুন।`
  - **Input**: `আপনার ইমেইল দিন`
  - **Submit Button**: `সাবস্ক্রাইব করুন` / `Subscribed!`

---

### Interactive Component: Constitutional Detail Modal (Article 4)
- **Modal Header**: SIO সংবিধান — ধারা ৪ (উদ্দেশ্য ও লক্ষ্য) / SIO Constitution — Article 4
### Interactive Component: Full Constitutional Detail Modal (Articles 4, 5 & 6)
- **Modal Header**: SIO সংবিধান — ধারা ৪, ৫ ও ৬ (লক্ষ্য, কর্মপদ্ধতি ও সদস্যপদ)
- **Mission Box [Article 4(A)]**:
  `“The mission of the Organisation shall be to prepare the students and youth for the reconstruction of the society in the light of Divine Guidance.”`
- **Six Constitutional Objectives [Article 4(B)]**:
  1. ছাত্র ও যুব সমাজকে ইসলামের দিকে আহ্বান জানানো (To call students and youth towards Islam)।
  2. ছাত্র ও যুব সমাজের মধ্যে ইসলামের সঠিক জ্ঞান ও উপলব্ধি বিস্তার করা (To promote and cultivate the knowledge and understanding of Islam)।
  3. কুরআন ও সুন্নাহ অনুযায়ী ব্যক্তিগত ও সামগ্রিক জীবন গঠনের জন্য ছাত্রদের প্রস্তুত করা (To prepare students to shape their lives in accordance with the Qur’an and the Sunnah)।
  4. সৎকাজের প্রতিষ্ঠা (মারুফ) এবং অন্যায়ের প্রতিরোধে (মুনকার) সক্রিয় হওয়া (To uphold Virtue and prevent Evil)।
  5. শিক্ষাব্যবস্থায় নৈতিক মূল্যবোধের প্রতিষ্ঠা ও শিক্ষাঙ্গনে শান্তিপূর্ণ শিক্ষার পরিবেশ নিশ্চিত করা (To promote moral values in education and foster better academic atmosphere)।
  6. সংগঠনের সাথে যুক্ত ব্যক্তিবর্গের সামগ্রিক বিকাশ ও তাদের প্রতিভার সদ্ব্যবহার করা (To facilitate holistic development of individuals and nourish their talents)।
- **Citation**: *Students Islamic Organisation of India Constitution, Amended Dec 2022, Pages 10–11*.
- **Methodology [Article 5]**: কুরআন-সুন্নাহর ভিত্তি, কঠোর নৈতিকতা ও শান্তিপূর্ণ-গঠনমূলক পন্থা।
- **Membership [Article 6]**: ভারতীয় নাগরিক, অনূর্ধ্ব ৩০ বছর, সালাত-সাওম পালন ও কবিরা গুনাহ বর্জন।
- **Citation**: *Students Islamic Organisation of India Constitution, Amended Dec 2022, Pages 10–12*.
- **Footer**: `[বন্ধ করুন / Close]`
