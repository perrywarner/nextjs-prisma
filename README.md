---
title: NextJS Prisma
description: A NextJS app using Prisma with a PostgreSQL database
tags:
  - next
  - prisma
  - postgresql
  - typescript
---

## 💁‍♀️ How to use

- [Provision a Postgres container on Railway](https://dev.new) and follow the [Getting Started](https://docs.railway.app/getting-started) docs or (TODO explain scenario where is already initialized)
- Connect to your Railway project with `railway link`
- Migrate the database `railway run yarn migrate:dev`
- Run the NextJS app ✨ with Postgres connection variables ✨ `railway run yarn dev` (`yarn dev` alone will not let you connect - see "[Run and Develop Your App](https://docs.railway.app/getting-started)" in Railway docs)

# NextJS Prisma Example

This example is a [NextJS](https://nextjs.org/) todo app that uses
[Prisma](https://www.prisma.io/) to store todos in Postgres.

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new?template=https%3A%2F%2Fgithub.com%2Frailwayapp%2Fexamples%2Ftree%2Fmaster%2Fexamples%2Fnextjs-prisma&plugins=postgresql)

## ✨ Features

- Prisma
- NextJS
- Postgres
- TypeScript

## 📝 Notes

This app is a simple todo list where the data is persisted to Postgres. [Prisma
migrations](https://www.prisma.io/docs/concepts/components/prisma-migrate#prisma-migrate)
can be created with `railway run yarn migrate:dev` and deployed with `railway run yarn migrate:deploy`. The Prisma client can be regenerated with
`yarn generate`.

[swr](https://swr.vercel.app/) is used to fetch data on the client and perform optimistic updates.
