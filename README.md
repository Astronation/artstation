# artstation

This is the source code automating the processes of ArtStation - the first star station in the virtual world of Astronation. 
ArtStation is showcasing and trading visual NFTs in the metaverse, while integrating several blockchains 

https://astronation.world/entities/a883f9a1-b90a-4a0a-84a0-e4818e5ce217

## Key components
1. [Vue Notus template](https://github.com/creativetimofficial/vue-notus) from [Creative Tim](https://www.creative-tim.com/)
2. [Tailwind CSS framework](https://github.com/tailwindlabs/tailwindcss)
3. [Vue.js framework](https://github.com/vuejs/)
4. [Apollo and GraphQL for Vue.js](https://github.com/vuejs/apollo)

## Integrated blockchains and services
1. [Arweave.org](https://docs.arweave.org/developers)
2. [Deso.org](https://docs.deso.org)
3. [community.xyz](https://github.com/CommunityXYZ/community-js)
4. [deso.ninja](https://deso.ninja/documentation)

## Processes

### Getting ART tokens
1. User transfers of 0.01+ $artstation CC to @artstation
2. User DM to @artstation - providing signature to the Arweave public key - `Arweave key for @artstation: <somepkey>`
3. DesoNinja receives the DM and starts the mint of ART tokens to signed Arweave public key
4. DesoNijna informs voters about a new vote on @artstation account and website
5. Votes on accepting the mint of new ART tokens
6. Optional, on failed vote or timeout: Deso Ninja transfers $artstation CCs back to the sender

### Being a governing member
1. User has tokens locked in the community vault (TBD lock periods)
2. Votes on accepting NFTs for showcase (metadata: commision, min auction, buy now)
3. Votes on removing NFTs from showcase (or should this be automatic)

### Automatic processes of the station
1. Preparing NFT showcase assets and storing them in Arweave
2. Local NFT showcase assets cache handling in VR clients.

## Developer setup

- Go to your file project (where you’ve unzipped the product)
- (If you are on a linux based terminal) Simply run `npm run install:clean`
- (If not) Run in terminal `npm install`
- (If not) Run in terminal `npm run build:tailwind` (each time you add a new class, a class that does not exist in `src/assets/styles/tailwind.css`, you will need to run this command)
- (If not) Run in terminal `npm run serve`

## Deployment process

1. Lint and fix files - `npm run lint`
1. *One time*: Install [arkb](https://github.com/textury/arkb) `npm install -g arkb`
1. *One time*: Link your Arweave wallet with arkb `arkb ws path\to\wallet.json`
1. Update the version number in `package.json`
1. Build the distribution package `npm run build`
1. Upload the `dist` folder `arkb deploy ./dist --bundle --license MIT --tag-name App-Name --tag-value ArtStation --tag-name App-Version --tag-value 0.1.4`
1. Commit the deployed url and build version `git commit -am"0.1.4 - https://arweave.net/IM1MpeGd0DM_zy359lq4EQ8us4WvsMYToG3-00mhUw0"`

### Customize design

1. [Vue Notus](https://github.com/creativetimofficial/vue-notus) is built with over frontend 120 components, giving you the freedom of choosing and combining. All components can take variations in colors, that you can easily modify using Tailwind CSS classes (NOTE: each time you add a new class, a class that does not exist in `src/assets/styles/tailwind.css`, you will need to compile again tailwind).

2. See [Vue.js Configuration Reference](https://cli.vuejs.org/config/)

