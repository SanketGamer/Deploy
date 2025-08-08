//1. in Main project create .gitignore like- node_modules,.env (so that github can ignore them or remove them)
## vercel.json

Vercel json config for express backend

```bash
  {
    "version": 2,
    "builds": [
        {
            "src": "server.js",
            "use": "@vercel/node",
            "config": {
                "includeFiles": [
                    "dist/**"
                ]
            }
        }
    ],
    "routes": [
        {
            "src": "/(.*)",
            "dest": "server.js"
        }
    ]
}
```

Vercel json config to support React Router in frontend

```bash
  {
    "rewrites": [
      {
        "source": "/(.*)",
        "destination": "/"
      }
    ]
  }
```
