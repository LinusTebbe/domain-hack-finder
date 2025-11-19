# Domain Hack Finder

Simple website to find TLD in search strings in order to help with domain hacks. So searching for `emotes` will suggest
the spanish URL `emot.es`.

Whether they are available or not has to be checked manually.

[Visit Domain Hack Finder](https://domain-hack-finder.tancred.de/)

## For developers

### Development setup

1. Start the container

```bash
docker compose up -d
```

2. Connect to the container

```bash
docker exec -it domain-hack-finder-app-1 bash
```

3. Start the backend

```bash
deno task dev
```

4. In a second terminal, connect to the same container, then start the frontend

```bash
npm run dev --prefix frontend -- --host 0.0.0.0
```

### Production setup

```bash
docker compose -f docker-compose.prod.yml up -d
```

## Licsense

MIT
