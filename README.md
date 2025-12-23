# Dialogflow CX Pizza Ordering Agent

---

## Overview and System Architecture 
This project is a conversational AI agent built using Google Dialogflow CX, focusing on flow design, state management, and natural language interaction. The agent simulates a full pizza ordering and checkout experience through both text based and custom payload interaction. The user is thus guided through:
1. Selecting Pizza
2. Adding Toppings
3. Specifiying Drinks and/or Desserts
4. Reviewing their Order
5. Collecting Customer Details
6. Completing Checkout

The agent is structured around two primary Dialogflow CX flows:

- **Pizza Order Flow**: Manages order initiation, pizza selection (signature or custom), toppings, drinks, sides, and order review.
- **Payment Flow**: Handles customer information collection, payment method selection, order confirmation, and order modification or cancellation.

These flows are connected through route groups and conditional transitions, allowing users to restart orders, revise customer details, or cancel orders at multiple points in the conversation. The **attached report section** goes into full depth in regards to conception, theoretical business implications, and further techincal aspects with imagery. The **attached video demo section** explores the conversational flow at work, for a signature and custom pizza respectively.

---

## Project Context
This project was developed as final group project of three for the course: **ADTA 5750 Applied Natural Language Processing** during Winter 2025. My key contribution involved the design and implementation of the conversational agent itself. This entails flow architecture, page routing, intent handling, and dialog logic within Dialogflow CX. This team efficiently collaborated in business application and conceptual brainstorming; assessing the preliminary areas that defined entity categories & intents. Partners respectively handled the creation of the preconditional lucidchart erd diagram draft, and in class presentation slides.

This repository presents the system as a standalone portfolio case study, consolidating the technical design, implementation details, and testing outcomes into a single, curated format.

---

## Platforms, Tools, & Feature Implementation 

- **Google Dialogflow CX** — Core conversational AI platform used for flow-based dialog design, state management, and multi-path conversation handling
- **Dialogflow Messenger & Custom Payloads (JSON)** — Used to enhance usability through interactive UI elements alongside text-based responses
- **Lucidchart** — Used to design and visualize the ERD and system data relationships
- **Multi-Flow Architecture** — Separate Pizza Order and Payment flows connected through route groups and conditional transitions
- **Intent-Based Routing** — User intents trigger page transitions, confirmations, corrections, and flow jumps
- **Entity-Driven Selection** — Entities capture structured inputs such as pizza size, crust type, toppings, drinks, and payment method
- **Conditional Responses** — Order summary logic dynamically checks which parameters were collected or skipped before generating responses
- **Event Handlers** — No-match and no-input handlers that prompt correct input before further advancement when input is unclear or missing
- **State Management with Parameters** — Session parameters persist user selections across pages and flows


