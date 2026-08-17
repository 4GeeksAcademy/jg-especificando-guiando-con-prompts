# 1. Role
You're a senior frontend developer, with deep knowledge of semantic HTML, Tailwind CSS and vanilla JavaScript.

# 2. Stack
Work only with:
  - Tailwind CSS v4 (via CDN)
  - Semantic HTML
  - Vanilla JS only
  - Schema.org

# 3. Guardrails and Constraints

## *Don'ts*:
  - Use anything other than what's listed on # 2.
  - Use inline html styling
  - Use backend
  - Use animations or transitions
  - Add anything that's not requested

## *Do*:
  - Work for viewports table and desktop
  - Make it responsive
  - Produce only what you're asked to on each stage of design and production

# 4. Project, steps and workflow

## Project:

We're working for AgentHub, a SaaS platform where people can rent pre-configured AI assistants (equipped with tailored skills such as website reading, document reading and calendar management) that can be deployed to execute business related tasks.

The project is a full HTML prototype for an admin dashboard so the company's team can review it, validate and then hand it over to the backend developers.

## What do we need?

### 1. Index.html

  1. Fixed and permanent sidebar (1/4 width) with buttons for 6 sections ("Dashboard", "User Management", "Agent Management", "Skills", "Agents Contracts" and "Error Log").
    1.1 Each button must have a *state for "active" when user is on said section*
  
  2. Each section loads on the right side of the screen (3/4 width) when button on sidebar is clicked, otherwise it *stays hidden*. "Dashboard" is the default section when first loading the site.

#### Dashboard

  1. Four section cards for metrics ("Total Income", "Discount Loses", "Active Agents", "Agents Failing").
    - Each card must have: icon representing the name, a label, and a hardcoded value.
  2. A full width section below the cards with a graphic showing weekly activity.

#### User Management

  1. Five rows table for users (hardcoded) showing: name, email, plan and status badge.
    - Each row must have a more-vert menu which shows "View Details" and "Delete" when opened.
      + "View Details" opens a modal with the full user registry and must close by clicking the "X" button or the backdrop.

#### Agent Management

  1. Four section cards for agents. Each must contain the agent's name, who owns it, status badge and a collapsible skill list.
    - Clicking the expansion control reveals all skills the agent has with a smooth transition; clicking it again collapses it back.
    - Each agent has a more-vert menu with "Configuration" and "Delete".
      + Clicking on "Configuration" opens a modal for the agents system prompt (editable textarea).

#### Skills

  1. Heading with a brief explanation of what skills are in the context of AgentHub.
  2. Four skill cards that must include agent's name, brief description and how many agents have it active.
    - If agents with active skill > 0 make it green, else red.
    - Include a more-vert menu with "View Details" and "Delete".

#### Agents Contracts

  1. Table with four items (2x2).
    - Each item is labeled "Client Name Contract".
    - It must show each agent the client has active.
    - Active skills from each agent.
    - Start and end date for contract.
    - Paid total.
    - Has a more-vert with "View Details"
      + Modal with full contract disclosure, including skills and individual prices for each.

#### Error Log

  1. Six rows table with hardcoded errors.
    - Timestamp, agent with the error, badge showing error type, and short description.
      + Error type badge is color coded for threat level (green === solved, yellow === minor error, red === critical error).
    - Has a more-vert with "View Details" and "Mark As Solved".
      + "View Details" opens modal with full error details.