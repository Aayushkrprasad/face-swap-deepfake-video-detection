# Deeptrace







SIH24 solution to problem statement no. 1683 by Synergia.

## Build

```bash
# Clone this repository
git clone https://github.com/Synergia-SIH24/face-swap-deepfake-video-detection.git
# Change directory into the project
cd face-swap-deepfake-video-detection
# Install updated dependencies (respects semver)
pnpm update
# Compose the docker compose file (pun intended)
docker compose -p deeptrace -f docker-compose.yaml up -d
# Rename .env.example to .env
mv .env.example .env # Modify the DATABASE_URL according to your needs
# Run migrations
pnpm db:generate
pnpm db:push
# Run dev server
pnpm dev
```
