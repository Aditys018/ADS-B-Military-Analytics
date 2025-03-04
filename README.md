# ADS-B Military Analytics

[![Deploy to Firebase Hosting](https://github.com/EMcNugget/adsb_mil_data/actions/workflows/firebase-hosting-merge.yml/badge.svg)](https://github.com/EMcNugget/adsb_mil_data/actions/workflows/firebase-hosting-merge.yml)
[![CodeQL](https://github.com/EMcNugget/adsb_mil_data/actions/workflows/codeql.yml/badge.svg)](https://github.com/EMcNugget/adsb_mil_data/actions/workflows/codeql.yml)
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/5caa91f758e54d11b3034743d903a1b8)](https://www.codacy.com/gh/EMcNugget/ADS-B-Military-Analytics/dashboard?utm_source=github.com&utm_medium=referral&utm_content=EMcNugget/ADS-B-Military-Analytics&utm_campaign=Badge_Grade)

## What is this?

This allows you to view military aircraft from an ever growing database. Find out how many aircraft flew on a specific day, what type, among other features that are coming soon!

![Screenshot](./util/demo.png)

## Requirements

- ![Node.js][node.js]

- ![Python][pyreq]

## How To Run

1.  Get an API key from ADS-B Exchange (<https://www.adsbexchange.com/data>)

2.  To configure the system, you need to define two environment variables named `API_KEY` and `API_HOST` using the provided key and host values. Additionally, you will require a MongoDB instance for the backend, and you can use the naming conventions specified in the [main.py](./server/main.py)
    file. Moreover, you might have to modify the URL in the api_fetch.tsx file located in client/src/components to match the URL of your Flask instance.

3.  Create a python virtual environment and then run the following commands in the root directory of the project:

```bash
npm run init
npm start
```

###### Note: If you are using Windows, you might have to run the following command instead:

```batch
npm run wininit
npm run winrun
```

4.  View the development server at <http://localhost:5173>

## Tech Stack

|       Backend       |     Frontend      |
| :-----------------: | :---------------: |
|    ![Python][py]    | ![TypeScript][ts] |
|   ![Flask][flask]   |  ![React][react]  |
|   ![MongoDB][mdb]   |   ![Vite][vite]   |
| ![Google Cloud][gc] |  ![Firebase][fb]  |
|                     |   ![SCSS][scss]   |

## Architecture

![Architecture](./util/architecture.svg)

## Current Tasks

See the project board for the current tasks.
[Roadmap and Tasks][rm]

## Change Log

See [CHANGELOG.md](./CHANGELOG.md)

## Questions, Comments, Concerns?

Feel free to contact me at <support@adsbmilanalytics.com> or open an issue on this repository.

[ts]: https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white
[flask]: https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white
[py]: https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54
[react]: https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB
[mdb]: https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white
[gc]: https://img.shields.io/badge/GoogleCloud-%234285F4.svg?style=for-the-badge&logo=google-cloud&logoColor=white
[vite]: https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white
[scss]: https://img.shields.io/badge/SCSS-hotpink.svg?style=for-the-badge&logo=SASS&logoColor=white
[fb]: https://img.shields.io/badge/firebase-%23039BE5.svg?style=for-the-badge&logo=firebase
[rm]: https://github.com/users/EMcNugget/projects/6
[pyreq]: https://img.shields.io/badge/Python-3.11.2-blue?style=flat&logo=python
[node.js]: https://img.shields.io/badge/Node.js-v18.15.0-green?logo=node.js&style=flat
