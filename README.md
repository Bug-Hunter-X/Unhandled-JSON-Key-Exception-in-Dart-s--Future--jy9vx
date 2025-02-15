# Unhandled JSON Key Exception in Dart

This repository demonstrates a common error in Dart applications that involves handling JSON responses from APIs.  The initial code example attempts to access a JSON key that might not always exist, leading to a runtime exception.  The solution shows how to safely access the key and gracefully handle the case where it's missing.

## Bug Description

The `fetchData` function fetches data from an API and parses the JSON response. It directly accesses `jsonData['someKey']` without checking if `someKey` exists. This will throw an exception if the response JSON doesn't contain this key.

## Solution

The improved version uses the `?` operator for null-aware access, preventing the runtime error.  It also includes better exception handling.
