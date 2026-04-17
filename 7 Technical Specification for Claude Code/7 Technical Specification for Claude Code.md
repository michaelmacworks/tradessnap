**7: Technical Specification for Claude Code**  
  
**Project Title:** Local SEO Programmatic CMS Architecture **Objective:** Build a "Hub-and-Spoke" CMS structure that automatically maps AI-generated Project Case Studies to specific Service and Location pages.  
**Project Title:** Local SEO Programmatic CMS Architecture **Objective:** Build a "Hub-and-Spoke" CMS structure that automatically maps AI-generated Project Case Studies to specific Service and Location pages.  
## 1. The Database Schema (Custom Post Types)  
Please build the following three collections/post types with these specific relationships:  
* **Collection 1: Services** (e.g., Roofing, Plumbing, HVAC)  
    * Fields: Service Name, Slug, Hero Image, SEO Description.  
* **Collection 2: Locations** (e.g., Blue Ash, Dublin, Westerville)  
    * Fields: City Name, State, Neighborhood Zip Codes, Google Map Embed Code.  
* **Collection 3: Project Case Studies** (The AI Output Destination)  
    * **Fields:** * Project Title (H1)  
        * Reference to **Service** (Multi-reference)  
        * Reference to **Location** (Single-reference)  
        * Before Photo (Image)  
        * After Photo (Image)  
        * The Problem (Text Area)  
        * The Solution (Rich Text)  
        * The Result (Text Area)  
        * JSON-LD Schema (Code/Text Area)  
## 2. The Logic Flow (The "Intelligence")  
When a new **Project Case Study** is published:  
* It must automatically appear in a "Recent Work" list on the corresponding **Service** page.  
* It must automatically appear in a "Local Projects" list on the corresponding **Location** page.  
* The page must dynamically generate a Call to Action (CTA) using the Business Name and the specific Location (e.g., "Need Roofing in Blue Ash? Call [Business Name] today!").  
## 3. SEO Requirements (The "Skeleton")  
* **Breadcrumbs:** Home > [Service] > [Project Title]  
* **Internal Linking:** Automatically link the City name in the Case Study back to the **Location Page**.  
* **Head Tags:** Ensure the JSON-LD Schema field from the CMS is injected into the <head> of the individual Project page.  
## 4. Front-End Mobile Optimization  
The site must be "Thumb-Friendly."  
* **Sticky Header:** Include a "Call Now" button that follows the user as they scroll.  
* **Image Slider:** A before/after slider component for the project photos.  
  
## How to use this with Claude Code  
When you open Claude Code, you can simply say:  
*"I am building a local SEO site for a contractor. Using the **Technical Specification** below, help me scaffold the CMS structure in [WordPress/Webflow] and write the logic for the dynamic internal linking."*  
*"I am building a local SEO site for a contractor. Using the **Technical Specification** below, help me scaffold the CMS structure in [WordPress/Webflow] and write the logic for the dynamic internal linking."*  
