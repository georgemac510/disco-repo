### Introduction

Try it online: https://crimson-cake-6149.on.fleek.co/

The app is a repo of 1960's and 1970's 

### Setup (MacOS)

Start by cloning the repository, or by clicking on **Use this template** above.

```sh
git clone git@github.com:application-research/next-bucket.git
cd next-bucket
```

- Create a `.env.local` file.
  - The command: `touch .env.local`.
- In this file you will want to include your Textile Hub keys and other secrets you don't want exposed to the client.

```sh
TEXTILE_HUB_KEY=XXX
TEXTILE_HUB_SECRET=XXX
IPFS_GATEWAY=https://ipfs.io
```

The easiest way to generate your `user group` keys for Textile is to download the latest version of the `hub` https://github.com/textileio/textile/releases/tag/v2.6.6

- Stuck? Read this: [https://docs.textile.io/hub/apis/](https://docs.textile.io/hub/apis/).
  - Still stuck? Post an issue if you have any questions :-)

Next,

```sh
npm install
npm run dev
```

Go to `http://localhost:3001` in your browser of choice.
