# Project Configuration

## Skills (123 total)

### Designer Skills (65) — design, build, deliver
- **Design Research** — personas, empathy maps, journey maps, interviews, usability testing
- **Design Systems** — tokens, components, accessibility, theming, documentation
- **UX Strategy** — competitive analysis, design principles, experience mapping, alignment
- **UI Design** — color systems, typography, layout grids, responsive, dark mode
- **Interaction Design** — micro-interactions, animations, state machines, gestures, error handling
- **Prototyping & Testing** — wireframes, heuristic evaluation, A/B testing, user flows
- **Design Ops** — critique, handoff specs, sprint planning, QA checklists, workflows
- **Designer Toolkit** — rationale, presentations, case studies, UX writing, adoption
- **Frontend Design** — distinctive, production-grade UI code (Anthropic official)
- **shadcn/ui** — Radix UI + Tailwind CSS component patterns

### Inclusive Design Skills (58) — accessibility, inclusion, cognitive a11y
- **Cognitive Accessibility** — cognitive load, plain language, wayfinding, memory, focus, error recovery
- **Inclusive Interaction** — keyboard nav, gestures, voice, touch targets, motion sensitivity, multi-modal
- **Accessible Content** — alt text, headings, forms, links, tables, readable content, plain language
- **Inclusive Personas** — disability personas, assistive tech scenarios, ability spectrum, edge cases
- **Adaptive Interfaces** — color independence, flexible typography, simplified views, user preferences
- **Accessibility Decisions** — compliance mapping, debt tracking, tradeoff analysis, handoff, testing strategy

## Agents (8 — auto-activate)
Just talk naturally. Claude picks the right agent based on your task.

## How Skills Layer Together
Designer skills build the system. Inclusive skills extend it for accessibility. Use together:
1. Design gestures → then design gesture alternatives
2. Build color system → then audit for color independence
3. Create personas → then expand with disability dimensions
4. Define animations → then check motion sensitivity
5. Write component spec → then verify keyboard navigation
6. Create typography scale → then ensure flexible typography
7. Design layouts → then audit responsive accessibility

## How to Use
- Skills load automatically from `.claude/skills/`
- Commands available as slash commands from `.claude/commands/`
- Agents auto-activate from `.claude/agents/`
- MCP servers (Puppeteer, Chrome DevTools) configured in `.mcp.json`
- Run `./setup.sh` on a new machine to install marketplace plugins

## Project Conventions
- Adapt all design outputs to the project's existing stack and conventions
- Prioritize accessibility (WCAG AA minimum) in all design decisions
- Use design tokens over raw values whenever possible
- Design for keyboard, screen reader, and reduced motion from the start
- Include disability as a natural dimension in all personas and user stories
