<h3 id='req.route'>req.route</h3>

Contains the currently-matched route, a string. For example:

```js
app.get('/user/:id?', (req, res) => {
  console.log(req.route)
  res.send('GET')
})
```

Example output from the previous snippet:

```
{ path: '/user/:id?',
  stack:
   [ { handle: [Function: userIdHandler],
       name: 'userIdHandler',
       params: undefined,
       path: undefined,
       keys: [],
       regexp: /^\/?$/i,
       method: 'get' } ],
  methods: { get: true }
}
```
