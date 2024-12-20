# Next.js 15 MetadataRoute Cache-Control Header Issue

This repository demonstrates a bug in Next.js 15 where the Cache-Control header set in MetadataRoute is not working correctly. The issue affects the caching of static assets, potentially impacting performance and SEO.

## Bug Description

The `Cache-Control` header, when set within a `MetadataRoute`, is unexpectedly ignored. This prevents the browser from caching static assets effectively.

## Solution

A workaround is provided using a middleware approach to handle the caching logic.  This correctly sets the `Cache-Control` header.