# Internship Plan — 16 Days

**Schedule:** 5 days/week · 0.5–1 hour/day

---

## Week 1: Contact Center Foundations & Call Studio Basics

### Day 1 — Introduction to Contact Center
- [ ] Watch / go through [Introduction to Contact Center](./Slides/Introduction%20to%20Contact%20Center.pptx) presentation
- [ ] Discuss: what is an IVR? what is a chatbot? how do they differ?

### Day 2 — Real IVRs
- [ ] Call We IVR `19777` — listen and note the structure (menus, prompts, routing)
- [ ] Call CIB Bank IVR `19666` — compare with We IVR
- [ ] Write down observations: menu depth, prompt style, error handling, routing logic

### Day 3 — Real Chatbots & Environment Setup
- [ ] Try [We Chat Bot](https://te.eg/wps/portal/te/Personal) — note the conversation flow
- [ ] Try [Elm WhatsApp Bot](https://wa.me/966920000356) — compare tone and capabilities
- [ ] Write down: 3 observations from real IVRs vs. 3 from chatbots
- [ ] Install [JDK 8](https://download.oracle.com/otn/java/jdk/8u461-b11/68ce765258164726922591683c51982c/jdk-8u461-windows-x64.exe?AuthParam=1754890059_d6d68a80f8210251e18a15f9ec3211bd)
- [ ] Install [Call Studio](https://istnetworkscom-my.sharepoint.com/:u:/g/personal/mgheta_istnetworks_com/ESvt5z_2JV1InI4WM5NgcjAB8VTBY8ikGSf3ry-RMortPg)
- [ ] Open Call Studio and explore the workspace

### Day 4 — Call Studio: `Prompt` & `Menu`
- [ ] Call We IVR `19777` again — map each step to a Call Studio element
- [ ] Learn the `Prompt` element — play a greeting, static message
- [ ] Learn the `Menu` element — build a simple 2-option menu

### Day 5 — Call Studio: `Decision` & `Input`
- [ ] Learn the `Decision` element — conditional branching based on variables
- [ ] Learn the `Input` element — collect DTMF or speech input from the caller
- [ ] Build a minimal "Hello World" flow that uses all four elements

---

## Week 2: Building IVRs & REST API Concepts

### Day 6 — Pizza Shop IVR
- [ ] 📝 Create [Pizza Shop IVR](./Projects/Project%200%20-%20Pizza%20Shop%20IVR.md)

### Day 7 — Telecom IVR
- [ ] 📝 Create [Telecom IVR](./Projects/Project%201%20-%20Telecom%20IVR.md)

### Day 8 — IVR Review & Consolidation
- [ ] Side-by-side comparison: Pizza Shop IVR vs. Telecom IVR
- [ ] Identify reusable patterns (common menus, error handling, re-prompt logic)
- [ ] Q&A on IVR design best practices

### Day 9 — REST API Concepts
- [ ] Install [VSCode](https://code.visualstudio.com/download) or [IntelliJ IDEA](https://www.jetbrains.com/idea/download)
- [ ] Learn: `Endpoints`, `HTTP Methods` (GET, POST, PUT, DELETE), `Status Codes`, `Request Params`, `Response Body`
- [ ] Explore a public API (e.g., [JSONPlaceholder](https://jsonplaceholder.typicode.com)) using a browser or Postman

### Day 10 — Products API (Part 1)
- [ ] Set up the Java project structure
- [ ] Implement GET `/products` and GET `/products/{id}`
- [ ] Test both endpoints manually

---

## Week 3: REST APIs & IVR ↔ API Integration

### Day 11 — Products API (Part 2) & Pizza Shop API
- [ ] Implement POST `/products`, PUT `/products/{id}`, DELETE `/products/{id}`
- [ ] Test all endpoints manually
- [ ] 📝 Submit completed [Products API](./Projects/Products%20API/README.md)
- [ ] 📝 Create [Pizza Shop API](./Projects/Pizza%20Shop%20API/README.md)

### Day 12 — API Review & Consolidation
- [ ] Compare Products API vs. Pizza Shop API designs
- [ ] Discuss REST best practices: naming conventions, status codes, error responses
- [ ] Q&A

### Day 13 — IVR ↔ API Integration: Pizza Shop
- [ ] Learn the `RestClient` element in Call Studio
- [ ] Understand how IVRs call APIs: request format, parsing responses
- [ ] Integrate [Pizza Shop IVR](./Projects/Pizza%20Shop%20IVR/README.md) with [Pizza Shop API](./Projects/Pizza%20Shop%20API/README.md)

### Day 14 — Telecom Full Integration
- [ ] 📝 Create [Telecom API](./Projects/Telecom%20API/README.md)
- [ ] 📝 Integrate [Telecom IVR](./Projects/Telecom%20IVR/README.md) with Telecom API

---

## Week 4: Tools, Database & Wrap-up

### Day 15 — IVR Audio Tools & Dynamic Prompts
- [ ] Use [PromptMatrixGenerator](https://github.com/moazmohamed20-ist/PromptMatrixGenerator) to generate `.wav` files from an Excel prompt matrix
- [ ] Use [GoldWave](https://goldwave.com/download.php?file=gw) to convert `.wav` files to **u-law 8000 Hz**
- [ ] Load generated prompts into a Call Studio project
- [ ] Explore IST SayItSmart plugins: `DigitByDigit`, `Number`, `Currency`

### Day 16 — Database Persistence, Swagger UI & Final Demo
- [ ] Integrate [Products API](./Projects/Products%20API/README.md) with SQLite
- [ ] Install [DB Browser for SQLite](https://github.com/sqlitebrowser/sqlitebrowser/releases/download/v3.13.1/DB.Browser.for.SQLite-v3.13.1-win64.zip) and inspect the database
- [ ] Add Swagger UI to [Products API](./Projects/Products%20API/README.md)
- [ ] Full end-to-end demo: IVR call → API → database → response
- [ ] Final retrospective: what did you learn? what would you explore next?
