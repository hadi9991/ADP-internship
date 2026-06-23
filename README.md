# Internship Plan — 4 Weeks

**Schedule:** 5 days/week · 0.5–1 hour/day

---

## Week 1: Contact Center Foundations

### Day 1 — Introduction to Contact Centers
- [ ] Watch / go through [Introduction to Contact Center](./Slides/Introduction%20to%20Contact%20Center.pptx) presentation
- [ ] Discuss: what is an IVR? what is a chatbot? how do they differ?

### Day 2 — Experiencing Real IVRs
- [ ] Call We IVR `19777` — listen and note the structure (menus, prompts, routing)
- [ ] Call CIB Bank IVR `19666` — compare with We IVR

### Day 3 — Experiencing Real Chatbots
- [ ] Try [We Chat Bot](https://te.eg/wps/portal/te/Personal) — note the conversation flow
- [ ] Try [Elm WhatsApp Bot](https://wa.me/966920000356) — compare tone and capabilities
- [ ] Write down: 3 observations from real IVRs vs. 3 from chatbots

### Day 4 — Environment Setup
- [ ] Install [JDK 8](https://download.oracle.com/otn/java/jdk/8u461-b11/68ce765258164726922591683c51982c/jdk-8u461-windows-x64.exe?AuthParam=1754890059_d6d68a80f8210251e18a15f9ec3211bd)
- [ ] Install [Call Studio](https://istnetworkscom-my.sharepoint.com/:u:/g/personal/mgheta_istnetworks_com/ESvt5z_2JV1InI4WM5NgcjAB8VTBY8ikGSf3ry-RMortPg)
- [ ] Open Call Studio and explore the workspace

### Day 5 — Call Studio Core Elements
- [ ] Call We IVR `19777` again — this time map each step to a Call Studio element
- [ ] Learn the 4 basic elements: `Prompt`, `Menu`, `Decision`, `Input`
- [ ] Build a minimal "Hello World" flow in Call Studio

---

## Week 2: Building IVRs

### Day 6 — Pizza Shop IVR (Part 1)
- [ ] Read the [Pizza Shop IVR](./Projects/Project%200%20-%20Pizza%20Shop%20IVR.md) project spec
- [ ] Design the call flow on paper before touching Call Studio
- [ ] Start building the main menu

### Day 7 — Pizza Shop IVR (Part 2)
- [ ] Complete the Pizza Shop IVR flow
- [ ] Test all menu paths and fix any issues
- [ ] Review: what worked, what was confusing?

### Day 8 — Telecom IVR (Part 1)
- [ ] Read the [Telecom IVR](./Projects/Project%201%20-%20Telecom%20IVR.md) project spec
- [ ] Design the call flow — compare complexity with Pizza Shop IVR
- [ ] Start building the Telecom IVR main structure

### Day 9 — Telecom IVR (Part 2)
- [ ] Complete the Telecom IVR flow
- [ ] Test all branches end-to-end
- [ ] :memo: Submit completed Telecom IVR

### Day 10 — IVR Review & Consolidation
- [ ] Side-by-side comparison of Pizza Shop IVR vs. Telecom IVR
- [ ] Identify reusable patterns (common menus, error handling)
- [ ] Q&A and open discussion on IVR design best practices

---

## Week 3: REST APIs

### Day 11 — REST API Concepts
- [ ] Install [VSCode](https://code.visualstudio.com/download) or [IntelliJ IDEA](https://www.jetbrains.com/idea/download)
- [ ] Learn: `Endpoints`, `HTTP Methods` (GET, POST, PUT, DELETE), `Status Codes`, `Request Params`, `Response Body`
- [ ] Explore a public API (e.g., [JSONPlaceholder](https://jsonplaceholder.typicode.com)) using a browser or Postman

### Day 12 — Products API (Part 1)
- [ ] Read the [Products API](./Projects/Products%20API/README.md) spec
- [ ] Set up the Java project structure
- [ ] Implement GET `/products` and GET `/products/{id}`

### Day 13 — Products API (Part 2)
- [ ] Implement POST `/products`, PUT `/products/{id}`, DELETE `/products/{id}`
- [ ] Test all endpoints manually
- [ ] :memo: Submit completed Products API

### Day 14 — Pizza Shop API
- [ ] Read the [Pizza Shop API](./Projects/Pizza%20Shop%20API/README.md) spec
- [ ] Build and test all endpoints
- [ ] :memo: Submit completed Pizza Shop API

### Day 15 — API Review & Consolidation
- [ ] Compare Products API vs. Pizza Shop API designs
- [ ] Discuss REST best practices: naming conventions, status codes, error responses
- [ ] Q&A and open discussion

---

## Week 4: Integration, Tools & Database

### Day 16 — IVR ↔ API Integration Concepts
- [ ] Learn the `RestClient` element in Call Studio
- [ ] Understand how IVRs call APIs: request format, parsing responses
- [ ] Integrate [Pizza Shop IVR](./Projects/Pizza%20Shop%20IVR/README.md) with [Pizza Shop API](./Projects/Pizza%20Shop%20API/README.md)

### Day 17 — Telecom Full Integration
- [ ] Build the [Telecom API](./Projects/Telecom%20API/README.md)
- [ ] Integrate [Telecom IVR](./Projects/Telecom%20IVR/README.md) with Telecom API
- [ ] :memo: Submit integrated Telecom project

### Day 18 — IVR Audio Tools
- [ ] Use [PromptMatrixGenerator](https://github.com/moazmohamed20-ist/PromptMatrixGenerator) to generate `.wav` files from an Excel prompt matrix
- [ ] Use [GoldWave](https://goldwave.com/download.php?file=gw) to convert `.wav` files to **u-law 8000 Hz**
- [ ] Load generated prompts into a Call Studio project

### Day 19 — Dynamic Prompts & Database
- [ ] Explore IST SayItSmart plugins: `DigitByDigit`, `Number`, `Currency`
- [ ] Add SQLite persistence to [Products API](./Projects/Products%20API/README.md)
- [ ] Install [DB Browser for SQLite](https://github.com/sqlitebrowser/sqlitebrowser/releases/download/v3.13.1/DB.Browser.for.SQLite-v3.13.1-win64.zip) and inspect the database

### Day 20 — Swagger UI & Final Wrap-up
- [ ] Add Swagger UI to [Products API](./Projects/Products%20API/README.md)
- [ ] Full end-to-end demo: IVR call → API → database → response
- [ ] Retrospective: what did you learn? what would you explore next?
