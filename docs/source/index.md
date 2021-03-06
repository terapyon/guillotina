# Guillotina: The Python AsyncIO REST API Framework

Guillotina is the only full-featured Python AsyncIO REST Resource Application
Server designed for high-performance, horizontally scaling solutions.

## Why Guillotina

 - **Performance**: Traditional Python web servers limit the number of simultaneous
   requests to the number of threads running the server. With AsyncIO, you are
   able to serve many more simultaneous requests.
 - **Front-end friendly**: Guillotina is designed to make your
   JavaScript engineers happy. With things like automatic Swagger documentation
   for endpoints, out of the box CORS and websockets, your front-end team will be happy
   to work with Guillotina. We speak JSON but can adapt to any content type
   payload request/response bodies.
 - **AsyncIO**: With AsyncIO, websockets are simple. More interestingly, AsyncIO
   is an ideal match with microservice architectures.
 - **Object model**: Guillotina uses a hierarchial object model. This hierarchy
   of objects then maps to URLs and is perfect for managing
   a large number of objects.
 - **Security**: Guillotina has a granular, hierarchical, multidimensional
   security system that allows you to manage the security of your content
   at a level not available to other frameworks.
 - **Scale**: With integrations like Redis, ElasticSearch and Cockroach, you
   have the tools to scale.

# Getting Started

Are you new to Guillotina? This is the place to start!

[Quick tour of Guillotina](./quick-tour.html) gives an overview of the major features in
Guillotina, covering a little about a lot.

Need help? Join our [Gitter channel](https://gitter.im/plone/guillotina).

# Training / Tutorial

To learn more, go to the [training section](./training/index.html).
You can learn basics and find topics about Guillotina:

```eval_rst
.. toctree::
   :maxdepth: 2

   training/index
```

# REST API

After you're up and running, primarily, Guillotina provides a REST API to work with
and it is what you should become the most familiar with.

Guillotina API structure mirrors the object tree structure. Within the object
tree structure, there are four major types of objects you'll want to be familiar
with:

- Application: The root of the tree: `/`
- Database: A configured database: `/(db)`
- Container: An main object to add data to: `/(db)/(container)`
- Content: Item or Folder by default. This is your dynamic object tree you create

The endpoints available around these objects are detailed below:

```eval_rst
.. toctree::
   :maxdepth: 1
   :glob:

   rest/application
   rest/db
   rest/container
   rest/item
   rest/folder
```

# Narrative Developer Documentation

After reading quick tour or training section,
Now you can start hands-on style guide to learn how to use it.

```eval_rst
.. toctree::
   :maxdepth: 2

   developer/narrative
   developer/security
   developer/roles
   developer/applications
   developer/addons
   developer/services
   developer/render
   developer/contenttypes
   developer/behavior
   developer/interfaces
   developer/events
   developer/commands
   developer/applicationconfiguration
   developer/design
   developer/persistence
   developer/blob
   developer/router
   developer/exceptions
   developer/fields
   developer/serialize
   developer/async_utils
   developer/component-architecture
   developer/debugging
```

# Deploying

- [Installing guillotina](./installation/installation.html)
  is simply done with pip but if you need to run with docker,
  [we also have you covered](https://hub.docker.com/r/guillotina/guillotina/).
- Guillotina has an quite a few
  [configuration options](./installation/configuration.html)
  you might be curious about.
- You can also setup
  [logging configuration](./installation/logging.html).
- Finally, you may also need to put Guillotina
  [behind a proxy](./installation/production.html)
  when you deploy it.

# Migration

- [< 4.3 to 4.3](./migration/4.3.html)

# Programming API Reference

```eval_rst
.. toctree::
   :maxdepth: 1

   api/configure
   api/content
   api/request
   api/response
   api/fields
   api/utils
   api/component
```

# About

- [Read about](./about.html) the rich history of the project

```eval_rst
 .. toctree::
    :hidden:
    :glob:

    developer/*
    installation/*
    training/*
    *
```
