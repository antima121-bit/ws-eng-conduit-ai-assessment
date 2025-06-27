# Conduit

This repository contains a full-stack TypeScript application consisting of a NestJS backend and an Angular frontend.

Prerequisites:
 - Docker or a locally running MySQL installation
 - NodeJS 16+ (tested with v18.13.0)
 - Code Editor (VSCode is recommended)

Getting started:
 - Install the dependencies `npx yarn install`.
 - If you don't have a local MySQL installation, start one in docker: `docker run -d -p 3306:3306 --name mysql -e MYSQL_ROOT_PASSWORD=conduit -e MYSQL_DATABASE=conduit -e MYSQL_USER=conduit -e MYSQL_PASSWORD=conduit mysql:8.1`
 - Adjust the `apps/backend/mikro-orm.config.ts` with your MySQL credentials (they already match the ones from the docker command above).
 - Start the app (both backend and frontend at once): `npm start`.
 - After the backend successfully starts, in a new terminal `npm run seed` to seed the database with some initial data.
 - You can now access the UI at http://localhost:4200 and login with `jcosten0@purevolume.com` / `password`.
 - You can also find the backend API spec at http://localhost:3000/docs.


MIT License

Copyright (c) [2018-2022] [Lignos Stefanos]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
