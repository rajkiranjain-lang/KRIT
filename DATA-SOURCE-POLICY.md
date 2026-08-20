# READ60 Geographic Data Source Policy

## Authoritative source

READ60 will use **Survey of India (SoI), Government of India** as the authoritative source for political and administrative map data.

Survey of India's Online Maps Portal lists an **Administrative Boundary Database for entire country up to district level with HQ** as a shapefile product and states that the administrative boundary database covers state and district boundaries. The portal also identifies Survey of India as the content owner/maintainer.

Survey of India's geospatial guidelines state that for political maps of India, including national, state and other boundaries, Survey of India published maps or Survey of India digital boundary data are the standard to be used.

## Target dataset

**Administrative Boundary Database — Entire Country — Up to District Level with HQ**

Product code shown by the Survey of India portal: `OVSF/1M/7`.

## Integration rule

The raw authoritative dataset must be acquired from the official Survey of India portal, preserved as the source artifact where licensing permits, and converted to the browser format required by READ60 (for example GeoJSON) without changing the geographic meaning of the boundaries.

Any generated/converted browser dataset must retain provenance metadata pointing back to the official Survey of India source and acquisition/version information.

## Prohibited as source of truth

- AI-generated India silhouettes
- Hand-drawn political boundaries
- Random GitHub India GeoJSON repositories
- Maps that silently use disputed/neighbouring territory as India's administrative territory
- Unverified boundary datasets

## Project behavior

If the authoritative map data is unavailable or cannot be verified, READ60 must fail safely rather than silently substitute another map.
