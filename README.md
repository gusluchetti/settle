# settle
Settle was my graduation thesis project (2021.2). We found that it was very hard for people moving to big cities to find dormitories to share with other students/young adults, when the only way to look for them was to search through a thousand posts on facebook, unfiltered, where most of them weren't even co-op postings to begin with.
Based on that, we attempted to create a website were people could, based on specific filters, search for dormitories that were best for them.

We developed a few micro-services and quite the beefy frontend. This is just a way to archive all the different modules and things we did along the way.

We had 5 repositories (all are merged together in this repo): 4 for the micro-services, one for the front-end.

## front
- This repo contains all things front-end, and it was built using React.

## maps
- The Maps micro-service was responsible, initially, for showing the Map on the 'list properties' screen, however, since that ended up being done on the front-end, it was just used to access a API to get an address based on the user's CEP (CEP Aberto).

## payment
- The Payment micro-service enabled us to integrate the Stripe API (albeit, just in test mode) with our application, so a user could pay for the spot on a dormitory with their credit-card.

## user
- The User micro-service was discontinued midway through the project; it was meant to do all the CRUD related actions for our users, but since we implemented Auth0, and it had a user database, there was no more need for our implementation.

## property
- The property micro-service was built with Typescript using AWS CDK, it managed the CRUD of the properties.
