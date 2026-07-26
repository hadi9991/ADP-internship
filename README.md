# Internship Plan — 4 Weeks

**Schedule:** 5 days/week · 0.5–1 hour/day · 16 working days

| Week | Focus | Days |
| :--- | :--- | :--- |
| **1** | Contact Center foundations & Call Studio basics | 1 – 5 |
| **2** | IVRs, REST concepts, audio tools & data | 6 – 10 |
| **3** | Review & building REST APIs | 11 – 14 |
| **4** | IVR ↔ API integration | 15 – 16 |

> 📝 marks a **deliverable** — something you submit at the end of the day.

---

## Week 1 — Contact Center Foundations & Call Studio Basics

### Day 1 — Introduction to Contact Center

- [ ] Watch / go through the [Introduction to Contact Center](./PPT/Introduction%20to%20Contact%20Center%20-%20IST.pptx) presentation
- [ ] Discuss: what is an IVR? what is a chatbot? how do they differ?

### Day 2 — Real IVRs & Environment Setup

- [ ] Call **We IVR** `19777` — listen and note the structure (menus, prompts, routing)
- [ ] Call **CIB Bank IVR** `19666` — compare with the We IVR
- [ ] Write down observations: menu depth, prompt style, error handling, routing logic
- [ ] Install [JDK 8](https://download.oracle.com/otn/java/jdk/8u461-b11/68ce765258164726922591683c51982c/jdk-8u461-windows-x64.exe?AuthParam=1754890059_d6d68a80f8210251e18a15f9ec3211bd)
- [ ] Install [Call Studio](https://istnetworkscom-my.sharepoint.com/:u:/g/personal/mgheta_istnetworks_com/ESvt5z_2JV1InI4WM5NgcjAB8VTBY8ikGSf3ry-RMortPg)

### Day 3 — First Look at Call Studio

- [ ] Verify the setup: JDK 8 installed and on the `PATH`, Call Studio launches cleanly
- [ ] Open Call Studio and explore the workspace — palette, canvas, properties, project tree
- [ ] Create an empty project and get familiar with where everything lives

### Day 4 — Call Studio: `Prompt` & `Menu`

- [ ] Learn the `Prompt` element — play a greeting, static message
- [ ] Learn the `Menu` element — build a simple 2-option menu

### Day 5 — Call Studio: `Decision` & `Input`

- [ ] Learn the `Decision` element — conditional branching based on variables
- [ ] Learn the `Input` element — collect DTMF or speech input from the caller
- [ ] Build a minimal "Hello World" flow that uses all four elements

---

## Week 2 — IVRs, REST Concepts, Audio & Data

### Day 6 — REST API Concepts

- [ ] Install [VSCode](https://code.visualstudio.com/download) or [IntelliJ IDEA](https://www.jetbrains.com/idea/download)
- [ ] Learn: `Endpoints`, `HTTP Methods` (GET, POST, PUT, DELETE), `Status Codes`, `Request Params`, `Response Body`
- [ ] Explore a public API (e.g. [JSONPlaceholder](https://jsonplaceholder.typicode.com)) using a browser or Postman

### Day 7 — Pizza Shop IVR

- [ ] 📝 Create the [Pizza Shop IVR](./Projects/Pizza%20Shop%20IVR/README.md)

### Day 8 — Database Persistence

- [ ] Learn the basics: tables, columns, primary keys, `SELECT` / `INSERT` / `UPDATE` / `DELETE`
- [ ] Install [DB Browser for SQLite](https://github.com/sqlitebrowser/sqlitebrowser/releases/download/v3.13.1/DB.Browser.for.SQLite-v3.13.1-win64.zip)
- [ ] Create a small SQLite database and inspect it — this is where the API data will live later

### Day 9 — IVR Audio Tools & Dynamic Prompts

- [ ] Use [PromptMatrixGenerator](https://github.com/moazmohamed20-ist/PromptMatrixGenerator) to generate `.wav` files from an Excel prompt matrix
- [ ] Use [GoldWave](https://goldwave.com/download.php?file=gw) to convert `.wav` files to **u-law 8000 Hz**
- [ ] Load the generated prompts into a Call Studio project
- [ ] Explore the IST SayItSmart plugins: `DigitByDigit`, `Number`, `Currency`

### Day 10 — Telecom IVR

- [ ] 📝 Create the [Telecom IVR](./Projects/Telecom%20IVR/README.md)

---

## Week 3 — Review & Building REST APIs

### Day 11 — IVR Review & Consolidation

- [ ] Side-by-side comparison: Pizza Shop IVR vs. Telecom IVR
- [ ] Identify reusable patterns (common menus, error handling, re-prompt logic)
- [ ] Q&A on IVR design best practices

### Day 12 — Products API (Part 1)

- [ ] Set up the Java project structure
- [ ] Implement `GET /products` and `GET /products/{id}`
- [ ] Test both endpoints manually

### Day 13 — Products API (Part 2) & Pizza Shop API

- [ ] Implement `POST /products`, `PUT /products/{id}`, `DELETE /products/{id}`
- [ ] Test all endpoints manually
- [ ] 📝 Submit the completed [Products API](./Projects/Products%20API/README.md)
- [ ] 📝 Create the [Pizza Shop API](./Projects/Pizza%20Shop%20API/README.md)

### Day 14 — API Review & Consolidation

- [ ] Compare the Products API vs. Pizza Shop API designs
- [ ] Discuss REST best practices: naming conventions, status codes, error responses
- [ ] Q&A

---

## Week 4 — IVR ↔ API Integration

### Day 15 — IVR ↔ API Integration: Pizza Shop

- [ ] Learn the `RestClient` element in Call Studio
- [ ] Understand how IVRs call APIs: request format, parsing responses
- [ ] Integrate the [Pizza Shop IVR](./Projects/Pizza%20Shop%20IVR/README.md) with the [Pizza Shop API](./Projects/Pizza%20Shop%20API/README.md)

### Day 16 — Telecom Full Integration

- [ ] 📝 Create the [Telecom API](./Projects/Telecom%20API/README.md)
- [ ] 📝 Integrate the [Telecom IVR](./Projects/Telecom%20IVR/README.md) with the Telecom API

---

<!-- ## Deliverables

| # | Deliverable | Day |
| :-- | :--- | :-- |
| 1 | [Pizza Shop IVR](./Projects/Pizza%20Shop%20IVR/README.md) | 7 |
| 2 | [Telecom IVR](./Projects/Telecom%20IVR/README.md) | 10 |
| 3 | [Products API](./Projects/Products%20API/README.md) | 12 – 13 |
| 4 | [Pizza Shop API](./Projects/Pizza%20Shop%20API/README.md) | 13 |
| 5 | Pizza Shop IVR ↔ Pizza Shop API integration | 15 |
| 6 | [Telecom API](./Projects/Telecom%20API/README.md) + Telecom IVR integration | 16 |

## Tools & Downloads

| Tool | First used | Purpose |
| :--- | :-- | :--- |
| [JDK 8](https://download.oracle.com/otn/java/jdk/8u461-b11/68ce765258164726922591683c51982c/jdk-8u461-windows-x64.exe?AuthParam=1754890059_d6d68a80f8210251e18a15f9ec3211bd) | Day 2 | Runtime required by Call Studio and the Java APIs |
| [Call Studio](https://istnetworkscom-my.sharepoint.com/:u:/g/personal/mgheta_istnetworks_com/ESvt5z_2JV1InI4WM5NgcjAB8VTBY8ikGSf3ry-RMortPg) | Day 2 | Designing IVR call flows |
| [VSCode](https://code.visualstudio.com/download) / [IntelliJ IDEA](https://www.jetbrains.com/idea/download) | Day 6 | Writing the REST APIs |
| [JSONPlaceholder](https://jsonplaceholder.typicode.com) | Day 6 | Practice API for exploring REST |
| [DB Browser for SQLite](https://github.com/sqlitebrowser/sqlitebrowser/releases/download/v3.13.1/DB.Browser.for.SQLite-v3.13.1-win64.zip) | Day 8 | Creating and inspecting the database |
| [PromptMatrixGenerator](https://github.com/moazmohamed20-ist/PromptMatrixGenerator) | Day 9 | Generating `.wav` prompts from an Excel matrix |
| [GoldWave](https://goldwave.com/download.php?file=gw) | Day 9 | Converting audio to u-law 8000 Hz | -->
