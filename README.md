### Install
`npm install`

### Start the Server
Run server with `npm start`

### Open channel
```
curl -H Accept:text/event-stream http://localhost:3000/events
```

### Add Data which will be reflected in the SSE channel
```
curl -X POST \
 -H "Content-Type: application/json" \
 -d '{"momma": "swamp_princess", "eggs": 40, "temperature": 31}'\
 -s http://localhost:3000/nest
```
