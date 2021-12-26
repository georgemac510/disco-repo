<img src="https://github.com/georgemac510/disco-repo/blob/master/public/Disco_Rock_Repo.png"/>

### Introduction

Try it online: https://disco-rock-repo.onrender.com/

The app is a repo of 1960's through 1990's popular music of the disco, classic rock, Brazilian jazz and other genres.
Users can store and retrieve audio and video files using IPFS for short-term storage and archive
for long-term storage using Filecoin. This is done through the magic of Textile Hub. IPNS Links to the data files are created for quick and easy retrieval. 

### Setup (Ubuntu)
Prerequisites: Node version 14.16.1

Start by cloning the repository:

```sh
git clone https://github.com/georgemac510/disco-repo.git
cd disco-repo/
```

- Create an `.env.local` file.
  - The command: `touch .env.local`.
- In this file you will want to include your Textile Hub keys and other secrets you don't want exposed to the client.

```sh
TEXTILE_HUB_KEY=XXX
TEXTILE_HUB_SECRET=XXX
IPFS_GATEWAY=https://ipfs.io
LIBP2P_KEY=
```

These keys can generated by

1) Downloading the latest version of the `hub` at https://github.com/textileio/textile/releases/tag/v2.6.13
2) Create a Hub account, then login with `hub login`.
3) View your keys with `hub keys ls`, then copy and paste the key and secret to the `.env.local` file.


Next,

```sh
npm install
npm run dev
```

Go to `http://localhost:3000` in your browser of choice. Can also be found at https://disco-rock-repo.onrender.com/
