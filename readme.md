Run `docker compose up`, let the daemon start, then kill the session with ctrl+c

To use the API, copy the config file from ipfs_data to the root directory, and modify API section: 

```
"HTTPHeaders": {
      "Access-Control-Allow-Origin": [
        "http://localhost:3000",
        "http://127.0.0.1:5001",
        "https://webui.ipfs.io"
      ],
      "Access-Control-Allow-Methods": [
        "PUT",
        "POST"
      ]
    }
```

To prevent hosting other files, set Gateway NoFetch to true.
