# ![Building a CRUD App with Mongoose, Express, and EJS Lab - Exercise](./assets/hero.png)

## Introduction

For this lab you will be creating a resource, or schema, from which you will contstruct a full CRUD application using Mongoose, Express, and EJS

### Think of the Data

What kind of data would you like to CRUD?  The choice is entirely yours but certainly push yourself to think of a schema with data that reflects the complexity of things that you interact with in the real world.  Examples of resources you could make:

- Dogs
- Cars
- Blogs
- Clothing
- Food
- Planets

Once you have decided on a type of resource you would like to build a CRUD app for, think of how this data could be structured in a Mongoose Schema.  We have provided an example of a `Plant` schema for reference.  

```javascript
const mongoose = require('mongoose')
const Schema = mongoose.Schema

const Plant = new Schema(
  {
    name: { type: String, required: true },
    description: { type: String, required: true },
    image: { type: String },
  },
  { timestamps: true },
)

module.exports = mongoose.model('Plant', Plant)
```

### Methodically construct you application

## Lab exercise

The Minimum Viable Product (MVP) for this lab is to create an application that allows a user to complete full CRUD operations on the resource you have defined via the browser.  Make sure to focus on only piece of functionality at a time with this app.  As a part of the workflow of building an application of this size, please make sure to focus on iteratively testing out your functionality throughout the building process.