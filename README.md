# Flask + Tailwindcss + DaisyUI + HTMX + Alpine.js Boilerplate

This project is a template for building modern web applications using Python
with Flask, Tailwindcss, DaisyUI, HTMX, and Alpine.js. The goal is to optimize
development velocity and performance by minimizing client-side state management and custom CSS.

## Stack

### Python with Flask

Provides a minimal, unopinionated WSGI web framework for Python, enabling rapid development of server-side logic with extensible routing and templating.

### Tailwindcss

Delivers a utility-first CSS framework that generates styles directly from HTML, reducing the overhead of custom CSS.

### DaisyUI

Extends Tailwindcss with a library of pre-designed, accessible UI components, standardizing visual design and reducing frontend implementation time.

### HTMX

Facilitates hypermedia-driven server responses via HTML attribute extensions, replacing complex client-side SPA state management with server-rendered updates.

### Alpine.js

Provides lightweight, declarative client-side reactivity without Virtual DOM overhead, enabling component-level interactivity in server-rendered HTML.

This architecture prioritizes server-side rendering and declarative client-side interactions, reducing the overhead of managing complex client-side state and custom styles.

## Prerequisites

Ensure you have Nix installed on your machine to setup the packages and development environment:

- Install Nix: Follow the instructions at
  [NixOS.org](https://nixos.org/download.html).

## Set Up Development Environment

To set up and enter the development environment:

```bash
nix develop
```

The `flake.nix` file in the repository automatically handles the creation of a
development environment with all the necessary dependencies for both the backend and
frontend.

## Running The Application

From within the Nix environment, the development server is accessible at `http://localhost:5000`. Python backend changes trigger automatic reloads; template modifications require a manual browser refresh.

## Check for Dependency Updates

Nix will check for the latest versions of tools whenever you run:

```bash
nix flake update
```

Updates the flake.lock file to pin the latest upstream versions.
