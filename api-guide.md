# API Guide

## Overview

This guide explains explains how to retrieve a post by its ID using the JSONPlaceholder API.

## Base URL

https://jsonplaceholder.typicode.com

## Endpoint

GET /posts/{id}

Retrieves a post by its ID.

## Path Parameters

| Parameter | Type | Required | Description |
| ----------|------|----------| ------------|
| id | integer | Yes | The ID of the post to retrieve. |

## Example Response

The following example illustrates the response structure for GET /posts/1. The string values are simplified for clarity.

```json
{
  "userId": 1,
  "id": 1,
  "title": "Example post title",
  "body": "Example post content"
}
```

## Response Fields

| Field | Type | Description |
| ------|------| ------------|
| userId | integer | The ID of the post's author. |
| id | integer | The ID of the post. |
| title | string | The title of the post. |
| body | string | The content of the post. |

## Response Status Codes

| Status Code | Description |
|-------------|-------------|
|200 OK | The request was successful, and the post data was returned. |
|404 Not Found | No post was found with the specified ID. |

## Error Response

If the specified post does not exist, the API returns HTTP 404 with an empty JSON object.

```json
{}
```
