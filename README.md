# SmartVoyage — AI-Powered WhatsApp Travel Assistant

**From a simple WhatsApp message to a personalized travel itinerary — powered by AI and workflow automation.**

SmartVoyage is an AI-powered travel planning and itinerary automation system. Built using n8n, AI agents, and multiple API integrations, the system is designed to simplify travel planning by collecting traveler preferences conversationally and automating itinerary generation and document delivery.

The project aims to reduce repetitive manual work for travel consultants while providing travelers with a convenient, personalized planning experience through WhatsApp.


## The Problem

Traditional travel planning often requires repeated conversations between travelers and travel consultants to collect trip preferences, research transportation and accommodation options, estimate costs, and prepare a detailed itinerary.

This process can be time-consuming and involves switching between multiple tools and information sources.

SmartVoyage explores how conversational AI and workflow automation can streamline these repetitive tasks.

## The Solution

SmartVoyage uses a WhatsApp-based conversational interface connected to an n8n automation workflow and AI models.

A traveler can communicate their requirements naturally rather than completing lengthy forms. The AI agent helps gather travel preferences, retrieve relevant travel information through configured integrations, prepare a cost estimate, and generate a personalized day-by-day itinerary.

The workflow is designed to produce a formatted PDF itinerary and deliver it to the traveler by email.

## How It Works

1. **Traveler sends a message:** The traveler initiates a conversation through WhatsApp.

2. **Conversational requirement gathering:** An AI agent powered by OpenAI and Groq helps understand the travel request and collect details such as destination, dates, departure city, transportation, hotel preferences, budget, food preferences, and interests.

3. **Destination suggestions:** If the traveler has not decided on a destination, the workflow can use available brochure information to suggest suitable options.

4. **Travel information retrieval:** Configured API integrations retrieve relevant flight, hotel, train, and weather information.

5. **Cost estimation and confirmation:** The workflow prepares an estimated travel budget and requests traveler approval before proceeding.

6. **Itinerary generation:** Google Gemini generates a structured, day-by-day itinerary based on the collected preferences and available information.

7. **Document creation:** Google Docs and Google Drive integrations are used to prepare and convert the itinerary into a PDF document.

8. **Email delivery:** The completed itinerary is sent to the traveler using Gmail integration.

## Key Features

- WhatsApp-based conversational travel planning
- AI-assisted collection of trip requirements
- Destination suggestions based on available brochure information
- Integration with external travel and weather information sources
- Estimated travel budget preparation
- Traveler confirmation before itinerary generation
- Personalized day-by-day itinerary generation
- Automated Google Docs and PDF document preparation
- Email delivery of the generated itinerary
- Workflow orchestration through n8n

Feature availability depends on the configured integrations, API access, and workflow implementation.

## Technology Stack

| n8n |                                         | Workflow orchestration and automation |
| WhatsApp API                                  | Conversational interface |
| OpenAI                                        | AI-assisted conversation and tool use |
| Groq                                          | LLM integration |
| Google Gemini                                 | Itinerary generation |
| Google Docs                                   | Document creation |
| Google Drive                                  | Document storage and PDF conversion |
| Gmail                                         | Email delivery |
| Google Sheets                                 | Structured data and workflow support |
| Google Flights and Hotels SERP APIs           | Travel information retrieval |
| OpenWeather API                               | Weather information |
| Apify railway APIs                            | Railway information retrieval |
| Prompt engineering                            | Instruction design and output consistency |
| AI agents and tool calling                    | Conversational reasoning and integration orchestration |


The project brought together several stages of a travel-planning process into a connected workflow, from the initial WhatsApp message to the generated itinerary and email delivery.

### Key Learnings

- AI agent development and tool calling
- n8n workflow design
- LLM API integration
- Prompt engineering and output validation
- Multi-API integration
- Conversational AI
- Business process automation
- Automated document generation and delivery

## Business Value

SmartVoyage demonstrates how AI and workflow automation can help reduce repetitive travel-planning tasks, standardize information gathering, and accelerate the preparation of personalized itineraries.

The project was designed to reduce a manual planning process that could take approximately 20–30 minutes to a process completed within a few minutes, depending on API response times, workflow execution, and the complexity of the trip.

## Future Improvements

- Add stronger validation of travel information and generated itineraries.
- Improve error handling and retry mechanisms for failed API requests.
- Add multilingual conversational support.
- Introduce itinerary editing and regeneration based on traveler feedback.
- Add automated workflow monitoring and execution logs.
- Evaluate itinerary quality using a consistent test dataset.


This project helped me gain practical experience in AI agent development, n8n workflow automation, LLM integrations, prompt engineering, and multi-API orchestration.

