# Spec: Bento Homepage Layout

## ADDED Requirements

### Requirement: Bento Grid Layout
The homepage MUST implement a responsive Bento-style grid layout.

#### Scenario: Grid configuration
The main content area uses a grid system that supports cells of varying sizes (1x1, 2x1, 2x2).

#### Scenario: Mobile responsiveness
On screens narrower than 768px, the grid collapses to a single column for readability.

### Requirement: Hero Section
The homepage MUST include a "Hero" bio section.

#### Scenario: Hero content
The most prominent grid item displays the user's name, title, and a brief "About" summary.

### Requirement: Featured Projects
The homepage MUST include a "Featured Projects" section.

#### Scenario: Project source
A subset of content from the `projects` section is displayed in grid cards.

#### Scenario: Project card details
Each project card displays a Title, Description snippet, and a Call-to-Action link.

### Requirement: Skills Display
The homepage MUST include a "Skills" or "Stats" display.

#### Scenario: Skill visualization
Specific cards are dedicated to listing technical skills or "dashboard-style" metrics (e.g., "Years Experience").

### Requirement: Social Footer
The homepage MUST include a Social Footer.

#### Scenario: Footer links
A footer section (or the final grid item) contains links to GitHub, LinkedIn, and Email.
