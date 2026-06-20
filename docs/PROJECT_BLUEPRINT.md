# Project Blueprint

# Masjid Syukur Website

Version: 1.0

Status: Draft

Last Updated: June 2026

---

# 1. Overview

This document describes the logical structure of the Masjid Syukur platform.

It acts as the primary reference for:

* Domain modeling
* Feature planning
* Administrative structure
* Future system expansion

This document should remain stable even as implementation details evolve.

---

# 2. Core Principles

The system should be:

* Content Driven
* Admin Friendly
* Maintainable
* Extensible
* Low Cost
* Easy to Understand

The platform should prioritize simplicity over complexity.

---

# 3. Domain Overview

The platform consists of six primary domains.

## Identity Domain

Represents the mosque itself.

Purpose:

Provide official information about Masjid Syukur.

Modules:

* Profile
* Vision
* Mission
* Management Structure
* Facilities

---

## Program Domain

Represents mosque activities and initiatives.

Purpose:

Inform visitors about available programs.

Modules:

* Programs
* Program Categories

Examples:

* Kajian
* Social Programs
* Education
* Youth Activities
* Ramadan Programs

---

## Content Domain

Represents published content.

Purpose:

Educate, inform, and document activities.

Modules:

* Articles
* Categories
* Announcements

Examples:

* Islamic Articles
* News
* Activity Reports

---

## Media Domain

Represents visual documentation.

Purpose:

Archive and display mosque activities.

Modules:

* Galleries
* Albums
* Media Assets

---

## Community Domain

Represents interaction with visitors.

Purpose:

Support communication and participation.

Modules:

* Contact Messages
* Event Registrations

---

## Donation Domain

Represents fundraising activities.

Purpose:

Support digital donations and transparency.

Modules:

* Donation Campaigns
* Donations
* Donation Reports

---

# 4. Administrative Domains

The administration panel should be organized around content management rather than technical concepts.

Primary Admin Sections:

* Profile Management
* Program Management
* Content Management
* Media Management
* Donation Management
* User Management

---

# 5. User Roles

## Super Admin

Responsibilities:

* Full system access
* User management
* Configuration management

Permissions:

* All permissions

---

## Admin

Responsibilities:

* Manage all content
* Manage programs
* Manage galleries
* Manage announcements

Permissions:

* Content management
* Media management
* Program management

---

## Editor

Responsibilities:

* Publish articles
* Upload galleries

Permissions:

* Limited content management

---

# 6. Public Website Structure

## Home

Purpose:

Provide quick access to important information.

Contains:

* Hero
* About
* Featured Programs
* Latest Content
* Contact Summary

---

## Profile

Contains:

* History
* Vision
* Mission
* Organization Structure
* Facilities

---

## Programs

Contains:

* Program Listing
* Program Detail

---

## Blog

Contains:

* Article Listing
* Article Detail

---

## Gallery

Contains:

* Gallery Listing
* Gallery Detail

---

## Announcements

Contains:

* Announcement Listing
* Announcement Detail

---

## Donations

Contains:

* Campaign Listing
* Campaign Detail

---

## Contact

Contains:

* Contact Information
* Contact Form

---

# 7. Primary Entities

The following entities are expected to exist throughout the life of the project.

## Phase 1

* User
* Profile
* Program
* ProgramCategory
* ContactInformation

---

## Phase 2

* Article
* ArticleCategory
* Gallery
* GalleryItem
* Announcement

---

## Phase 3

* DonationCampaign
* Donation
* DonationReport
* Event
* EventRegistration

---

# 8. Relationships

## Program Domain

ProgramCategory

has many

Program

---

## Content Domain

ArticleCategory

has many

Article

---

## Media Domain

Gallery

has many

GalleryItem

---

## Donation Domain

DonationCampaign

has many

Donation

---

## Event Domain

Event

has many

EventRegistration

---

# 9. Navigation Strategy

Public navigation should remain simple.

Maximum top-level menus:

* Home
* Profile
* Programs
* Blog
* Gallery
* Donations
* Contact

Avoid excessive menu nesting.

---

# 10. Content Ownership

Every content entity should support:

* Author
* Published Status
* Publication Date

Purpose:

Support future content governance.

---

# 11. SEO Considerations

Content-oriented entities should support:

* Slug
* Meta Title
* Meta Description

Applicable Entities:

* Program
* Article
* Announcement
* Donation Campaign

---

# 12. Future Expansion Guidelines

Future features should integrate into existing domains whenever possible.

Examples:

Volunteer Registration

→ Community Domain

Educational Videos

→ Content Domain

Fundraising Campaigns

→ Donation Domain

Avoid creating new domains unless necessary.

---

# 13. AI Agent Instructions

Before implementing any feature:

1. Identify the target domain.
2. Verify the feature exists in the roadmap.
3. Reuse existing entities when possible.
4. Avoid introducing duplicate concepts.
5. Maintain consistency with PRD and ROADMAP.

If a requested feature does not fit an existing domain, evaluate whether:

* The feature belongs to a future roadmap phase.
* The feature can extend an existing domain.
* A new domain is truly required.
