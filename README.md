Ember Practice

This repository contains my personal EmberJS practice project, created while following the official Ember tutorial and the CCC onboarding material for Ember development.

The main goal of this project was to become familiar with Ember’s development workflow, project structure, routing system, components, templates, testing approach, and data handling patterns.

I completed the tutorial using Ember 6.11, which is close to the version currently used in some CCC projects, and also reviewed the Ember 5.4 tutorial as part of the onboarding process.

Project Overview

The application built in this repository is based on the official Ember Super Rentals tutorial.

Super Rentals is a small rental listing application where users can browse rental properties, navigate between pages, view property details, interact with UI components, and work with data loaded through Ember routes and EmberData.

Through this project, I practiced the most important concepts needed to understand and contribute to Ember-based applications.

What I Practiced

Ember CLI and Project Setup

I started by creating a new Ember application using Ember CLI. This helped me understand the basic structure of an Ember project and the purpose of the main folders and files.

I practiced:

* Creating a new Ember app
* Running the development server
* Working with live reload
* Understanding the app, public, config, and tests folders
* Adding static assets and global styles
* Using Ember’s file conventions

Routing and Pages

I created several routes and templates for the application, including the home page, about page, contact page, and individual rental detail pages.

This helped me understand how Ember maps URLs to route templates and how navigation works inside a single-page application.

I practiced:

* Defining routes in router.js
* Creating route templates
* Customizing route paths
* Using the <LinkTo> component for internal navigation
* Working with dynamic route segments such as /rentals/:rental_id
* Accessing route parameters inside the route model hook

Templates and Components

A major part of the tutorial focused on building reusable UI with Ember components.

I started with simple template-only components and later moved into Glimmer components with JavaScript classes when behavior or state was needed.

I practiced:

* Creating reusable components
* Extracting duplicated markup into components
* Passing content with {{yield}}
* Passing data through component arguments
* Using ...attributes to forward HTML attributes
* Organizing components in folders
* Creating namespaced components such as rental/image
* Keeping components focused and reusable

Some of the components created during the tutorial include:

* Jumbo
* NavBar
* Rental
* RentalImage
* Map
* RentalDetailed
* ShareButton
* Rentals
* RentalsFilter

Component State and Interactivity

I also practiced adding behavior to components using Glimmer component classes.

This included making components interactive and managing internal state.

I practiced:

* Creating component classes with @glimmer/component
* Using @tracked properties
* Creating computed values with getters
* Handling user interactions with @action
* Using element modifiers such as {{on}}
* Adding conditional rendering in templates
* Building an interactive image component that can toggle between small and large views

Working With Data

The tutorial gradually moved from hard-coded data to route-based data loading.

I practiced loading data through Ember route files and using the model() hook to prepare data for templates.

I also worked with local static JSON files to simulate server responses.

I practiced:

* Creating route files
* Returning data from the model() hook
* Accessing route data through @model
* Fetching data from static JSON endpoints
* Adapting JSON data before rendering it
* Rendering lists with {{#each}}
* Passing loaded data into components

EmberData

Later in the tutorial, I refactored duplicated route data-loading logic by using EmberData.

This helped me understand how Ember applications can manage application data in a more structured way.

I practiced:

* Creating EmberData models
* Defining model attributes
* Moving computed data such as rental type into the model
* Loading models from routes
* Using the EmberData store
* Understanding the purpose of adapters and serializers
* Reducing duplicated data-fetching logic across routes

Services and Dependency Injection

I practiced using Ember services to share behavior across the application.

The main example was the share button feature, where the current route information was needed to generate a shareable URL.

I practiced:

* Creating reusable services
* Injecting services into components
* Using the router service
* Avoiding global variables where a service is more appropriate
* Mocking services in tests

Provider Component Pattern

I also practiced the provider component pattern while implementing the rental search feature.

This helped me understand how a component can manage data or filtering logic and yield the result back to the caller.

I practiced:

* Creating a search form
* Handling input and submit events
* Storing the search query as tracked state
* Filtering rental results
* Yielding data from one component to another
* Using block parameters when invoking components

Testing

Testing was an important part of the tutorial. I added tests while building the application to make sure each feature continued to work after refactors.

I practiced:

* Writing acceptance tests
* Writing component/rendering tests
* Using QUnit
* Using Ember test helpers such as visit, click, currentURL, and render
* Testing navigation between routes
* Testing component output
* Testing user interactions
* Testing components with router access
* Reusing setup logic with beforeEach
* Mocking services in tests

This gave me a better understanding of how Ember encourages test-driven and regression-safe development.

Main Concepts Learned

By completing this project, I became more comfortable with:

* Ember CLI
* Ember project conventions
* Routing and route templates
* Dynamic routes
* Glimmer components
* Template-only components
* Component arguments
* {{yield}}
* ...attributes
* Tracked state
* Actions and modifiers
* Route model hooks
* EmberData models and store
* Services and dependency injection
* Provider components
* Automated testing with QUnit and Ember test helpers

Purpose of This Repository

This repository is not intended to be a production application. It is a learning and practice project created to document my progress while learning EmberJS.

The work done here helped me build the foundation needed to contribute to Ember-based projects at CCC, especially upcoming work related to CKATKT.
