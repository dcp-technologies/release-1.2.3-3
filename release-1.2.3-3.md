# Nouvelles Images du patch 1.2.3-3
```
dcptechnologies/api:x86-1.2.3-3
dcptechnologies/health:x86-1.2.3-3
dcptechnologies/podwatcher:x86-1.2.3-3
dcptechnologies/logwatcher:x86-1.2.3-3
```

# Arrêter les service DCP
```sh
helm -ndcp uninstall dcpapi
```

# env.sh
Dans le fihier "envs/env.sh", modifier la ligne suivante
```sh
API_VERSION=x86-1.2.3-3
```

# env-api.sh
Dans le fihier "envs/env-api.sh", mModifier la ligne suivante
```sh
MASTER_API_VERSION=1.2.3-3
```

# Installer l'api
```sh
./09-api.sh
```