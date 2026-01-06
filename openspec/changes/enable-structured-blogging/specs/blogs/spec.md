# Spec: Blog System

## ADDED Requirements

### Requirement: Blog Metadata Visibility
The blog layouts MUST conditionally display metadata based on presence.

#### Scenario: Selective Metadata
If a blog has a `project` field but no `tags`, only the project link is shown.

### Requirement: Homepage Blog Feed
The homepage MUST feature a "Blogs" section replacing older placeholders.

#### Scenario: Replacement of Alpha/Beta
The grid items previously occupied by "Project Alpha" and "Project Beta" are replaced by a feed or link to the latest blog posts.

### Requirement: Archive Listing
The site MUST provide a dedicated route at `/blogs` for browsing content.

#### Scenario: Paginated List
A vertical list of blog summaries with date and title.
