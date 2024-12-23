# Express.js JSON Body Parsing Issue

This repository demonstrates a common issue encountered when working with JSON request bodies in Express.js applications.

## The Problem

The provided `bug.js` file showcases an Express.js application that attempts to parse JSON data from a POST request. However, if the client doesn't send the correct `Content-Type` header (specifically, `application/json`), the request body will be empty, leading to unexpected behavior.

## Solution

The `bugSolution.js` file contains the corrected code. By using `express.json()` middleware, the solution handles different scenarios correctly and prevents potential errors caused by missing or incorrect headers.